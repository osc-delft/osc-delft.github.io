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

<div id = "AE" class="people">
{% for entry in metadata.ae %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>

# Applied Sciences (AS)
<div id="AS" class="people">
{% for entry in metadata.as %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>

# Architecture and the Built Environment (ABE)
<div id="ABE" class="people">
{% for entry in metadata.abe %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>

# Civil Engineering & Geosciences (CEG)
<div id="CEG" class="people">
{% for entry in metadata.ceg %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>

# Electrical Engineering, Mathematics and Computer Science (EEMCS)
<div id="EEMCS" class="people">
{% for entry in metadata.eemcs %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>

# Industrial Design Engineering (IDE)
<div id="IDE" class="people">
{% for entry in metadata.ide %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>

# Mechanical, Maritime and Materials Engineering (3mE)
<div id="threemE" class="people">
{% for entry in metadata.threemE %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>

# Technology, Policy and Management (TPM)
<div id="TPM" class="people">
{% for entry in metadata.tpm %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>

# Non-Faculty
<div id="NF" class="people">
{% for entry in metadata.other %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>

# Alumni
<div id="Alumni" class="people">
{% for entry in metadata.alumni %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>
