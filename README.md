<div align="center">

# Scalable Decentralized Asynchronous System Design: Camera–Monitor Architecture  
© August 2025, Yehonatan Barel  

</div>


---

## Introduction
This project presents the design of a scalable, decentralized, and asynchronous Camera–Monitor system that operates using shared memory.  
The system consists of two independent agents – a **camera** and a **monitor** that coordinate only through shared-memory pointers, flags, and metadata while following simple rules. Each agent runs at its own clock frequency and continues functioning even if the other is removed.  

With only minor adjustments, the same principles extend naturally to many more agents, making the design inherently scalable.  
The first part of the project explores the baseline case of one camera and one monitor, while later sections extend the same principles to multi-agent scaling.

---

## Motivation
This project was created to show how simple decentralized rules, when combined with a shared resource, can produce robust and scalable system behavior.  
Instead of relying on a central controller, each agent operates independently, coordinating only through shared-memory flags.  

This approach emphasizes core principles of system design:
- **Simplicity**
- **Fault tolerance**
- **Scalability**

---

## Concepts Demonstrated

### Core Concepts
- **Decentralized Asynchrony** – agents operate independently at different clock rates, without a master controller or global timing.  
- **Shared-Memory Communication** – coordination occurs only through flags, pointers, and metadata, avoiding direct messaging.  
- **Scalability** – the same mechanism extends naturally to multiple agents with minimal design changes.  

### Additional Concepts
- **Fault Tolerance and Low Coupling** – the system continues functioning even if one agent fails, and each agent can be upgraded or replaced independently.  
- **Overlap Optimization** – in certain configurations, reads and writes can proceed in parallel, reducing latency and improving efficiency.  
- **Future Extensions** – this design offers a glimpse of many possible improvements and advanced variations, explored in later sections.  

---

## Repository Contents
📄 **Scalable Decentralized Asynchronous System Design.pdf**
