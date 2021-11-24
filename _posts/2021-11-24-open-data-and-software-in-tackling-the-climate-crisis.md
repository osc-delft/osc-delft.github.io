---
layout: post
title: "Open Data and Software in Tackling the Climate Crisis"
image: https://unsplash.com/photos/RN14PbITnnM/download?ixid=MnwxMjA3fDB8MXxzZWFyY2h8Nnx8Y2xpbWF0ZXx8MHx8fHwxNjM3NzQ4Njcw&force=true&w=1920
photo:
  name: Photo by Markus Spiske on Unpslash
  url: https://unsplash.com/@markusspiske
authors:
   - Emmy Tsang
youtubeId: HUiEADH686o
---

*A recording and summary of our Open Science Coffee on Open Data and Software in Tackling the Climate Crisis.*

As part of the Dutch National Climate Week, we hosted an informal online discussion on "Open Data and Software in Tackling the Climate Crisis" on November 5. Over 40 members of our community and beyond joined and contributed to the conversation.  

We were particularly grateful to our three panellists for sharing their experience and perspectives on the topic:
- Nick van de Giesen, Full Professor, Faculty of Civil Engineering and Geoscience, TU Delft
- Maarten Plieger, Senior Software Engineer, KNMI
- Diána Szász, Programme Lead - Data Ecosystems and Innovation, Open Data Institute

Here we share a summary of our discussion and a recording of the multifaceted debate.

{% include youtubePlayer.html id=page.youtubeId %}

# What are some of the challenges associated with working with climate data?
Although not unique to climate data, data heterogeneity is a well-recognised challenge when working with climate data: datasets come from different sources and often have diverse formats. This makes working with climate data challenging, as one needs to understand what the data is for, how it is collected, what it contains, and its limitations.

At the same time, the amount of data is growing, as climate models generate more and more data (now in petabyte ranges). Downloading and working with this data becomes problematic because it requires robust network infrastructure and intensive computing power.

Moreover, fragmentation hampers discoverability. Data is collected and stored in various places, making it hard to not only find, but also work with multiple relevant datasets.

Last but not least, there are costs associated with storing large amounts of data. Storage costs are surpassing compute resources as the bottleneck for working with big sets of climate data and models. This poses a challenge for the sustainability of the current climate data ecosystem. There are some innovations in this area, such as climate data marketplaces and freemium models, but this remains a concern for those working with climate data and research.

## What does "open" mean for climate data?

Diana shared the Open Data Institute's definition for open data: data that everyone can access, use and share. This involves ensuring that the datasets are shared with appropriate open licenses, which define how the dataset can be reused, and with good documentation.

However, considering the challenges above, ensuring that "everyone can access, use and share" a dataset goes beyond just putting the dataset online. For others to access a dataset, the dataset needs to be findable and/or citable; and to use a petabytes-large dataset effectively, users need to be able to bring their code and analysis workflows to where the data is. Maarten also highlighted the need to have visualisation tools for users to quickly understand what the dataset contains and what one can do with it.

Open data and code are particularly crucial for improving the reproducibility of climate research. Nick pointed out that while many publish some results from climate models, it is often difficult to check the robustness of these results because the underlying code is not accessible. Technological solutions like containerisation are helping improve reproducibility by capturing not only the code used for producing results, but also the environment parameters and variables.

# What would the ideal climate data ecosystem look like in 10 years time?

Diana envisioned a data ecosystem that supports the needed changes to transition to a low carbon and climate resilient society. It should be able to cater to diverse data user needs, and this also means not opening some data, e.g. personal data, or data that can pose risks to national security. The ideal data ecosystem should also be trustworthy: one where there is transparency and clarity around what various data are used for, and where data are used in a way that builds towards tangible benefits for the society.

Maarten shared recent efforts to develop environmentally sustainable climate data centres. As more compute and storage is required, it is crucial that we scrutinise the carbon footprint of our climate research infrastructure and work towards environmental sustainability.

From his extensive experience researching in Africa, Nick wished to see a well-organised, well-funded data collection system on the ground worldwide. Having ground data with good coverage and resolution is very valuable in increasing the accuracy of climate models.

# What practical steps can researchers take towards fostering a more healthy, vibrant climate data ecosystem?

Sharing data and allowing others to understand and use it increases the impact of researchers' work. Researchers can learn more about data publishing and licensing to know how to best share their data - there are guides and online resources that can help (see "Useful links and resources" below for some examples). Universities also often have dedicated support (e.g. data stewards) that can provide advice and guidance. Having good data descriptions and documentation makes a huge difference to help others understand how they can work with and make the most out of the data shared.

There is also a need for more technological innovation, especially discovery mechanisms (e.g. search tools) for data, and for more social innovation, e.g. to incentivise researchers to increase the reusability of their data.

*The 2021 series of Delft Open Science Coffee has now concluded - we'd like to thank everyone who attended and contributed. We are currently evaluating where we have done well and what could be improved, and we would appreciate your feedback! Please leave your comments in this [GitHub issue](https://github.com/osc-delft/ideas-and-plans/issues/7), or email community coordinator Emmy at f [dot] tsang [at] tudelft [dot] nl.*

## Useful links and resources
- [TAHMO](https://tahmo.org/)
- [eWaterCycle](https://www.ewatercycle.org/)
- [ADAGUC](https://adaguc.knmi.nl/)
- [The Open Data Institute](https://theodi.org)
- [Accelerating progress on tackling the climate crisis through data collaboration](https://theodi.org/article/accelerating-progress-on-tackling-the-climate-crisis-through-data-collaboration/)
- [Tackling the climate crisis with data: what the built environment sector can do?](https://theodi.org/article/tackling-the-climate-crisis-with-data-what-the-built-environment-sector-can-do/?ff)
- [4TU.ResearchData](https://data.4tu.nl/)
- [netCDF and OPeNDAP](https://data.4tu.nl/info/en/about-your-data/netcdf-and-opendap)
- [The data spectrum - ODI](https://theodi.org/about-the-odi/the-data-spectrum/)
- [Sustainability of data access - ODI](https://theodi.org/project/rd-sustainable-data-access/)
- [Systematic Observations Financing Facility](https://alliancehydromet.org/systematic-observations-financing-facility/)
- [Publishing Open Data  in times of crisis](https://theodi.org/article/publishing-open-data-in-times-of-crisis/)
- [Guide to open data licensing](https://theodi.org/article/publishers-guide-to-open-data-licensing/)
- [World Community Grid](https://www.worldcommunitygrid.org/)
