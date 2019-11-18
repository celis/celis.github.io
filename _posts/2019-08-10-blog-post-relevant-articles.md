---
title: 'Relevant articles'
date: 2019-11-18
permalink: /posts/2019/08/blog-post-relvant-articles/
tags:
  - representation learning
---

Recently, together with [Jose Eliel Camargo](https://github.com/JoseEliel) I have been exploring a very nice and simple idea.    When writing scientific articles, researchers put a lot of effort collecting relevant references and placing them within their text for different puposes: to give credit, to guide the reader to other points of view, to support some statement, etc.  This means that looking for papers which tend to be cited close to each other in a collection of scientific articles should provide a good way to extract a group of similar or relevant articles.  


With this in mind, we have extracted reference lists from [inspirehep](https://labs.inspirehep.net) using the
[inspirehep python wrapper](https://github.com/celis/inspirehep_api_wrapper).  Each reference list for us is just a list of inspire article ids.   We then trained a Skip-Gram model using the [gensim](https://radimrehurek.com/gensim/) library implementation.   We end up with a dense representation in the space of inspirehep article ids, from where we can extract similar items using cosine similarity.   Very simple!  

Lets look at some of the results, I will start with one of my favourites:












