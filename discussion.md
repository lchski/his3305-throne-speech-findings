---
layout: page
title: Discussion of results
---

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

* event TODO
* issue TOOD
* author TODO
* 

## Trends in public priorities

[quote project question]

the [rise in interest in social policy](/topics/6-health-communities-children/), the [rise in mentions of the environment and women](/topics/8-plan-economy-values/) (including the shifting connotations of those words)