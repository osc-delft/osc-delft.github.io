---
layout: page
title: OSC Delft members
image: /images/syllabus.jpg
photos:
  name: Niklas Morberg
  license: CC BY-NC 2.0
  url: https://flic.kr/p/5BXB6s
---

{% assign people = site.data.people %}
{% assign metadata = site.data.members-metadata %}

Our community members are *some description of roles of community members*.

If you would like to join the community, please fill in the form here - our community coordinator will be in touch within a week.

# Aerospace Engineering (AE)

<!-- Any modification of the content should be done in the _data/ols-2-projects.yaml file -->

<div class="people">
{% for entry in metadata.ae %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>

# Civil Engineering & Geosciences (CEG)
<div class="people">
{% for entry in metadata.ceg %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>
