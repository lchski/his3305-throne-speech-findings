---
layout: page
title: Conclusions, project implications, next steps
---

My main conclusions about the project’s guiding question are noted in the [discussion section](/discussion/). Here, I explore what the project taught me about using topic modelling, about speeches from the throne as a corpus, and about the combination of the two for the study of government priorities. I also expand on some potential next steps.

## What can we learn about...

### ...topic modelling?

Topic modelling is a useful tool to quickly get a sense of a corpus. Some prior knowledge is certainly beneficial to help determine the number of topics and to get a sense of what the topics mean. But for those with little to no knowledge of an historical period, topic modelling can quickly reveal interesting points on which to dive in, such as the [1973 oil crisis](/topics/10-oil-food-transportation/), by identifying major points of discussion at certain times. However, one must be careful not to draw unfounded conclusions: the [various mentions of the Arctic between 2006 and 2015](/topics/18-families-hard-north/), for example, likely had less to do with a particular historical event than with the political interests of the governing party at the time.

Topics like “[declining parliamentary formality](/topics/24-act-asked-provide/)” reveal the great potential of topic modelling as a tool to suggest research opportunities. Admittedly, it is not a particularly relevant topic to this project’s overall question. But it suggested an entirely new path of research—thanks to topic modelling, I was better able to think through the corpus and understand its possibilities for research.

### ...speeches from the throne?

They do offer a decent corpus for analyzing priorities. We were able to observe, for example, the [rise in interest in social policy as a broad issue area](/topics/6-health-communities-children/). That said, they are not an exhaustive listing of a government’s priorities, and many more nuanced or niche issues may not have been picked up by the topic modeller.

That said, the topic modeller would have been more effective with a larger corpus. 158,000 words and 51 documents is relatively small for topic modelling. It may have been more fruitful to use a corpus like yearly budget speeches, and to expand the years under analysis. However, for the purposes of this small project, speeches from the throne worked well enough.

### ...government priorities?

Ultimately, the topics generated did not surface too many “issue” topics. Given the constraints of topic modelling, noted above, this is not necessarily a surprise.

The approach taken by Montpetit and Foucault (CITEME 2012), tagging portions of sentences with specific policy issues, would be more effective at exhaustively identifying the priorities discussed by governments in speeches from the throne. However, such an approach may not have yielded the alternative conclusions suggested by topic modelling, and it would have taken far more time.

Nonetheless, we were able to observe various trends, as noted in [the discussion section](/discussion/). While this corpus and tool could not provide an extremely detailed portrait of such trends, it was certainly able to point to some shifts.

## Next steps

This work suggested a variety of paths for future research:

* Further explore each of [the thirty topics identified](/topics/). Given my limited time, I prioritized ten for annotation, but each topic could potentially yield interesting results.

* One of topic modelling’s great features is that one can take the topics generated on one corpus and check them against other corpora, to see whether the topics are equally prevalent. It would be interesting to take the list of issue topics from speeches from the throne and compare them with other political documents, to see whether these priorities are mentioned only within speeches from the throne or whether they indicate a more general historical trend.

* One specific example of this would be to compare [the formality topic]((/topics/24-act-asked-provide/)) with speeches delivered by the governor general outside of Parliament and speeches delivered by the prime minister. 

	This would allow for two additional perspectives: the governor general would provide an “institutional” perspective (What formality does the governor general use when they write their own speeches?) a “political” perspective (Does the formality of political prime ministerial speeches correspond to the shifting formality of speeches from the throne?). With these perspectives, we could investigate whether the formality has indeed decreased.

* Another example would be to compare [the “new government rhetoric” topic](/topics/17-trust-stronger-middle/) with other political documents from both the Harper Conservatives and Trudeau Liberals after their first speech from the throne  (prime ministerial speeches, press releases, etc.), to see whether that language continues to appear or not.

* Though time did not allow for me to clean up and properly annotate my codebase, I would also like to publish the code I used to generate my models and produce my data. As topic modelling is still relatively rare in historical research, offering a practical example of how I processed my data could be useful to other researchers. (And it would allow anyone interested to pick up the analysis where I left it.)