---
layout: archive
title: "How Java Programmer Test Exceptional Behavior"
permalink: /msr21/
author_profile: true
---

{% include base_path %} 


<center><img src="/images/msr21-first-page.png" width="480"></center>

<i class="fas fa-fw fa-file-pdf" aria-hidden="true"></i> [Please check the preprint here.](https://dvmarcilio.github.io/papers/msr2021.pdf)

<i class="fas fa-fw fa-video" aria-hidden="true"></i> [This paper has a quick 4 minutes summary video available here.]()

## Abstract

Exceptions often signal faulty or undesired behavior; hence, high-quality test suites should also target exceptional behavior. 
This paper is a large-scale study of _exceptional tests_—which exercise exceptional behavior—in 1 157 open-source Java projects hosted on GitHub.

We analyzed JUnit exceptional tests to understand what kinds of exceptions are more frequently tested, what coding patterns are used, and how features of a project, such as its size and number of contributors, correlate to the characteristics of its exceptional tests. 

We found that:

- exceptional tests are only 13% of all tests, but tend to be larger than other tests on average; 
- unchecked exceptions are tested twice as frequently as checked ones;
- 42% of all exceptional tests usetry/catch blocks and usually are larger than those using other idioms; 
- and bigger projects with more contributors tend to havemore exceptional tests written using different styles. 

The paper also zeroes in on several detailed examples involving some of the largest analyzed projects, which refine the empirical results with qualitative evidence. 
The study’s findings, and the capabilities ofthe tool we developed to analyze exceptional tests, suggest several implications for the practice of software development and for follow-up empirical studies.

## Replication Package

A replication package including the tool, the dataset and all scripts used for the analysis is [available on figshare](https://doi.org/10.6084/m9.figshare.13547561).

## Top-17 Tested Exceptions

1. java.lang.IllegalArgumentException
1. java.lang.Exception
1. java.lang.UnsupportedOperationException
1. java.lang.NullPointerException
1. java.lang.Throwable
1. java.lang.IllegalStateException
1. java.io.IOException
1. java.lang.AssertionError
1. java.lang.IndexOutOfBoundsException
1. java.lang.RuntimeException
1. java.lang.InterruptedException
1. java.util.NoSuchElementException
1. java.sql.SQLException
1. java.util.concurrent.ExecutionException
1. java.lang.ClassCastException
1. java.lang.ArithmeticException
1. java.lang.NumberFormatException
