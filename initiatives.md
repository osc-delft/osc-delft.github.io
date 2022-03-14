---
layout: page
title: OSC Delft Initiatives
image: /images/initiatives.jpg
photos:
  name: picjumbo_com
  license: https://pixabay.com/service/license/
  url: https://pixabay.com/photos/tools-construct-craft-repair-864983/
---

{% assign people = site.data.people %}
{% assign metadata = site.data.members-metadata %}

**Open Science Community Delft initiatives are:**
- Designed by and for community members, with the goal to bring together community members with similar interest or goals to dive deeper/learn more about a certain are of open science
- Open to participation from all OSC Delft members

**All OSC Delft members can propose or start a new initiative.** Likewise, existing TU Delft communities can become an initiative of Open Science Community Delft. The advantages of being an OSC Delft initiative are:
- Having a big, diverse network of like-minded people to reach out to, encouraging otherwise unlikely collaborations
- Access to an online infrastructure to build upon - you don't need to build a website or social media account from scratch to start
- Benefit from the collective existing knowledge of the community members and community managers
- Assistance with event organisation and community management, e.g. running mailing lists

If you would like to start a new initiative or bring your community into OSC Delft, please use our [idea sandbox](https://github.com/osc-delft/ideas-and-plans) to propose and discuss the idea, or [email our community coordinator](mailto:openscience@tudelft.nl).

# Data champions

- Are you practising or advocating for good research data management?
- Would you like to share your data management tips and tricks in your group/department?
- Would you like to get rewarded for that?

If you answered 'yes' to any of the above, consider joining OSC Delft and becoming a data champion!

## What do data champions do?
- *Advocate* for research data management and sharing at the department/group/section - data champions help spread the word about the latest developments and opportunities regarding data/code, and establish good data practices within their groups and/or departments
- *Inform* policy, service and training development - data champions work closely with faculty data stewards and help design and offer input and feedback for data policies, workflows, tools and training
- *Speak* to others about their experience with data management during departmental and section presentations and training events- data champions are considered local experts on data-related issues.
- *Network* with other data champions from different faculties and departments through participating in bi-annual meetings for all TU Delft’s Data Champions

## Data champions rewards
- Build new networks and collaborations - data champions have reached out through the network to find new collaborations for projects and grant applications
- Recognition by faculty management - faculty management and staff recognise and value the input and expertise from data champions in data-related initiatives
- Upskilling opportunities - for example, data champions can hone their communication skills through presenting to a large, diverse audience
- Close working relationships with faculty data stewards, faculty support staff and staff from the university corporate offices, e.g. Library, ICT,


## Become a data champion
[Join OSC Delft](https://osc-delft.io/join) - in the onboarding email, you will be given the option to sign up to become a data champion.

## Who are data champions?

<div id = "datachampions" class="people">
{% for entry in metadata.datachampions %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>

# Delft Open Hardware

**Delft Open Hardware** is a bottom-up community of students, researchers, university staff and alumni at TU Delft, started in September 2019. We believe that open source software and hardware are game changers in education, research and sustainability. This is why we work on open source hardware projects and run events where we share our expertise and passion with others.

## What is open source hardware?
Open (source) hardware means releasing publicly the source of how hardware is designed so that anyone can study, improve and distribute the technology. By doing so, everyone: engineers, developers, end-users and other stakeholders, are free to improve and decide how the projects evolve on the basis of innovative ideas,
excellent work and, intensive peer review for and quality assurance.

## What do Delft Open Hardware members do?
- Design and develop open hardware projects together, through sharing our ideas in meetups and our Telegram group.
  - See some of our [running hardware projects](https://delftopenhardware.nl/projects/)
- Organise training and events to raise awareness around open hardware
- (coming soon!) Mentor and supervisor open hardware bachelor & master theses projects and internships
- (Coming soon!) Manage a makers space

[Visit the Delft Open Hardware website](https://delftopenhardware.nl/) to find out more, and [join our community](https://docs.google.com/forms/d/e/1FAIpQLSdSR4w9Im24kFD_bJfGQ3pl8TsqOAIqJUTgEa9Rm22RzcAwkg/viewform)!

## Open Hardware community members

<div id = "openhardware" class="people">
{% for entry in metadata.openhardware %}
    {% assign username = entry %}
    {% assign user = people[username] %}
    {% include _includes/people.html username=username user=user %}
{% endfor %}
</div>
