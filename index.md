---
layout: page
title: welcome to my site
---

Hi! Lorem ipsum dolor sit amet.

This is a place for my projects and thoughts!  
I like to draw and code.  
Here are some of the things I've done:

- [project 1: proident aperiam]({{ '/projects/project-1/' | relative_url }})
- [project 2: nemo eu]({{ '/projects/project-2/' | relative_url }})
- [project 3: inventore ea]({{ '/projects/project-3/' | relative_url }})

Reprehenderit iste aliquip voluptatem cupidatat voluptatem inventore sit culpa deserunt natus quae ipsam. Eaque ipsam id in quae omnis consectetur dicta irure veritatis. Aliqua velit dicta vitae elit aut ex sit.

> Commodo aliquip ipsam excepteur laboris voluptas dicta explicabo unde rem.

## latest posts

{% for post in site.posts limit:5 %}
- {{ post.date | date: "%Y-%m-%d" }}: [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
