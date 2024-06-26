---
layout: archive
title: "How Java Programmer Test Exceptional Behavior"
permalink: /msr21/
author_profile: true
---

{% include base_path %} 

2021 Mining Software Repositories Conference ([MSR 2021](https://2021.msrconf.org/track/msr-2021-technical-papers))

<img src="/images/msr21-first-page.png" width="480">

<i class="fas fa-fw fa-file-pdf" aria-hidden="true"></i> [Preprint](https://dvmarcilio.github.io/papers/msr2021.pdf)

<i class="fas fa-fw fa-copy" aria-hidden="true"></i> [Replication package including the tool, the dataset and all scripts used for the analysis](https://doi.org/10.6084/m9.figshare.13547561)

<i class="fas fa-fw fa-video" aria-hidden="true"></i> [4 minutes summary video](https://youtu.be/1vZRwgJnA8M)

<i class="fas fa-fw fa-images" aria-hidden="true"></i> [Slides](https://dvmarcilio.github.io/papers/MSR-presentation.pdf)

## Abstract

Exceptions often signal faulty or undesired behavior; hence, high-quality test suites should also target exceptional behavior. 
This paper is a large-scale study of _exceptional tests_—which exercise exceptional behavior—in 1 157 open-source Java projects hosted on GitHub.

We analyzed JUnit exceptional tests to understand what kinds of exceptions are more frequently tested, what coding patterns are used, and how features of a project, such as its size and number of contributors, correlate to the characteristics of its exceptional tests. 

We found that:

- exceptional tests are only 13% of all tests, but tend to be larger than other tests on average; 
- unchecked exceptions are tested twice as frequently as checked ones;
- 42% of all exceptional tests use try/catch blocks and usually are larger than those using other idioms; 
- and bigger projects with more contributors tend to have more exceptional tests written using different styles. 

The paper also zeroes in on several detailed examples involving some of the largest analyzed projects, which refine the empirical results with qualitative evidence. 
The study’s findings, and the capabilities ofthe tool we developed to analyze exceptional tests, suggest several implications for the practice of software development and for follow-up empirical studies.
