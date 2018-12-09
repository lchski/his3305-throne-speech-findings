---
layout: page
title: Background and methodology
---

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

* Though not focused explicitly on the study of political parties, Nevitte (CITEME 1996) considered the changing values of Canadians, political and otherwise, between 1981 and 1990. Nevitte’s study drew on the World Values Survey, an extensive public opinion project, based on the premise that “the best way to find out about people’s values is to ask them” (20). This statistical analysis of survey data was able to demonstrate trends over time in popular opinion on numerous questions of values. While not directly related to this project’s question, such an approach can offer an interesting proxy into what political parties might prioritize, as parties must ultimately be responsive to popular opinion.
* More directly related is the work of Penner et al. (CITEME 2006). Penner et al. developed a coded database of 19,000 questions asked during Question Period in the House of Commons between 1988 and 1999. With this database, they investigated which issues parties spoke to most often, and categorized the nature of those issues as either “generalized” (appealing to the entire electorate) or “particularized” (appealing to some subsection of the electorate). Each question was manually coded according to a set of policy topics drawn from similar research in the United States (1009–1010), such that each question had one topic. The authors note that analysis on such a corpus can only speak directly to the priorities of *opposition* parties, as they ask most of the substantive questions during Question Period (1009). This approach, however, is a useful example for this project, in that it demonstrates that the words spoken in Parliament are valid measures of their speaker’s priorities.
* Montpetit and Foucault (2012) also examined this question of policy attention. Analyzing speeches from the throne delivered in the United Kingdom, the Canadian federal government, and Canadian provinces, Montpetit and Foucault examined when policy attention changes. Though the specific question they ask is of less relevance, their approach is highly so. Based on existing academic literature, Montpetit and Foucault identified speeches from the throne as a particularly strong corpus for the study of *government* (as opposed to opposition) priorities (643–644). They manually coded each speech, capturing the range of policy issues to which it referred, finding that the distribution of topic issues per speech corresponded to their intuitive sense of the various governments’ priorities (644–647). Montpetit and Foucault’s example is a useful one for this project, as it identifies speeches from the throne as a suitable corpus, and suggests one way to identify the government priorities expressed within that corpus.

* methodological examples, e.g. topic modelling and automatic analysis of LiPaD

From this grounding in existing literature, I decided to analyze speeches from the throne using topic modelling, supplemented with other forms of computerized textual analysis. For a specific question, then, this project investigates the following:

> What does topic modelling on speeches from the throne delivered in the Canadian House of Commons between 1953 and 2015 indicate about the changing public priorities of federal governments?

## Corpus

Speeches from the throne are a strong corpus for studying the public priorities of governing parties. They have several advantages:

* They are delivered regularly. At the start of each parliamentary session (which occur at least once during each Parliament, though most governments have opted to split their Parliament up into multiple sessions), the governing party prepares the speech, which is delivered by the Queen or her representative, the governor general (CITEME Cochrane, Blidook, and Dyck 2017, 573). This regularity means that there is data available for each government during this period.
* They have a relatively standardized form. Speeches from the throne outline government priorities, and have the unique advantage of describing policy issues that may be acted on through either legislative or budgetary measures (CITEME Montpetit and Foucault 2012, 644). This means that speeches from the throne can offer a more comprehensive overview of a government’s priorities than can be obtained through studying either legislation or budgets alone.

Admittedly, speeches from the throne are not a perfect corpus. There may be issues on which a government is intensely focused during a parliamentary session that, for whatever reason, it does not mention in its speech from the throne. Accordingly, I can draw conclusions only on the public priorities stated by governments during their speeches from the throne. I do not mean to imply that these are a government’s *only* priorities.

This project is based on an analysis of the 51 speeches from the throne delivered between 1953 and 2015. I gathered these speeches from both [the Library of Parliament’s list of speeches](https://lop.parl.ca/sites/ParlInfo/default/en_CA/Parliament/procedure/throneSpeech) and the [Linked Parliamentary Data Project, LiPaD](https://www.lipad.ca/). I used LiPaD’s digitized record for the 35 speeches that the Library of Parliament had not converted from PDF, as LiPaD’s versions include significant optical character recognition corrections, amid other improvements (CITEME Beelen et al. 2017).

The time period in question, 1953–2015, spans 21 Parliaments. 12 of these Parliaments had Liberal governments, while 9 had Conservative governments. (I group the Progressive Conservative Party and the modern Conservative Party of Canada under the shared label “Conservative”.) This time period includes at least one speech from the throne from each party during each decade from the 1950s to the 2010s.

## Method

Topic modelling (MALLET and R)
Other textual analysis (Voyant) [for final analysis]

[following example of Penner et al. in terms of using words spoken in Parliament and coding topics. however, topics here are *inferred* from the text instead of imposed. also, different scale. also, government instead of opposition (different corpus).]

[one topic works for QP Qs, while multiple topics makes more sense for a lengthier document like a speech from the throne]

[automatic coding instead of manual]

### Topic modelling considerations

### How I created my model

Process
1. Load corpus
[describe?]
2. Curate list of stopwords
	[provide stopwords]
3. Generate topics over and over again  (varying the number, e.g., 10, 15, 25, 30, 40)
	 [give a sample topic]