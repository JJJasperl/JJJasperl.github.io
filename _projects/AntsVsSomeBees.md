---
layout: page
title: Ants Vs. SomeBees
description: A tower defense game inspired by Plants Vs. Zombies
img: assets/img/antsvssomebees.jpg
importance: 3
category: School Projects
related_publications: false
---

### Overview

[Ants Vs. SomeBees](https://inst.eecs.berkeley.edu/~cs61a/fa22/proj/ants/) is a tower defense game developed as a part of a CS 61A project. The objective of the game is to protect the ant queen from invading bees by strategically placing different types of ants. The project focuses on object-oriented programming, involving the implementation and extension of various classes to manage game logic, insects, and interactions between them.

---

### Project Requirements

**Part 1: Basic Gameplay**
- Implemented two basic ants: HarvesterAnt and ThrowerAnt.
- HarvesterAnt gathers food for the colony, while ThrowerAnt attacks bees in its place.
- Modified the game logic to handle food costs for placing ants and tracking entrances and exits in places.

**Part 2: More Ants!**
- Introduced specialized ants with different attack strategies, such as LongThrower, ShortThrower, FireAnt, WallAnt, HungryAnt, BodyguardAnt, TankAnt, and SlowThrower.
- Implemented different behaviors and actions for each ant type to enhance gameplay and strategy.

**Part 3: Water and Might**
- Added water as a new place type, requiring waterproof insects to occupy them.
- Introduced the ScubaThrower and the QueenAnt.
- The QueenAnt has special rules, such as doubling the damage of ants behind her and ensuring there is only one queen in the game.

---

### Implementation

**Ants and Bees:**
- Developed classes for various ant and bee types, each with specific attributes and actions.
- Implemented logic for ant placement, food cost management, and bee movement and attack strategies.

**Places and Colony:**
- Created a colony structure consisting of linked places forming tunnels.
- Implemented tracking of entrances and exits for proper game mechanics.

**Game Logic:**
- Managed the game state, including food availability, time progression, and winning/losing conditions.
- Developed methods to handle the actions of all insects in each turn.

**Graphical User Interface (GUI):**
- Provided a GUI to visualize the game state and interact with the game.
- Implemented text-based and graphical modes for different gameplay experiences.

---

### Conclusion

The Ants Vs. SomeBees project was a comprehensive assignment that provided hands-on experience in object-oriented programming, game development, and complex system design. By working on this project, I gained valuable skills in managing game state, implementing diverse behaviors for game entities, and creating interactive user interfaces.

---

