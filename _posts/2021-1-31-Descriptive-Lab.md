---
layout: post
title: Descriptive Lab
subtitle: 3.5
tags: [lab]
comments: true
---

## Introduction

I analyzed data from the results from a [a survey]() done on people who learned to code within the past 5 years. I looked at the relationship between taking a coding boot camp, educational major, and expected earning. I found that in all four majors I studied, people who attended coding boot camps expected to make more money on average than their collegues who did attend boot camps.

## Study

I chose to study four majors, all having a rather large sample size in comparison to the majors that were not studied as to maximize the likelihood that the data I am analyzing is reflective of the population. I chose two majors wherein a knowledge of coding would likely carry immediate utility to the majors' field (computer science and economics) and two with less immediate coding applications to their field (psychology and English).

## Findings

I produced the following violin plot:

https://jacobshaw41.github.io/jacob-shaw.github.io/assets/img/Figure_1.png

It shows that, for all majors, people who took a coding boot camp expect to make nontrivially more than people who did not. For instance, the mean expected earning for English majors who did not attend a boot camp was 55832.36, whereas that of English majors who did attend a bootcamp was $67125.00. It also seems that the data was more spread out among English majors who did attend boot camp (σ: 31220.128 than those who did not (σ = 17085.32).

One should also note the massive spread in computer science expected salaries (min = $6000, max = $800000, σ = 60132.40). This is because there is a small group of people in the larger dataset who expect to make the most (falling into the 99th percentile). This can be seen in the violin plot. These outliers are not necessarily inaccurate, especially in a field like computer science, wherein the range of salaries between jobs—for instance, hobby coders working for small start-ups and senior executives at companies like Apple and Google—is immense.

It is important to keep in mind that while this points to correlation, it does not say anything definitive about causation. That is to say, this data only demonstrates a relationship between variables. It could very well be true, for instance, that the people who expect to make more money already have financial means to be able to sign up for coding boot camps. It's also possible that coding opens new doors across disciplines. Without running a more studies—specifically longterm or more detailed studies that seek to directly study the reasons why this relationship is observed, researchers can only guess at any origins of this correlation. Attention should also be given to the specifics of this survey. Not only was the whole study optional, leading the data to only reflect the people who happen to find the survey and decided to take it, but each question was optional. This might lead to unwanted trends in the represenation of respondants for each question. There is also no way of verifying any of the information, and I have reason to believe that at least some of the data is inaccurate—for instance, a 16-year-old "self-employed" high school student who expected to make $1,000,000 after coding for 2 years.

## Code

My code was relatively straightforward. I took the data from a CSV (comma separated values), converted it into a dataframe (using Pandas), and filtered the data. Then I took the data and produced a violin graph as to display the center as well as the variability of the data.

## Muffin Recipe

[Today's recipe](https://www.tasteofhome.com/recipes/peanut-butter-banana-muffins/) is a treat—peanut butter-banana muffins? Say less.

_Tsufridenem bakn!_
