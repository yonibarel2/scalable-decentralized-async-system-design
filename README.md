# scalable-decentralized-async-system-design
This project presents a scalable, decentralized, and asynchronous Camera-Monitor system using shared memory. Two agents coordinate only through flags, pointers, and metadata, each running at its own clock. The design extends from one Camera-Monitor pair to many agents, enabling concurrent reads/writes with order, consistency, and efficiency.
