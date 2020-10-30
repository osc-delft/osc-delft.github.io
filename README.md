# Open Science Community Delft

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

In the sequel, we assume you use miniconda.

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

## Run the link checks

To avoid dead or wrong links, run the link checkers:

```
$ make check-html
```

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
