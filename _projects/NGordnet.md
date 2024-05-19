---
layout: page
title: NGordnet - Exploring Word Usage History
description: A browser-based tool for analyzing the history of word usage in English texts.
importance: 3
category: School Projects
related_publications: false
---

### Overview

The [NGordnet project](https://fa22.datastructur.es/materials/proj/proj2a/) was part of a comprehensive assignment for CS 61B. The goal was to create a browser-based tool for exploring the history of word usage in English texts. The front-end code, written in JavaScript and HTML, was provided, while I developed the back-end in Java to handle input and generate output for display. This project involved implementing various data structures and algorithms to manage and analyze large datasets efficiently.

---

### Project Requirements

**NGrams Viewer (2A):** \
The first phase focused on building an Ngrams viewer, which displays the historical frequency of individual words (1grams) over time using the Google Ngram dataset. Key components included:

- **TimeSeries:** A custom extension of the TreeMap class to handle year-wise data points.
- **NGramMap:** A class to interact with the Google Ngrams dataset, providing methods to retrieve word frequencies and compute relative frequencies over time.

[Introduction Video](https://www.youtube.com/watch?v=ri9BzE723QA&list=PL8FaHk7qbOD7-899l1hKEd5aICB9u1wrm&index=2)

**WordNet Integration (2B):** \
The second phase integrated the WordNet dataset, adding semantic analysis capabilities. Key tasks included:

- **HyponymsHandler:** Handling requests to find hyponyms (specific instances) of given words using WordNet data.
- **Graph Operations:** Developing a graph representation to manage and traverse semantic relationships in the WordNet dataset.
- **Combining Datasets:** Synthesizing results from the NGramMap and WordNet data to provide comprehensive word analysis.

[Introduction Video](https://www.youtube.com/watch?v=Em3nRZWmkUU&list=PLNpmrGKEeMf727KwSrG8Ez1o3odK--o9i&index=2)


---

### Implementation

**TimeSeries Class:**
- Extended the TreeMap class with Integer keys (years) and Double values (data points).
- Implemented utility methods for year-wise operations such as addition, division, and data retrieval.

**NGramMap Class:**
- Parsed large datasets to create maps of word counts and total counts over time.
- Provided methods for retrieving word frequencies and computing relative frequencies.

**HyponymsHandler Class:**
- Developed a graph-based approach to find and return hyponyms for given words.
- Implemented methods to handle complex queries involving multiple words and year ranges.

**Graph Operations:**
- Built a custom graph class to represent WordNet's synset relationships.
- Implemented efficient algorithms for graph traversal and data retrieval.

**Web Integration:**
- Modified provided front-end code to interact with the back-end Java handlers.
- Registered new handlers for different functionalities such as historical text and graphical plots.

---

### Features

**NGrams Viewer:** \
A tool to visualize the historical frequency of individual words over time using a subset of the Google Ngram dataset.

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/ngrams_viewer.jpg" title="NGrams Viewer" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Dynamic Graph Handling:** \
Implemented a graph structure to manage and traverse WordNet's semantic relationships efficiently.

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/graph_handling.jpg" title="Graph Operations" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Interactive Web Interface:** \
Developed handlers to process user queries and return results through an interactive web interface.

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/web_interface.jpg" title="Web Interface" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

---

### Conclusion

The NGordnet project was a multifaceted assignment that provided hands-on experience in data analysis, algorithm development, and web integration. By working on this project, I gained valuable skills in handling large datasets, developing efficient algorithms, and creating interactive web applications.

---

