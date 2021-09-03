---
layout: post
title: "Research Code Review: Best practices, Challenges and Opportunities"
image: https://unsplash.com/photos/feXpdV001o4/download?force=true&w=1920
photo:
  name: Photo by Anas Alshanti on Unsplash
  url: https://unsplash.com/@anasalshanti
authors:
   - emmyft
youtubeId: KPSBNc8FNKM
---

*A recording and summary of our Open Science Coffee on Research Code Review.*

On Sep 1, we hosted our first **Open Science Coffee** - an informal community discussion on a shared open science topic of interest.

We discussed Research Code Review and are thrilled to host 3 experts who led the discussion:
- Anton Akhmerov: Associate Professor, Department of Quantum Nanoscience & Kavli Institute of Nanoscience, TU Delft
- Stephen Eglen: Professor of Computational Neuroscience, University of Cambridge & Co-Founder, CODECHECK
- Djura Smits: Research Software Engineer, Netherlands eScience Center

We're also very grateful for the 50+ participants from all around the world who joined and contributed to a very lively discussion.

Here we share a summary of our discussion and a recording of the session, for anyone who would like to learn more about this very interesting topic.

{% include youtubePlayer.html id=page.youtubeId %}

# What is code review, and why is this important?
There are different reasons why one would review code: in industry, it could be used to increase the maintainability of the code base; while working in a team, it can help knowledge transfer between team members. In academic research, there is no general agreement over what a "standard code review" process is: we know that code review can be done to help increase reproducibility and reusability of the code, and the process itself is a valuable learning opportunity for the code writers and reviewers to receive feedback and learn from others, to improve their coding skills. However, it could also simply be a process to check whether the code works- this "minimal" approach to code review helps make it as easy as possible for people to start participating in code review, slowly building towards a culture of sharing and contributing to each others' code.  

# What are the challenges of reviewing research code?
We still have a lot to do to ensure that data and code are shared with publications, let alone data and code review. We heard a case where editors refuse to accept code that was submitted alongside manuscripts for review; we still read the ominous "data available upon request". This is a lost opportunity, as code review can greatly improve the quality of the published work.

Another related challenge is the lack of time and resources. Peer review as it stands is largely powered by unpaid labour, and adding code review to that process is adding a huge amount of work to the already effortful process. On top of that, most code reviewers, many of whom are early career researchers, are doing this out of interest and on a voluntary basis.

Last but not least, the academic culture is currently not one that is open to admitting errors. This causes many to be hesitant to share their code, for the fear of it being imperfect or wrong. Most of us have to learn to mitigate our intrinsic defensiveness and accept criticism and feedback. Similarly, reviewers also need to learn to deliver constructive feedback.

## How do we move towards building a vibrant code reviewing culture?
A prerequisite of this is that code needs to be shared: within teams, in the submission process with manuscripts, and/or openly as open-source software. While we recognise that many are hesitant to share code because they don't want their competitors to get ahead of them (i.e. "scooping"), it can be very rewarding for others to reuse and build upon your work, and this also increases the impact of your research. Opening your code early in the development process allows others to offer feedback early and help improve the software.

Individually, we can make our code easier for others to understand and comment on, by following best practices: using version control, providing an overview of what different scripts do in a repository, sharing your thoughts on the code (e.g. "this part is new and I'm not sure about it"), etc. By participating in community events and initiatives like [CODECHECK](https://codecheck.org.uk), [Reprohack](https://reprohack.github.io/reprohack-hq/) and [the Turing Way](https://the-turing-way.netlify.app/welcome.html), you also have the opportunity to learn from and exchange ideas with a larger group.

Ultimately, making code review a norm in academia will take a cultural change. Concepts like "reproducibility" and "open science" often come across as far-fetched ideals that take a lot of time and altruistic efforts, while in fact, we should find selfish reasons and practical small steps to work reproducibly and participate in code review. For example, helping review someone else's code connects you with more colleagues in the field and gives you early access to the field's cutting edge work.

We've come a long way, but needless to say, we still have a long way to go. We should continue to discuss and experiment, and hopefully, soon, these insights will help us address questions like how we can scale code review and reward reviewers, and how we can incorporate research domain expertise in code review.

*Also read participant Lisa DeBruine's [live tweet thread](https://twitter.com/LisaDeBruine/status/1432978273554903043) of this session for audience comments and questions.*

*Join us for the next open science coffee on Diversity and Inclusion Research, Technology and Design - see our [Events page](https://osc-delft.github.io/events) for more details.*

## Useful links and resources
- [CODECHECK](https://codecheck.org.uk)
- [Reprohack](https://reprohack.github.io/reprohack-hq/)
- [The Turing way](https://the-turing-way.netlify.app/welcome.html)
  - In particular, [this chapter on reproducible computational environments](https://the-turing-way.netlify.app/reproducible-research/renv.html) provides practical and useful information on virtual machines, containers, and other relevant topics.
- [Five selfish reasons to work reproducibly, by Florian Markowetz](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-015-0850-7)
- [Announcement by Nature Human Behaviour about code reviewing](https://www.nature.com/articles/s41562-021-01190-w)
- [Anton's Twitter poll on code reviewing frequency](https://twitter.com/AkhmerovAnton/status/1429878810288304131)
- [Episode of the podcast FAIRly Open After Dark on Reproducibility](https://fairlyopenafterdark.podbean.com/e/repeat-after-me-1618326899/)
