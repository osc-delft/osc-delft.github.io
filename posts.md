---
layout: posts
title: Our stories
image: /images/posts.jpg
photos:
  name: Julia Joppien
  license: https://unsplash.com/license
  url: https://unsplash.com/photos/-3wygakaeQc
---

This is a collection of articles, blog posts and reports written by community members and coordinators.

Your article can also be featured here!
- Do you have an existing blog post, publication or presentation related to open science that you would like to share with another community member? You can request to link to it from this page! Please [submit an issue](https://github.com/osc-delft/osc-delft.github.io/issues) with a URL to the article.
- Would you like to share your ideas, thoughts and/or experience about open science with other community members? You can write a blog post here. [Contact our community coordinator](mailto:openscience@tudelft.nl). We will also happy to advise on writing and help editing, and brainstorm and co-author the post with you!

{% assign date_format = site.minima.date_format | default: "%b %-d, %Y" %}

<div class="post">
{% for post in site.posts %}
    {% capture authors %}
    {% for id in post.authors %}, {% assign name = site.data['people'][id].name | default: id %}{{ name }}{% endfor %}
    {% endcapture %}
    <div class="card">
        {% if post.image %}
        <div class="card-image">
            <figure class="image">
              <img src="{{ post.image }}" alt="{{ post.title }}">
            </figure>
        </div>
        {% endif %}

        <div class="card-content">
            <div class="content">
                <p class="title">
                {% if post.external %}
                    <a href="{{ post.external }}" target="_blank">{{ post.title | escape }}</a>
                {% else %}
                    <a href="{{ post.url }}">{{ post.title | escape }}</a>
                {% endif %}
                </p>

                <p class="subtitle">
                    <time datetime="{{ post.date | date: date_format }}">{{ post.date | date: date_format }}</time>
                    - {{ authors | remove_first: ', ' | strip }}
                </p>

                {{ post.excerpt }}
            </div>
        </div>
    </div>
{% endfor %}
</div>
