---
layout: page
title: Background and methodology
---

## Overview and scholarly context

I am interested in understanding the publicly stated priorities of Canadian governments. This project is guided by the following overall question:

> How have the governments of different Canadian political parties described their priorities over the past 65 years?

This question implies a few different sub-questions:

* What issues have been discussed over the last 65 years?
	* Do these issues vary with time?
	* What issues have fallen out of the spotlight?
	* What issues have gained in prominence?
* Have different governing parties (namely, the Liberal and Conservative parties) spoken to these issues differently?
	* Are some issues discussed more by one party than the other?
	* Do the parties use different language to describe their priorities?

This is not a new field of study. Other scholars have considered this broad question from different angles, using a variety of methods:

* Though not focused explicitly on the study of political parties, Nevitte ([1996](/references/#ref-nevitte-1996)) considered the changing values of Canadians, political and otherwise, between 1981 and 1990. Nevitte’s study drew on the World Values Survey, an extensive public opinion project, based on the premise that “the best way to find out about people’s values is to ask them” (20). This statistical analysis of survey data was able to demonstrate trends over time in popular opinion on numerous questions of values. While not directly related to this project’s question, such an approach can offer an interesting proxy into what political parties might prioritize, as parties must ultimately be responsive to popular opinion.

* More directly related is the work of Penner, Blidook, and Soroka ([2006](/references/#ref-penner-blidook-soroka-2006)). Penner, Blidook, and Soroka developed a coded database of 19,000 questions asked during Question Period in the House of Commons between 1988 and 1999. With this database, they investigated which issues parties spoke to most often, and categorized the nature of those issues as either “generalized” (appealing to the entire electorate) or “particularized” (appealing to some subsection of the electorate). Each question was manually coded according to a set of policy topics drawn from similar research in the United States (1009–1010), such that each question had one topic. The authors note that analysis on such a corpus can only speak directly to the priorities of *opposition* parties, as they ask most of the substantive questions during Question Period (1009). This approach, however, is a useful example for this project, in that it demonstrates that the words spoken in Parliament are valid measures of their speaker’s priorities.

* Montpetit and Foucault ([2012](/references/#ref-montpetit-foucault-2012)) also examined this question of policy attention. Analyzing speeches from the throne delivered in the United Kingdom, the Canadian federal government, and Canadian provinces, Montpetit and Foucault examined when policy attention changes. Though the specific question they ask is of less relevance, their approach is highly so. Based on existing academic literature, Montpetit and Foucault identified speeches from the throne as a particularly strong corpus for the study of *government* (as opposed to opposition) priorities (643–644). They manually coded each speech, capturing the range of policy issues to which it referred, finding that the distribution of topic issues per speech corresponded to their intuitive sense of the various governments’ priorities (644–647). Montpetit and Foucault’s example is a useful one for this project, as it identifies speeches from the throne as a suitable corpus, and suggests one way to identify the government priorities expressed within that corpus.

From this grounding in existing literature, I decided to analyze speeches from the throne using topic modelling, supplemented with other forms of computerized textual analysis. For a specific question, then, this project investigates the following:

> What does topic modelling on speeches from the throne delivered in the Canadian House of Commons between 1953 and 2015 indicate about the changing public priorities of federal governments?

## Corpus

Speeches from the throne are a strong corpus for studying the public priorities of governing parties. They have several advantages:

* They are delivered regularly. At the start of each parliamentary session (which occur at least once during each Parliament, though most governments have opted to split their Parliament up into multiple sessions), the governing party prepares the speech, which is delivered by the Queen or her representative, the governor general ([Cochrane, Blidook, and Dyck 2017](/references/#ref-cochrane-blidook-dyck-2017), 573). This regularity means that there is data available for each government during this period.

* They have a relatively standardized form. Speeches from the throne outline government priorities, and have the unique advantage of describing policy issues that may be acted on through either legislative or budgetary measures ([Montpetit and Foucault 2012](/references/#ref-montpetit-foucault-2012), 644). This means that speeches from the throne can offer a more comprehensive overview of a government’s priorities than can be obtained through studying either legislation or budgets alone.

Admittedly, speeches from the throne are not a perfect corpus. There may be issues on which a government is intensely focused during a parliamentary session that, for whatever reason, it does not mention in its speech from the throne. Accordingly, I can draw conclusions only on the public priorities stated by governments during their speeches from the throne. I do not mean to imply that these are a government’s *only* priorities.

This project is based on an analysis of the 51 speeches from the throne delivered between 1953 and 2015. I gathered these speeches from both [the Library of Parliament’s list of speeches](https://lop.parl.ca/sites/ParlInfo/default/en_CA/Parliament/procedure/throneSpeech) and the [Linked Parliamentary Data Project, LiPaD](https://www.lipad.ca/). I used LiPaD’s digitized record for the 35 speeches that the Library of Parliament had not converted from PDF, as LiPaD’s versions include significant optical character recognition corrections, amid other improvements ([Beelen et al. 2017](/references/#ref-beelen-etal-2017)). The 51 speeches total over 158,000 words; the longest is 7,206 words, while the shortest is 144 words.

The time period in question, 1953–2015, spans 21 Parliaments. 12 of these Parliaments had Liberal governments, while 9 had Conservative governments. (I group the Progressive Conservative Party and the modern Conservative Party of Canada under the shared label “Conservative”.) This time period includes at least one speech from the throne from each party during each decade from the 1950s to the 2010s.

## Method

I chose topic modelling as a digital tool with which to analyze this corpus.

Topic modelling uses a computer algorithm (run by a program such as [MALLET](http://mallet.cs.umass.edu/)) to infer statistically significant groups of words that appear in a collection of texts. Graham, Weingart, and Milligan explain the approach clearly in [a tutorial at *The Programming Historian*](https://programminghistorian.org/en/lessons/topic-modeling-and-mallet):

> Topic models represent a family of computer programs that extract topics from texts. A topic to the computer is a list of words that occur in statistically meaningful ways. A text can be an email, a blog post, a book chapter, a journal article, a diary entry – that is, any kind of unstructured text. By unstructured we mean that there are no computer-readable annotations that tell the computer the semantic meaning of the words in the text.
> 
> Topic modeling programs do not know anything about the meaning of the words in a text. Instead, they assume that any piece of text is composed (by an author) by selecting words from possible baskets of words where each basket corresponds to a topic. If that is true, then it becomes possible to mathematically decompose a text into the probable baskets from whence the words first came. The tool goes through this process over and over again until it settles on the most likely distribution of words into baskets, which we call topics. ([Graham, Weingart, and Milligan 2012](/references/#ref-graham-weingart-milligan-2012))

For a very practical (and amusing) example of how topic modelling works, “[The LDA Buffet is Now Open; or, Latent Dirichlet Allocation for English Majors](http://www.matthewjockers.net/2011/09/29/the-lda-buffet-is-now-open-or-latent-dirichlet-allocation-for-english-majors/)” ([Jockers 2011](/references/#ref-jockers-2011)) explains the technique well.

Each topic is a list of words with associated weights. The first eight words in [one topic that I generated](/topics/3-olympic-athletes-winter/), for example, are “olympic athletes winter step planning unnecessary stories gold”. Texts are then compared each topic’s list of words weights to see how much of the text is reflected in that topic. The weight of the word determines its importance to the topic—a topic actually contains much more than eight words, but the weight of some is so minimal as to not influence these calculations.

Topic modelling has been put to some use in historical research. Perhaps the best known example is Nelson’s “[Mining the _Dispatch_](http://dsl.richmond.edu/dispatch/)”, which combines topic modelling with an innovative approach to web-based scholarship ([Nelson](/references/#ref-nelson-nd)). More in the vein of this project, in 2014, Milligan offered an early example of topic modelling for political history. He ran a topic modelling algorithm on the entirety of the Canadian Hansard (the official parliamentary record) between 1994 and 2012, extracting several topics and using them to evaluate a thesis on a shifting narrative surrounding Canada’s portrayal to the outside world ([Milligan 2014](/references/#ref-milligan-2014)).

Topic modelling offers two notable advantages when analyzing speeches from the throne over manual coding:

* It allows for multiple “codes” per speech, as a topic is merely a collection of words—one text can be made up of several topics.

* Topics are inferred from the content of speeches instead of imposed from the “outside,” allowing us to find potentially significant concepts that may otherwise pass unnoticed with a restricted list of pre-existing topics.

### Topic modelling considerations

Based on a survey of literature related to topic modelling ([Blevins 2010](/references/#ref-blevins-2010); [Graham, Weingart, and Milligan 2010](/references/#ref-graham-weingart-milligan-2012); [Jockers 2011](/references/#ref-jockers-2011); [Milligan 2014](/references/#ref-milligan-2014); [Weingart 2012a](/references/#ref-weingart-2012a); [Weingart 2012b](/references/#ref-weingart-2012b); [Yang, Torget, and Rada 2011](/references/#ref-yang-torget-rada-2011)), I identified the following important points to consider in using topic modelling for research:

* Computers do not understand the _meaning_ of texts, so topics do not have any inherent meaning. Rather, the researcher assigns meaning to these topics. Often they do so through a label. Accordingly, I labelled and annotated the most interesting topics. (You can [see the full list](/topics/) or [read my focused analysis](/discussion/).)

* Most documents in the corpus will be made up of several topics, while some topics may only appear within one document.

* Researchers must develop a list of stopwords to prevent the topic modeller from incorporating frequently used but “meaningless” words. (“Meaningless” is relative, which is why the researcher must put some thought into the development of this list.)

* The number of topics must be *chosen* by the researcher. There is no optimal number of topics—as I note below, I varied the number of topics produced by the algorithm until I settled on a number that seemed right. Ultimately, though, the number is a choice.

* Topic modelling should be used alongside other research methods, such as close reading. Accordingly, when analyzing certain topics I read seemingly notable speeches and turned to [Voyant](https://voyant-tools.org/) for standard textual analysis tools like term and phrase frequency.

* Topic modelling does not necessarily _prove_ anything about the corpus, but it can offer new interpretations for further research.

### How I created my model

1. I first loaded my corpus (described above) into MALLET.

2. I then curated my list of stopwords. In addition to Voyant’s automatically-generated list (based on common English words), I added the following:

	```
	government
	members
	ministers
	parliament
	parliamentary
	parliamentarians
	senate
	house
	commons
	speech
	throne
	th
	session
	```
	I assembled this list by looking at the most frequent words and removing any that seemed to appear only in “routine” portions of the speeches—namely, the openings and closings.

3. I then generated topics numerous times. I varied the number of topics, comparing the results when I tried to generate 10, 15, 20, 25, 30, 35, or 40 topics. I ultimately settled on [30 topics](/topics/), as I found that this seemed to strike a good balance between having meaningful topics that were also distinct from one another.
