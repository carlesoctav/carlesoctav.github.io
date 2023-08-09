---
title: "My Attempt at Blogging"
date: "2023-07-12"
categories: [Learning]
author: "Carles Octavianus"
toc: true
draft: true
---

# Semantic Search / Vector Search Dengan Transformers, a future of search engine?

## Introduction

when participating bangkit 2023, my friend and I got a chance to do company proposed capstone project (it's a project that proposed by some tech company in indonesia). we got dicoding indonesia cases, to improve discussion forum.

after a glimpse look on dicoding discussion forum, what's i feel lack in that forum are the search bar, and a proper aiding to tagging their discussion (there's just a user-based tagged, no rules).
koko
for the search engine, you need a proper match of an word /sentence for the search to able find a relevant document, not even a fuzzy search. also it's only search on title not on the body (discussion). i would say, it was a  nightmare to search as if, it's more possible to get answer with just adding new discussion (since there's a assistant that probably will answer your question ) even tho it's a duplicate.

so, for the past month (may to june) we have been researching on how we can improve search using machine learning (since it's a must as it's bangkit 2023 progam (machine learning path)) and also how to create an auto-tagger to aiding new user to properly tagging their newly disucssion.

I and some of my friend do work on search thingy while other do work on auto-tagger. for those who want to see all the research and finally what we have to decided to use, you guys can take a look github  [C23-DF01-Dicoding-Indonesia](https://github.com/orgs/C23-DF01-Dicoding-Indonesia/repositories) (it's not well documented so you will need to explore yourself). also, the model are aviailable on [huggingface](https://huggingface.co/carlesoctav/indo-sentence-bert-KD) which you can easily use it.

## preview what we have achive.

here's some example of model capability, to find a relevant document :D.

you guys can try it yourself on this notebook,





## Text ranking problem

let's define the problem more formally or mathematically.

>Given an information need expressed as a query $q$, the text ranking task is to return a ranked list of $k$ texts $\left\{d_1, d_2 \ldots d_k\right\}$ from an arbitrarily large but finite collection of texts $\mathcal{C}=\left\{d_i\right\}$ that maximizes a metric of interest, for example, nDCG, AP, etc.

so it's just a matter of re-ranking a list of document based on a query, that satisfy some metric.




## Before machine learning era


## Learning to Rank era


## Deep learning era, the two approaches

as a Deep learning more and more feasible and popular to use to solve a machine learning problem, also someone has been using it to solve text ranking problem. in general, deep learning approach more end to end approach, without hand-crafted feature. so, it's more flexible and can be applied to any language.



## Representation-based, a bit unrealibale but it's fast


## a way to train the model


## multilingual cases


## how we decided to train the model


##








