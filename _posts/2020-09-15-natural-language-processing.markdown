---
layout: default
title: Natural Language processing (NLP)
permalink: /natural-language-processing.html
categories: categorisation
---
TODO

### Definition

> "NLP enable machine to understand natural language. e.g. english, polish, french ..."

> "Natural Language Processing (NLP) and aims to tackle the task of teaching computers how to understand and use human language.[^1]"
> "Combining the process of Deep Learning and NLP enables a deeper understanding of language data for machines that gives more clarity about words and their relational meaning.[^1]"

NLP is tight with and uses 
   - **<a href="/sentence-boundary-disambiguation.html">SBD (Sentence boundary disambiguation)</a>** : identify the start and the end of sentense.
   - **<a href="/named-entity-recognition.html">NER (Named entity recognition)</a>** : finds named entities like people, locals, organizations, addresses ...
   - **<a href="/part-of-speech.html">POS (Part of speech) tagging</a> tag word like verbs, adjectives, nouns ...** (TODO penn tree bank)
   - **<a href="/lemmatization.html">Lemmatization</a> mapping word form that have a tense, gender mood... to the base form of the word (Lemma)** 
   - **<a href="/chunking.html">Chunking</a> dividing sentences into grammatically meaningful word groups.** 
   - **<a href="/language-detection.html">Language detection</a> needs training data file.** 
### Java libraries

- <a href="http://opennlp.apache.org">OpenNLP</a>
   - NER, SBD, POS, tokenization.
- <a href="https://stanfordnlp.github.io/CoreNLP/">Standford CoreNLP</a>


### Important links

<hr />

[^1]: https://onlim.com/en/how-do-machines-learn-to-understand-natural-language/