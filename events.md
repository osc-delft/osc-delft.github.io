---
layout: page
title: Community events
image: https://images.unsplash.com/photo-1435527173128-983b87201f4d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1047&q=80
photos:
  name: Eric Rothermel
  license: CC BY
  url: https://unsplash.com/photos/FoKO4DpXamQ
---

<div style="display: flex; justify-content: center;">
    <img src="https://github.com/osc-delft/osc-delft.github.io/blob/master/images/red-box-declare-out-of-date.png?raw=true" width="1000">
</div>
<p style="text-align:center; font-size:36px;"><a href="https://www.tudelft.nl/en/open-science/community">Click here for new website</a></p>

{% assign schedule = site.data.events %}

This is a list of events organised by members of the Open Science Community Delft that can be of interest to other members.

If you would like to add an event here, please [submit an issue on GitHub](https://github.com/osc-delft/osc-delft.github.io/issues/new?assignees=&labels=&template=event-listing-submission-template.md&title=Event).

{% for event in schedule %}

# {{ event.title }}

<i class="fas fa-calendar-alt"></i> **Date & time**: {{ event.date_time }}

<i class="fas fa-calendar-alt"></i> **Location**: {{ event.location }}

{% if content %}

{{ event.content | markdownify }}

{% endif %}

{% if event.website %}
**Find out more** at [the event website]({{ event.website }}){:target="_blank"}
{% endif %}

{% endfor %}
