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

Our community members:
- are interested in learning, adopting, and/or advocating for open science practices
- receive and can contribute to a bi-monthly open science news ([read past newsletters here](https://github.com/osc-delft/newsletters))
- attend our [community meet-ups and events](https://osc-delft.github.io/events), e.g. the Data Champions bi-annual meetings
- can start [open science initiatives](https://osc-delft.github.io/initiatives) within TU Delft

If you would like to join the community, please [fill in this sign up form](https://osc-delft.github.io/join) - our community coordinator will be in touch within two weeks.

If you spot any errors on the list below or would like to update some information on your profile, please [submit an issue](https://github.com/osc-delft/osc-delft.github.io/issues/new/choose) or [email the community coordinator](mailto:opensciece@tudelft.nl)

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
