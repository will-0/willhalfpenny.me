---
layout: post
title:  "Book notes: 'Fundamentals of Data Engineering'"
date:   2025-01-12 19:00:00 -0000
---

## Why did I read this book?

My present interest is how we can make information accessible and interoperable across different systems. Within a large company, this is a task that would typically fall to individuals known as "data engineers". I was yet to read one resource that provided a comprehensive overview of the field, and this one had good reviews. 

It was read all in one go, on a Saturday night, when I was locked away at home due to an illness. I present my thoughts and digestions of it here.

## Overall Impression

This book was, as advertised, a broad overview of the field. It went through the problems, technologies and paradigms that a data engineer might face in the course of doing their job.

*The definition they use for data engineering is "the develpoment and implementation of processes that take in raw data and produce high-quality information for downstream use cases" (paraphrasing).*

## Takeaways

Here are the things I noticed about the perspective of the authors when reading this book.

1) Focus on the 'business problem'

One thing that frequently strikes me in books on engineering (`Clean Code` being another example), is that frequent mention of the business problem. Having come from an academic background, I typically expect problems to be phrased in terms of *technical* issues, such as an optimization challenge or a biomedical treatment. However, I like the approach presented here. Thinking purely of technical issues can cause wasted effort on problems that don't truly move the needle. Thinking about the ultimate 'business' utility would go a long way in the fields I've been exposed to. It's no stranger to someone working in the health tech space that engineers and computer scientists often try to build solutions to problems that weren't really there in the first place.

2) Technologies and details, rather than abstract concepts.

At the beginning of the book, the authors said they would try and focus on the general, non-changing aspects of data engineering. However, I nevertheless found that the authors focussed on specific details of the algorithms and computational paradigms, more than I would have hoped. This may be related to this specific book, or it may be that this is just more reflective of the day-to-day challenges of data engineers. I think the latter is very likely, given that the abstract understanding I'm searching for more relates to design of systems rather than implementation.

3) Data engineering is increasing in recognition

This is one that felt fairly obvious to me, but it was helpful to hear that experts in the space had noticed the same. They state at the beginning of the book that they are 'recovering data scientists', because they'd initially worked in that space but had then moved to data engineering once they'd seen the requirement for it. My perception is that a lot of the world of work has been like this: it's pretty much impossible to do good data science or machine learning research if the data hasn't been appropriately prepared for you.

4) Many of the goals laid out by the book were... pretty obvious.

Actually, this was one of the main takeaways from the book. There are extensive sections arguing the case for the importance of security, interoperability, observability, cost etc., but my main thought when reading them was: do I really need to read a book to tell me that these things are important? When we were designing data pipelines for research, or for startups, the fact that we should be designing for these goals was never hidden. Security was clearly vital, both for user trust and basic ethics. Observability was needed if we were going to detect errors. Cost is a primary metric of a business! I would rather have known core principles on *how* to achieve these things.

## Summary

Overall, I personally found that this book didn't quite satisfy either of the niches I'd want to look for. In my mind, I like to separate data engineering into two tasks: conceptual (involving semantic models and transformations) and implementation (performance, cloud implementations, etc.). This book sat a level above implementation, but didn't provide satisfactory insights on a conceptual level. I felt a mathematical or representational framework was missing.

Nevertheless, it remains a good book to have on the shelf for referencing some of the paradigms used when needing to solve a specific problem. Whilst I think that many of the problems are self-evident in practice, I will likely refer back to it to ensure I'm ticking the key boxes, next time I implement it.