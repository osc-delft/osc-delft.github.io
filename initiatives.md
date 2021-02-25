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

If you would like to start a new initiative or bring your community into OSC Delft, please use our [idea sandbox](https://github.com/osc-delft/ideas-and-plans) to propose and discuss the idea, or [email our community coordinator](mailto:f.tsang@tudelft.nl)

# Data champions

- Are you practising or advocating for good research data management?
- Would you like to share your data management tips and tricks in your group/department?
- Would you like to get rewarded for that?

If you answered 'yes' to any of the above, consider joining OSC Delft and becoming a data champion!

## What do data champions do?
- Act as advisors/mentors to other in their department/group/section
- Advocate for research data management and sharing at the department/group/section
- Speak to others about own experience with data management during departmental and section presentations and training events. Data Champions will be able to apply to the dedicated Data Champions Training Fund to get financial support to organise these.
- Work closely with your faculty data stewards and participate in Data Champions meetings at your faculty
- Participate in bi-annual meetings for all TU Delft’s Data Champions

## Data champions rewards
- **Network building**: connect with and to learn from other people interested in data stewardship from other departments and faculties, through opportunities to attend international conferences - you can apply for a dedicated Data Champions Travel and Training Fund for this, and will receive regular updates about interesting conferences and workshops
- **Inform development of research data services**: serve as local subject experts and be consulted (optional) bout new central initiatives related to research data stewardship and software sustainability
- **Financial incentives**: access to any new data stewardship-related funding opportunities available at TU Delft; Can apply for a dedicated Data Champions Travel and Training Fund to organize or attend activities relating to research data management/sharing at TU Delft or elsewhere
- **Learn new skills**: you can attend training and workshops to learn more about good data stewardship and about data services available at TU Delft; hone your communication and presentation skills by presenting at departmental and faculty training and events
- **Increased impact**: you will become the local experts on data stewardship, and will be introduced as such to their Heads of Departments and Faculty Deans

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

# Open Hardware

**Delft Open Hardware** is a bottom-up community of students, researchers, university staff and alumni at TU Delft, started in September 2019. We believe that open source software and hardware are game changers in education, research and sustainability. This is why we work on open source hardware projects and run events where we share our expertise and passion with others.

## What is open source hardware?
Open (source) hardware means releasing publicly the source of how hardware is designed so that anyone can study, improve and distribute the technology. By doing so, everyone: engineers, developers, end-users and other stakeholders, are free to improve and decide how the projects evolve on the basis of innovative ideas,
excellent work and, intensive peer review for and quality assurance.

## What does Delft Open Hardware members do?
- Design and develop open hardware projects together, through sharing our ideas in meetups and our Telegram group.
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
