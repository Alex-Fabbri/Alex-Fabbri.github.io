---
layout: posts
title: "TutorialBank: Learning NLP Made Easier"
author: Alex Fabbri
author_profile: true
use_math: true
draft: true
---

# Introduction 

Welcome! If you've made it here, you are probably interested in Natural Language Processing \(NLP\) or a related field \(even if you're not, keep reading!\). NLP is rapidly growing, and, as a result, advancing in the field can seem daunting to the student or the researcher. To help the growing NLP community and advance research related to NLP for educational applications, we introduced a new corpus in our paper "[TutorialBank: Using a Manually-Collected Corpus for Prerequisite Chains, Survey Extraction and Resource Recommendation]()" by Alexander Fabbri, Irene Li, Prawat Trairatvorakul, Yijiao He, Weitai Ting, Robert Tung, Caitlin Westerfield and Dragomir Radev
 [LILY, YALE](https://yale-lily.github.io/)."


header: 
  image: https://commons.wikimedia.org/wiki/File:Test_card.png
# What is TutorialBank?

TutorialBank is a manually collected dataset of over 5,600 resources on NLP as well as the related fields of Artificial Intelligence (AI), Machine Learning (ML) and Information Retrieval (IR). Over a few years we hand-picked high-quality resources related to these areas. These include surveys, tutorials, libraries, codebases, among others. We feel that students learn a lot from reading tutorials in addition to academic papers, so we focus on resources other than papers. For each resource, we populate our database with meta-data such as the type of resource (pedagogical function as stated in the paper) and categorize each one according to our own taxonomy of over 300 topics. Here are some of the topics:

<br> 

| ![]({{ "/assets/imgs/taxonomy.png" | absolute_url }}){:height="800px" width="800px"} | 
|:--:| 
| *The top level of the TutorialBank taxonomy* |

<br> 

Very easily! We created [a search engine](http://tangra.cs.yale.edu/newaan/) which we call "All About NLP" (AAN) and which you can use to quickly search our corpus ([Access the corpus](https://github.com/Yale-LILY/TutorialBank)).  The acronym AAN may be known to you from the ACL Anthology Network Corpus introduced [here](http://clair.si.umich.edu/~radev/papers/aan09.pdf) and [here](http://clair.si.umich.edu/~radev/papers/aan_lre.pdf), which itself builds upon the [ACL Anthology Reference Corpus](http://clair.si.umich.edu/~radev/papers/lrec08.pdf). We host the ACL Anthology Network Corpus on our site and our search engine allows you to search over 24,000 papers. Additionally, as stated above, our corpus focuses on tutorials and resources other than the academic papers from the above corpora. You can explore our taxonomy and pick the type of resource you are looking for by clicking "Browse Resources by Topic:"


<br> 

| ![]({{ "/assets/imgs/search_resources.png" | absolute_url }}) | 
|:--:| 
| *In the mood to learn about Deep Learning? Look at all the resources we have for you!* |

<br> 

or you can just search for specific terms by clicking "Search Resources" as shown below: 


<br> 

| ![]({{ "/assets/imgs/search_cnn.png" | absolute_url }})| 
|:--:| 
| *I wish I had this resource before I did my homework on CNNs...* |

<br> 

# Is there more? 

Yes! While the collection of all these resources in a search engine is great in and of itself, we annotated our corpus to make it more useful for both the student and the researcher. Additionally, we created a simple command-line tool (available along with the corpus) to make our annotations more accessible, as described below. 

## Survey Topics, Reading Lists and Prerequisite Chains
We created a list of 200 topics for which we felt a survey of the topic would benefit students. As stated in the paper, these topics differ from the taxonomy topics, since we do not want our survey topics to be too broad or fine-grained. For each topic, annotators created reading lists of up to 5 resources on the topic. We then split up resources from these lits into content cards and abeled the cards as useful or not for learning the topic at hand. This is important since often resources are on a more general topic and only partly cover the topic you want to learn about. 

What if you don't know which topic to start with? To address this question, we annotated which topics are prerequisites of which other topics; which topics should you learn to better understand a given topic. A subsection of our graph is shown below:


<br> 

| ![]({{ "/assets/imgs/prerequisites.png" | absolute_url }}){:height="800px" width="800px"}  | 
|:--:| 
| *Time to brush up! Where did I leave Gilbert Strang's book?* |

<br> 

## Accessing our annotations
That sounds like a mouthful to go through. Luckily for you, we created a command-line tool to make our annotations easily accessible:

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


# How can I use this for research? 
Our annotations for resource type and topic categorization promote research in text classification and topic modeling while we hope our annotated reading lists and survey extraction annotations will promote information retrieval for scientific topics. Finally, our extensive prerequisite chain annotations can be used for learning concept dependencies in a supervised/semi-supervised manner. 


# What can I expect in the future? 

In the future we are planning to expand our taxonomy and corpus. We are also going to add new features to our site, and so we greatly appreciate any feedback you may have. Feel free to email me or send a message under "Contact" on our site. Additionally, we are planning to refine our annotation and explore more deeply the research areas of prerequisite chains, resource recommendation and survey extraction.  
