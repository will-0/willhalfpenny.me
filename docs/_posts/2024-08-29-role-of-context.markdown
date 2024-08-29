---
layout: post
title:  "The Role of Context in Data and Communication"
date:   2024-05-23 21:00:00 +0100
---

## Introduction

I'm currently on a deep dive into the various ways humans knowledge, in a hope that it will inform how we can find methods to connect these representations up. The topic of today is an attempt to understand the importance of context in information representations, motivated by the research and engineering topic of [document AI](https://arxiv.org/abs/2111.08609).

## What is the role of context in language?

Context in language provides many uses. It is necessary for several aspects of language comprehension:
-	Word disambiguation (e.g. bank vs bank)
-	Allows efficient representation of information (encoding/compression)
    - This is both quicker and reduces cognitive load.
    - This can equivalently be thought of as ‘ensuring the correct message is conveyed’ i.e. if you give the same message without context it could be misinterpreted.

Context is also helpful for other reasons in language, such as the following, although we are less interested in these:
-	Allows listener to filter out irrelevant information
-	Several human-factors roles (e.g. instigating the end of a party without offending)
-	Facilitate unspoken inferences to be made faster.

## What is the role of context in data?

I would argue that the main role of context in data representation is that it allows more efficient communication of information. 
We are likely familiar with the frame of reference that data without context can be meaningless. Take the following sequence of bits as an example: 10100000 00011100. Without context, this is useless. However, if you’re told a) this is an I2C packet, b) it’s from glucose sensor peripheral, and c) the units are mmol/L (and integer), this is very significant meaning indeed (alarm bells for diabetic ketoacidosis!).

However, I would argue there’s an alternative frame through which to view this. Realistically, no one bothers to record data without someone being able to ascribe meaning to it, even if it’s only the author and only temporarily. By combining data with context, we are instead able to reduce its cognitive and storage burden.

