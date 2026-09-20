---
layout: without-toc
title: Designing and Prototyping a Website for the Zoological Society of London’s Biobank
---

# Designing and Prototyping a Website for the Zoological Society of London’s Biobank

While studying abroad in London, I helped to develop a searchable web catalog for a 
wildlife biobank operated by the [Zoological Society of London](https://www.zsl.org/)
(ZSL). This page gives some background about the project and gives details about the
website design process.

## Background

### What is ZSL?

The Zoological Society of London (ZSL) is a science-driven conservation charity dedicated
to restoring wildlife, both in the UK and globally, through scientific research, field
conservation, and public engagement. They are known for operating two zoos in the UK, the
[London Zoo](https://www.londonzoo.org/) and the [Whipsnade Zoo](https://www.whipsnadezoo.org/). 
What they are less known for is their wildlife biobank, which is a large collection of 
biological specimens that are grouped into 4 categories: dry, frozen, wet, and slides. The
dry and frozen collections where the focus of our research. The dry collection contains
specimens like bones, skulls, pelts, and taxidermies, and the frozen collection contains
preserved tissue samples.

### What is an IQP?

At [WPI](https://www.wpi.edu/), all students partake in three major projects throughout
there academic journey. One is in the topic of Humanities (HUA), one in Social Science 
(IQP), and one in the topic of the student's major (MQP). The 
[Interactive Qualifying Project](https://www.wpi.edu/project-based-learning/project-based-education/interactive-qualifying-project)
(IQP) is designed to give students an out-of-classroom experience that has real-world
impact and is usually done in small teams of students with mixed majors. Most students 
choose to do their IQP at one of many 
[project centers](https://www.wpi.edu/project-based-learning/project-based-education/global-project-program/project-centers)
located around the globe where they volunteer for a local organization.

## About the project

My project was to develop a searchable web catalog for the ZSL wildlife biobank so that
users could browse the collections and make loan requests.

Instead of making assumptions about how the website would be used, my team worked 
closely with stakeholders and end-users to understand their needs. We spent several weeks
administering a survey to prospective users and conducting follow-up interviews to learn
more about what collections people would be interested, what they plan on using the
specimens for (e.g., research, educational events, etc.), and what their experience has
been like borrowing specimens from other biobanks.

### Translating survey results into website design

The most interesting part of the project to me was figuring out how to design our website
based on the results from our data collection. Below are a few examples of how we
translated our findings into concrete design decisions.

Our user survey revealed who might use the biobank website as well as their expected usage 
habits. We found that there were two primary groups of users, researchers and educators, 
and that researchers were more interested in the frozen collection, presumably due to 
their focus on DNA sampling, while educators were more interested in the dry collection,
since they often wanted nice-looking items to display or use as props at their
educational events (see figure below).

![Collection interest by type](/assets/images/biobank/collection-interest-by-user-type-captioned.png)

Since these two groups would only be interested in one of the collections at a time, it
made sense to only allow users filter search results to just one of the collections. It is
for this reason that there are tabs on the search page limiting search results to only the
selected collection (see image below). 

![Search page tabs](/assets/images/biobank/search-page-tabs.png?v=2)

Another element of the search page that is influenced by findings is the ordering of
search filters. The ordering mirrors how important each attribute is to the users, with
the most important ones near the top.

![Search page filter ordering](/assets/images/biobank/search-page-filters.png)

When it came to displaying search results, there are different ways we chose to display
items in the dry collection vs the frozen collection. You may notice that in the bar chart
above, for Has images, there is much higher interest with the dry collection than with the
frozen collection (this makes sense since people who are interested in the dry collection
often want specimens for visual/display purposes). For this reason, we chose to display
specimens in a style that mimics an e-commerce shopping website with nice big images on
each item listings.

![Dry collection search results](/assets/images/biobank/dry-search-results.png)

For the frozen collection, we chose to use a different display style. Instead of item
cards with big images, we chose to use a list format that displays more information about
the specimen upfront. From a data perspective, this also makes more sense since the images
for frozen collection specimen would all be just some generic test tube. Additionally, the
frozen collection search results are grouped by specimen type since there can be multiple
specimens of the same type. This makes the search results less overwhelming to navigate.

![Frozen collection search results](/assets/images/biobank/frozen-search-results.png)

The search page was obviously a big focus for my team with this website, and it is where we
incorporated most of our survey findings. Besides the search page, we have made a few other
pages that are typically found on a website like this just to make it a complete package.

![General website pages](/assets/images/biobank/general-website-pages.png)

### Takeaways

This project exposed me to the less technical side of software engineering, and the skills
and methods I learned will definitely stick with me. I am grateful to have had the
opportunity to work on this project, and I'm thankful to my advisors 
[Dominic Golding](https://www.wpi.edu/people/faculty/golding) and
[Laureen Elgert](https://www.wpi.edu/people/faculty/lelgert) for there help throughout the
project, and also to the 
[ZSL biobank team](https://www.zsl.org/what-we-do/science-research/zsl-biobank) for making
me and my team feel welcome.

