# Open Science Community Delft
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-19-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

This is the online home of the Open Science Community Delft, officially launched on Sep 17, 2020.

The website is forked from the awesome [Open Life Science programme website](https://open-life-science.github.io) - the programme is led by 3 of the best people in the world, co-created by a beautiful community.

We're in the process of adapting this site for our community - please see below on how *you* can help out. We ask for your patience as we iron out all the glitches and stitches.

## Welcome!

This document (the `README` file) is a hub to give you some information about the
project. Jump straight to one of the sections below, or just scroll down to find
out more.

## Get involved

Please note that it's very important to us that we maintain a positive and
supportive environment for everyone who wants to participate. When you join us
we ask that you follow our [code of conduct](CODE_OF_CONDUCT.md) in all
interactions both on and offline.

## How can I generate the website locally?

You need a `ruby` environment (version >= 2.4). Either you have it installed and
you know how to install [Bundler](https://bundler.io/) and
[Jekyll](https://jekyllrb.com/) and then run Jekyll, or you use
(mini-)[conda](https://conda.io/docs/index.html), a package management system
that can install all these tools for you. You can install it by following the
instructions on this page: https://conda.io/docs/user-guide/install/index.html

### Using Miniconda on Linux/MacOS

1. Open a terminal
2. Clone this GitHub repository:

   ```
   $ git clone https://github.com/osc-delft/osc-delft.github.io.git
   ```

3. Navigate to the `osc-delft.github.io/` folder with `cd`
4. Set up the conda environment:

   ```
   $ make create-env
   ```

5. Install the project's dependencies:

   ```
   $ make install
   ```

6. Start the website:

   ```
   $ make serve
   ```

7. Open the website in your favorite browser at:
   [http://127.0.0.1:4000/](http://127.0.0.1:4000/)

#### Run the link checks

To avoid dead or wrong links, run the link checkers:

```
$ make check-html
```

### Using Ruby on Windows

We asume you have a working installation of [Git for Windows](https://git-scm.com/downloads)

1. Download and install the latest version of [Ruby+Devkit for Windows](https://rubyinstaller.org/downloads). Mind about a *32-bit*  or *64-bit*.   Keep all the default options. Put attention to where the location of the Ruby's root directory is located. For example, `C:\Ruby27-x64`

2. When the installation is done a *command prompt*  will pop up. Type `3` and press enter. This will install the Ruby's toolchain. When done, press enter once more.

3. Install `Jekyll` and `Bundler`. On the same *command prompt*  run:

   ```
   > gem install jekyll bundler
   ```

4. On the *Ruby command prompt*, use `git` to clone the repository.

   ```
   > git clone https://github.com/osc-delft/osc-delft.github.io.git
   ```

5. Got to the root of the repository and install the dependencies

   ```
   > cd ./osc-delft.github.io
   > bundle install
   ```

6. The previous command will install all dependencies except for the `libcurl` library. We will install the library manually. Donwnload [curl for Windows](https://curl.haxx.se/windows/), choose a version that fits your OS.

7. Unzip the file and look for the `libcurl.dll` file in the `.\bin` directory. If using the *64-bit version*, the file is called `libcurl-x64.dll`, remane the file to `libcurl.dll`

8. Copy the `libcurl.dll` file to the `\bin` folder in the Ruby's root directory. 

9. Compile and run the local server:

```
bundle exec jekyll serve
```

10. Open the website in your favorite browser at:
   [http://127.0.0.1:4000/](http://127.0.0.1:4000)

## Create a new blog post

To create a new blog post:

1. Create a file in the folder `_posts` with a file named following the pattern `yyyy-mm-dd-name.md`
2. Add some metadata on the top of the file

    ```
    ---
    layout: post
    title: <title of the post>
    author: <github id of the author>
    image: images/yyyy-mm-dd-name.jpg
    ---
    ```

4. Add content of the post in the file in Markdown
3. Add images in `images/posts/`

## Add someone as member

Add someone to the list of people:

1. Open the `_data/people.yaml` file
2. Create a new entry there (using Lastname-Firstname) following the alphabetical order
3. Fill in information using the tags:
  - `first-name` (*mandatory*)
  - `last-name` (*mandatory*)
  - `photo`
  - `position`
  - `faculty` (*mandatory*)
  - `department`
  - `twitter`
  - `email`
  - `website`
  - `gitter`
  - `orcid`
  - `linkedin`
  - `researchgate`
  - `expertise`
  - `motivation`

Add the person to their corresponding faculty list to be visible on the website, on `data/members-metadata.yaml`.

Add many people in a row to `_data/people.yaml`: (the following set of instruction is not up to date and needs amending)

1. Create a CSV file with at least the following columns (named this way):
   - `First name`
   - `Last name`
   - `Email`
   - `Twitter username`
   - `Website`
   - `ORCID`
   - `Affiliation`
   - `Country`
   - `Pronouns`
   - `Areas of expertise (1 element per line)`
   - `Bio`

   A form like [this one](https://docs.google.com/forms/d/e/1FAIpQLScmsWw0VSvdytz3A1k6HnbfgOnsE4SiJcL9_qkMTs_Na6-l2Q/viewform?usp=pp_url) can be used to generate such csv

2. Get a copy of the CSV file at the root of this folder
3. Activate the conda environment

   ```
   $ source activate osc-delft-website
   ```

   Or alternatively, get locally:
   - Python 3.*
   - pyyaml
   - pandas

4. Run the script which extract information from the CSV file and add them to `_data/people.yaml`

   ```
   $ python bin/extract-people.py -i <path to csv file>
   ```

## List a new event

The event calendar displayed is automatically generated from a file `_data/events.yaml`.

In this file, for each week, it is listed the timeframe and the different calls planned. For each call, several information are given:
title:

- `date-time`: string, e.g. `"December 1, 2020, 5-7pm"`
- `location`: string, e.g. `zoom`
- `content`: a short description of the event, markdown can be 20used
- `website`: a link to the event website

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://github.com/EstherPlomp"><img src="https://avatars1.githubusercontent.com/u/46314469?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Esther Plomp</b></sub></a><br /><a href="#question-EstherPlomp" title="Answering Questions">💬</a> <a href="#content-EstherPlomp" title="Content">🖋</a> <a href="#ideas-EstherPlomp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-EstherPlomp" title="Maintenance">🚧</a></td>
    <td align="center"><a href="https://github.com/Metahofzicht"><img src="https://avatars3.githubusercontent.com/u/70009155?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Meta Keijzer</b></sub></a><br /><a href="#data-Metahofzicht" title="Data">🔣</a></td>
    <td align="center"><a href="http://jurra.github.io"><img src="https://avatars1.githubusercontent.com/u/18581201?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jose Carlos Urra Llanusa</b></sub></a><br /><a href="#content-jurra" title="Content">🖋</a> <a href="#ideas-jurra" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/hrblyth"><img src="https://avatars3.githubusercontent.com/u/73690656?v=4?s=100" width="100px;" alt=""/><br /><sub><b>hrblyth</b></sub></a><br /><a href="#ideas-hrblyth" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="http://ashleycryan.me"><img src="https://avatars0.githubusercontent.com/u/70262847?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ashley Cryan</b></sub></a><br /><a href="#content-aecryan" title="Content">🖋</a> <a href="#ideas-aecryan" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/osc-delft/osc-delft.github.io/commits?author=aecryan" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/mwakok"><img src="https://avatars2.githubusercontent.com/u/15414938?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Maurits Kok</b></sub></a><br /><a href="#question-mwakok" title="Answering Questions">💬</a> <a href="#ideas-mwakok" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/osc-delft/osc-delft.github.io/issues?q=author%3Amwakok" title="Bug reports">🐛</a> <a href="https://github.com/osc-delft/osc-delft.github.io/commits?author=mwakok" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/ThorkellMoon"><img src="https://avatars0.githubusercontent.com/u/45631318?v=4?s=100" width="100px;" alt=""/><br /><sub><b>ThorkellMoon</b></sub></a><br /><a href="https://github.com/osc-delft/osc-delft.github.io/issues?q=author%3AThorkellMoon" title="Bug reports">🐛</a> <a href="https://github.com/osc-delft/osc-delft.github.io/commits?author=ThorkellMoon" title="Code">💻</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://junzis.com"><img src="https://avatars2.githubusercontent.com/u/9550577?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Junzi Sun</b></sub></a><br /><a href="#design-junzis" title="Design">🎨</a> <a href="#ideas-junzis" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/ebrahimifard"><img src="https://avatars2.githubusercontent.com/u/70349945?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Amir Fard</b></sub></a><br /><a href="#ideas-ebrahimifard" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/martateperek"><img src="https://avatars1.githubusercontent.com/u/10851024?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Marta Teperek</b></sub></a><br /><a href="https://github.com/osc-delft/osc-delft.github.io/issues?q=author%3Amartateperek" title="Bug reports">🐛</a> <a href="#blog-martateperek" title="Blogposts">📝</a></td>
    <td align="center"><a href="https://github.com/sebranchett"><img src="https://avatars0.githubusercontent.com/u/22983889?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Susan Branchett</b></sub></a><br /><a href="https://github.com/osc-delft/osc-delft.github.io/pulls?q=is%3Apr+reviewed-by%3Asebranchett" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/osc-delft/osc-delft.github.io/commits?author=sebranchett" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://garciageosmart.com/"><img src="https://avatars3.githubusercontent.com/u/8195424?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Manuel Garcia</b></sub></a><br /><a href="https://github.com/osc-delft/osc-delft.github.io/commits?author=manuGil" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/ConnieClare"><img src="https://avatars3.githubusercontent.com/u/72912958?v=4?s=100" width="100px;" alt=""/><br /><sub><b>ConnieClare</b></sub></a><br /><a href="#blog-ConnieClare" title="Blogposts">📝</a></td>
    <td align="center"><a href="https://github.com/yaseminturkyilmaz"><img src="https://avatars3.githubusercontent.com/u/45484225?v=4?s=100" width="100px;" alt=""/><br /><sub><b>yaseminturkyilmaz</b></sub></a><br /><a href="#ideas-yaseminturkyilmaz" title="Ideas, Planning, & Feedback">🤔</a> <a href="#blog-yaseminturkyilmaz" title="Blogposts">📝</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/santoshilam"><img src="https://avatars3.githubusercontent.com/u/49054107?v=4?s=100" width="100px;" alt=""/><br /><sub><b>santoshilam</b></sub></a><br /><a href="#ideas-santoshilam" title="Ideas, Planning, & Feedback">🤔</a> <a href="#blog-santoshilam" title="Blogposts">📝</a></td>
    <td align="center"><a href="https://github.com/niketagrawal"><img src="https://avatars1.githubusercontent.com/u/15953349?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Niket Agrawal</b></sub></a><br /><a href="#ideas-niketagrawal" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/emmyft"><img src="https://avatars1.githubusercontent.com/u/24935760?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Emmy Tsang</b></sub></a><br /><a href="https://github.com/osc-delft/osc-delft.github.io/commits?author=emmyft" title="Code">💻</a> <a href="#data-emmyft" title="Data">🔣</a> <a href="https://github.com/osc-delft/osc-delft.github.io/commits?author=emmyft" title="Documentation">📖</a> <a href="#eventOrganizing-emmyft" title="Event Organizing">📋</a> <a href="#ideas-emmyft" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-emmyft" title="Maintenance">🚧</a> <a href="#projectManagement-emmyft" title="Project Management">📆</a></td>
    <td align="center"><a href="http://damtp.cam.ac.uk/user/eglen"><img src="https://avatars.githubusercontent.com/u/1095067?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Stephen Eglen</b></sub></a><br /><a href="https://github.com/osc-delft/osc-delft.github.io/issues?q=author%3Asje30" title="Bug reports">🐛</a> <a href="https://github.com/osc-delft/osc-delft.github.io/commits?author=sje30" title="Documentation">📖</a></td>
    <td align="center"><a href="http://yo-yehudi.com"><img src="https://avatars.githubusercontent.com/u/9271438?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Yo Yehudi</b></sub></a><br /><a href="#ideas-yochannah" title="Ideas, Planning, & Feedback">🤔</a></td>
  </tr>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!

## Study notice

Please note that this repository is participating in a study into sustainability of open source projects. Data will be gathered about this repository for approximately the next 12 months, starting from May 2021.

Data collected will include number of contributors, number of PRs, time taken to close/merge these PRs, and issues closed.

For more information, please visit [our informational page](https://sustainable-open-science-and-software.github.io/) or download our [participant information sheet](https://sustainable-open-science-and-software.github.io/assets/PIS_sustainable_software.pdf)
