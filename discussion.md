---
layout: page
title: Discussion of results
---

Let us return to this project’s guiding question:

> What does topic modelling on speeches from the throne delivered in the Canadian House of Commons between 1953 and 2015 indicate about the changing public priorities of federal governments?

Much of my analysis is contained within my annotations of specific topics. Here are the topics that I annotated with analysis:

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

## Trends in public priorities

To try to provide some response to this work’s guiding question, I offer the following observations:

* the [rise in interest in social policy](/topics/6-health-communities-children/), the [rise in mentions of the environment and women](/topics/8-plan-economy-values/) (including the shifting connotations of those words)