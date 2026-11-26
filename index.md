---
layout: page
title: The peak of the iceberg of Lio Dubois
---


Can't safely self host for a while, too many downtimes because of electrical issues in the place I live in right now.
So made this, it's built using a CI with jekyyll processing .md files for content on a github repo.
I'll try to keep it updated and to be my main hub for ever.



> Texts are full of spelling mistakes that I keep on purpose to show it's fully handwritten on the moment without AI.

## latest posts

{% for post in site.posts limit:5 %}
- {{ post.date | date: "%Y-%m-%d" }}: [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
