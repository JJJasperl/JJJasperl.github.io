---
layout: page
title: Pac-Man
description: Learn foundational AI concepts with Pac-Man, including search, probabilistic inference, and reinforcement learning.
img: assets/img/pacman.jpg
importance: 2
category: School Projects
related_publications: false
---

### Overview

The [Pac-Man projects](https://inst.eecs.berkeley.edu/~cs188/sp24/projects/) were developed for CS 188. They apply an array of AI techniques to playing Pac-Man. However, these projects don’t focus on building AI for video games. Instead, they teach foundational AI concepts, such as informed state-space search, probabilistic inference, and reinforcement learning. These concepts underly real-world application areas such as natural language processing, computer vision, and robotics.

---

### Part 1: Search

I implemented depth-first, breadth-first, uniform cost, and A* search algorithms. These algorithms are used to solve navigation and traveling salesman problems in the Pacman world.

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/search.jpg" title="Search" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

---

### Part 2: Multi-Agent Search

Classic Pacman is modeled as both an adversarial and a stochastic search problem. I implemented multiagent minimax and expectimax algorithms, as well as designing evaluation functions.

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/multiagent.jpg" title="Multi-Agent Search" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

---

### Part 3: Logic and Classical Planning

Pacman world is represented with booleans, and logical inference is used to solve planning tasks as well as localization, mapping, and SLAM.

---

### Project 4: Bayes Nets and HMMs

Pacman uses probabilistic inference on Bayes Nets and the forward algorithm and particle sampling in a Hidden Markov Model to find ghosts given noisy readings of distances to them.

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/bayesnets.jpg" title="Bayes Nets and HMMs" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

---

### Part 5: Machine Learning

I implemented the perceptron algorithm, neural network, and recurrent nn models, and applied the models to several tasks including digit classification and language identification.

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/machinelearning.jpg" title="Machine Learning" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

---

### Part 6: Reinforcement Learning

I implemented Value Function, Q learning, and Approximate Q learning to help pacman and crawler agents learn rational policies.


---

### Technical Notes

The Pac-Man projects are written in pure Python 3.6+ and do not depend on any packages external to a standard Python distribution, except the Logic and ML projects.
