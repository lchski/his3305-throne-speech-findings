---
layout: page
title: Discussion of results
---

## Trends in public priorities

Let us return to this project’s guiding question:

> What does topic modelling on speeches from the throne delivered in the Canadian House of Commons between 1953 and 2015 indicate about the changing public priorities of federal governments?

To try to provide some response to this work’s guiding question, I offer the following observations:

* Over this period, there appears to have been rising interest in both [social policy](/topics/6-health-communities-children/) and [the environment and women](/topics/8-plan-economy-values/).

* In terms of [the environment and women](/topics/8-plan-economy-values/), the connotations of those words shifted: the environment became an active issue of protection and regulation, while attention to women’s issues shifted from women in general to certain specific groups of women and girls.

* Governments sometimes use speeches from the throne to speak to events going on in the world at the time. Certain “public priorities” thus only appear at certain periods, such as [the 1973 oil crisis](/topics/10-oil-food-transportation/), [the renewed efforts at constitutional negotiation in the 1980s](/topics/20-national-cooperation-objectives/), or [the response to the 2008 market crash](/topics/11-jobs-protect-businesses/). This demonstrates that governments do indeed appear responsive to the world around them, crafting their public priorities based on contemporary events.

* Certain governments try to “own” a particular issue, using unique language to carve out their own vision, [as the Harper Conservatives did with northern sovereignty](/topics/18-families-hard-north/).

* In the 21st century, there may be a new trend of governments adopting [very open language in their first speech from the throne](/topics/17-trust-stronger-middle/). This emphasis on trust, transparency, and accountability may be less a true priority than a rhetorical device used when a government is young.

Other observations from my analysis are contained within my annotations of specific topics. Here are the topics I annotated:

<ul>
    {% assign sorted_topic_annotations = site.topic_annotations | sort: "topic_number_sort" %}
    {% for topic_annotation in sorted_topic_annotations %}
        <li>
            #{{ topic_annotation.topic_number }}: <a href="{{ topic_annotation.url }}">{{ topic_annotation.title }}</a>
        </li>
    {% endfor %}
</ul>

## Types of topics

In analyzing the topics, I identified several types of topics:

* *Issue.* An issue topic refers to an issue of public policy. For example, “[social policy](/topics/6-health-communities-children/)” or “[private sector rights](/topics/21-private-initiatives-sector/)”. This is the type of topic that seems is most useful to answer the project’s overall question.

* *Event.* An event topic refers to some historical event going on at the time. For example, the [1973 oil crisis](/topics/10-oil-food-transportation/) or the [2010 Olympic games](/topics/3-olympic-athletes-winter/).

* *Author.* An author topic contains language that is strongly associated with one particular government (a political party at a certain point in time). For example, [the Harper Conservatives’ distinctive political language](/topics/18-families-hard-north/).