---
layout: post
title: Natural Language Processing Pretraining
subtitle: From Dive into Deep Learning Book
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/nlp.jpeg
share-img: /assets/img/path.jpg
tags: [nlp, word2vec]
---

## Word Embedding (word2vec)

One-hot vectors: create a vector of all 0s with a length of N and set element i (index of a word in a dictionary) to 1.  

* Easy to construct.  
* Cannot accurately express the similarity between different words.  

Word embedding: map words to vectors of real numbers.

Word2vec comes up with to solve the problem above, contains two models: skip-gram & continuous bag of words (CBOW).  

### Skip-Gram model

A word can be used to generate the words that surround it in a text sequence.  

Example:  
Text sequence: "the", "man", "loves", "his", "son".  

The skip-gram model is concerned with:  

**P("the", "man", "his", "son" \| "loves")  
= P("the" \| "loves").P("man" \| "loves").P("his" \| "loves").P("son" \| "loves").**  

![Skip-gram](/assets/img/skip-gram.jpg)
