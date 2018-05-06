---
layout: posts
title: "TutorialBank: Learn NLP More Easily"
tags: [test]
author: Alex Fabbri
author_profile: true
use_math: true
draft: true
---

# Introduction 
testsetsts
branch name
test231413241
test

Welcome! If you've made it here, you are probably interested in Natural Language Processing \(NLP\) or a related field \(even if you're not, keep reading!\). NLP is rapidly growing, and as a result, advancing in the field can seem daunting to the student or the researcher. To help the growing NLP community and advance research related to NLP for educational applications, we introduced a new corpus in our paper "TutorialBank: Using a Manually-Collected Corpus for Prerequisite Chains, Survey Extraction and Resource Recommendation."

# What is TutorialBank?

TutorialBank is a manually collected dataset of over 5,600 resources on NLP as well as the related fields of Artificial Intelligence (AI), Machine Learning (ML) and Information Retrieval (IR). Over a few years we hand-picked high-quality resources related to these areas. These include tutorials, libraries, codebases, among others. We feel that students learn a lot from reading tutorials in addition to academic papers, so we focus on resources other than papers. For each resource, we populate our database with meta-data such as the type of resource (pedagogical function as stated in the paper) and categorize each one according to our own taxonomy of over 300 topics. 

# How can I use TutorialBank? 

Very easily! We created [a search engine](http://tangra.cs.yale.edu/newaan/) which we call "All About NLP" (AAN) and which you can use to easily search our corpus ([Access the corpus](https://github.com/Yale-LILY/TutorialBank)).  Our site also hosts the ACL Anthology Network Corpus and allows you to search over 24,000 papers. You can explore our taxonomy and pick the type of resource you are looking for by clicking "Browse Resources by Topic:"


<br> 

| ![]({{ "/assets/imgs/search_resources.png" | absolute_url }}){:height="800px" width="800px"} | 
|:--:| 
| *In the mood to learn about Deep Learning? Look at all the resources we have for you!* |

<br> 

or you can just search for specific terms by clicking "Search Resources" as shown below: 


<br> 

| ![]({{ "/assets/imgs/search_lstm.png" | absolute_url }}){:height="800px" width="800px"}| 
|:--:| 
| *I wish I had this resource before I did my homework on LSTMs...* |

<br> 

# Is there more? 

Yes! While the collection of all these resources in a search engine is great in and of itself, we did annotation to make our corpus more useful for both the student and the researcher. Additionally, we created a simple command-line tool to make our annotations easily accessible, as described below. 

## Survey Topics and Reading Lists
We created a list of 200 topics for which we felt surveys or overviews would be useful and created short reading lists for each topic. What if you don't know which topic to start with? To deal with these, we annotated which topics are prerequisites of which other topics; which topics should you learn to better understand a given topic. Finally, we split up resources for these 200 topics into content cards and then labeled the cards as useful or not for learning the topic at hand. This is important since often resources are on a more general topic and only partly cover the topic you want to learn about. 

### Accessing our annotations
That sounds like a mouthful to go through. Luckily for you, we create a command-line tool to make our annotations more accessible through an interface:


<br> 

| ![]({{ "/assets/imgs/interface.png" | absolute_url }}){:height="800px" width="800px"}  | 
|:--:| 
| *Try out some of the options from our interface!* |

<br> 

<br> 

| ![]({{ "/assets/imgs/nmt.png" | absolute_url }}){:height="800px" width="800px"} | 
|:--:| 
| *Get a reading list for any of the annotated topics* |

<br> 


# Can I use this for research too? 
Of course! Our annotations for resource type, reading lists and topic categorization can be used for experiments in text classification, resource recommendation systems and topic modeling. Our extensive prerequisite chain annotations can be used for learning concept dependencies, while we hope that our annotations for survey extraction will promote information retrieval for scientific topics. 


# What can I expect in the future? 

In the future we are planning to expand our taxonomy and corpus. We are also going to add new features to our site, and so we greatly appreciate any feedback you may have. Feel free to email me or send a message under "Contact" on our site. Additionally, we are planning to refine our annotation and explore more deeply the areas of prerequisite chains, resource recommendation and survey extraction.  


# References
