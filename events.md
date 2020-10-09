---
layout: page
title: OLS-2 schedule
image: https://images.unsplash.com/photo-1435527173128-983b87201f4d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1047&q=80
photos:
  name: Eric Rothermel
  license: CC BY
  url: https://unsplash.com/photos/FoKO4DpXamQ
---

{% assign schedule = site.data.events %}
{% assign cohort = 'ols-2' %}

This is a list of events organised by members of the Open Science Community Delft that can be of interest to other members.

If you would like to add an event here, please submit an issue on GitHub using this template.

# Events

{% for event in schedule %}

## {{ event.title }}

<i class="fas fa-calendar-alt"></i> **Date & time**: {{ event.date_time }}

<i class="fas fa-calendar-alt"></i> **Location**: {{ event.location }}

{% if content %}

{{ event.content | markdownify }}

{% endif %}

{% if event.website %}
**Find out more** at [the event website]({{ event.website }})
{% endif %}

{% endfor %}
