---
layout: page
title: BYOW - Build Your Own World
description: A 2D tile-based world exploration engine developed from ideation to presentation.
img: assets/img/byow.jpg
importance: 2
category: School Projects
related_publications: false
---

### Overview

The [BYOW project](https://fa22.datastructur.es/materials/proj/proj3/) was part of a large design assignment for CS 61B. The goal of this project was to create an engine for generating explorable 2D tile-based worlds. This project involved working through every stage of development, from ideation to presentation, and emulated a product development cycle. The experience was designed to teach how to handle a larger piece of code with minimal starter code, much like a real-world software engineering project.


Project Presentation During Covid: [Link](https://www.youtube.com/watch?v=CgPNk4_X8Mw)


---

### Project Requirements

**Team Formation:** \
The project required collaboration with one partner, reinforcing the importance of teamwork and communication in software development.

**World Generation (3A):** \
The first phase focused on creating a world generator capable of producing random, valid 2D tile-based worlds. The worlds included distinct rooms and hallways with random dimensions and locations, ensuring each generated world was unique and explorable.

**Interactivity (3B):** \
The second phase added user interactivity, allowing control of an avatar to explore the world. The interface included a Heads-Up Display (HUD) showing information about the tiles under the mouse pointer, and the system supported saving and loading the world state.

**Ambition & Demos (3C):** \
The final phase encouraged creativity with additional features like dynamic lighting, entities with AI behaviors, and advanced UI elements. The project was evaluated based on ambition, with features like line-of-sight rendering, light sources, and interactive encounters.

---

### Implementation

**Random World Generation:**
- Created a world consisting of a 2D grid of tiles.
- Included distinct rooms and hallways, ensuring they were connected and reachable.
- Ensured hallways had turns and rooms were placed randomly without clipping off the edge of the world.

**User Interaction:**
- Implemented control of an avatar using the W, A, S, and D keys.
- Added the ability for the avatar to interact with the world.
- Created a HUD displaying tile information under the mouse pointer.

**Saving and Loading:**
- Enabled saving the world state with the ":Q" command and loading it with the "L" command.
- Ensured the system was deterministic, producing the same world for the same seed and input sequence.

---

### Ambition Features

**Dynamic Lighting:** \
Added light sources that could be toggled on and off, with light intensity diminishing with distance and not passing through walls.

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/dynamic_lighting.gif" title="Dynamic Lighting" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
 

---

### Conclusion

The BYOW project was an extensive and open-ended assignment that offered valuable insights into software engineering principles, project management, and creative problem-solving. By handling a larger piece of code with minimal starter material, I developed a robust understanding of developing complex systems and iterating on designs to achieve desired outcomes.

---

