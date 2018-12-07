---
layout: page
title: Background and methodology
---

I’m interested in understanding the publicly stated priorities of Canadian governments. This project is guided by the following overall question:

> How have the governments of different Canadian political parties described their priorities over the past 65 years?

This question implies a few different sub-questions:

* What issues have been discussed over the last 65 years?
	* Do these issues vary with time?
	* What issues have fallen out of the spotlight?
	* What issues have gained in prominence?
* Have different governing parties (namely, the Liberal and Conservative parties) spoken to these issues differently?
	* Are some issues discussed more by one party than the other?
	* Do the parties use different language to describe their priorities?

This is not a new field of study.

* changing values [Nevitte]
* stated priorities of parties in HoC QP [Penner, Blidook, Soroka]
* studying Throne Speeches [Bélanger?]
* others? [?]

While there are a number of avenues through which to study this issue, I decided to analyze Speeches from the Throne using topic modelling, supplemented with other forms of computerized textual analysis. For a specific question, then, this project investigates the following:

> What does topic modelling on Speeches from the Throne from 1953 to 2015 indicate about the changing public priorities of Canadian governments?

## Corpus

Corpus [cite LOP, LiPaD]
51 Speeches from the Throne
1953–2015
21 Parliaments (12 Liberal, 9 Conservative)
Why? Regular, standardized(ish), at least one of each party per decade, planned priorities

## Method

Topic modelling (MALLET and R)
Other textual analysis (Voyant) [for final analysis]


### Topic modelling considerations

### How I created my model

Process
1. Load corpus
[describe?]
2. Curate list of stopwords
	[provide stopwords]
3. Generate topics over and over again  (varying the number, e.g., 10, 15, 25, 30, 40)
	 [give a sample topic]