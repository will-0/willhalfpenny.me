---
layout: post
title:  "Introduction to LinkML"
date:   2025-01-27 15:00:00 +0000
---

Whilst trying to build an [open-source data model for NHS pay](https://github.com/finomics-ltd/nhs-pay-ontology), I was stumped that there wasn't a good modelling language that could serialize into all the other common formats (JSON-schema, DDL, Pydantic, OWL, etc) that developers use. If I was going to write a general-purpose, interoperable framework, would I really have to make the choice for the downstream developer about which technology to use?

Turns out, there was such a modelling language, and I'm super excited about it! Enter, [LinkML](https://linkml.io/).

## [LinkML](https://linkml.io/) features

LinkML describes itself as a "a general purpose modeling language that can be used with linked data, JSON, and other formalisms". The thing that's *really* cool about it, is that it provides generators for compiling this data model to other frameworks.

I will not walk through how it works, or how to use it. I'll instead leave that to the excellent [documentation](https://linkml.io/linkml/index.html). What I will do, however, is highlight the core features I love about it.

### Model once, validate everywhere

One of the first exercises in the documentation walks you through creation of a simple data model, and allows you to validate arbitrary data formats. You can write a model in YAML, and validate an object instance that's defined in JSON, with ease.

### Easy transformations

In the same step (within ~1 minute's worth of reading) you've already got to the next feature, where you can translate a object in one format (e.g. JSON) into another (e.g. RDF Turtle), with a single command. 

It brought a tear to my eye.

### Visualization

Data visualization is, to me, a very important part of data modelling. As well as making it easier to communicate with domain experts (who may not be comfortable reading markup), it think it is a good cognitive aid in getting to grips with what we've built.

LinkML allows you to easily create UML diagrams from a data model, such as the one below:

![Image: Example UML diagram](/assets/posts/20250127/example_uml.png)

### Semantic markup

The final thing which I think is super exciting, is that LinkML provides you with the ability to back up your schema with semantic annotations. As mentioned [here](https://linkml.io/linkml/schemas/uris-and-mappings.html), all the elements of your schema (i.e. class and slot definitions) have a globally unique IRI/URI. This is either explicitly defined in the model, or implicity, using the default prefix.

The benefit of doing this may not be familiar to all readers, but it is significant in the semantic web and interoperability communities. To quickly summarize my view of it, URIs are just a way to *uniquely* label an arbitrary (or 'resource'). [This article](https://www.cogsci.ed.ac.uk/~ht/WhatAreURIs/) talks about it a bit more. It can be a bit meta, but it is pretty useful if you want to do entity resolution between databases, and it's great to have it as an option when defining a data model.

## Conclusion

Once again, it seems the biology community is crushing it with respect to developing data modelling and interoperability tools. I'm excited to be using LinkML in my projects, and imagine it will be a tool I stick with for a while.