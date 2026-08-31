# CRDTs and Databases: A Hands-On Tutorial

## Overview

Traditional isolation models such as Serializability or Snapshot Isolation, with a total commit order, are not compatible with large-scale, highly-available partition-tolerant services. Even a weaker model such as Parallel Snapshot Isolation, while allowing different commit orders at different sites, when defined for the traditional read-write API,  must imply either aborting concurrent transactions on shared objects or losing updates. The only way out is to offer transactions over higher-level shared abstractions beyond a read-write API. Conflict-free Replicated Data Types (CRDTs) are such an abstraction. But CRDTs and relational databases have been developed in two worlds apart. Existing CRDT databases have ad hoc non-relational implementations that are not easily combined with database systems, in particular, regarding query optimization which is the mainstay of SQL systems.
This tutorial covers how to bring these two worlds together. First, it provides solid coverage of what CRDTs are, and their main approaches, in a self-contained way. Then it addresses how CRDTs can be combined with the relational model, accessed by standard SQL, and implemented over standard relational databases, by the recent notion of Conflict-free Replicated Data Views.

## Slides

- [Part 0: Introduction](slides/part0-intro.pdf)
- [Part 1:  Conflict-free Replicated Data Types](slides/part1-CRDTs.pdf)
- [Part 2: CRDTs in database systems](slides/part2-survey.pdf)
- [Part 3: CRDVs Hands-On](slides/part3-hands-on.pdf)
- [Part 4: Open challenges](slides/part4-challenges.pdf)

## Related work

- Paulo Sérgio Almeida. 2025. Approaches to Conflict-free Replicated Data Types.
ACM Comput. Surv. 57, 2 (2025), 51:1–51:36. [DOI:10.1145/3695249](https://doi.org/10.1145/3695249)

- Nuno Faria and José Pereira. 2025. CRDV: Conflict-free Replicated Data Views.
Proc. ACM Manag. Data 3, 1, Article 25 (Feb. 2025). [DOI:1145/3709675](https://doi.org/10)

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

