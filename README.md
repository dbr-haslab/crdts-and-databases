# CRDTs and Databases: A Hands-On Tutorial

## Overview

Traditional isolation models such as Serializability or Snapshot Isolation, with a total commit order, are not compatible with large-scale, highly-available partition-tolerant services. Even a weaker model such as Parallel Snapshot Isolation, while allowing different commit orders at different sites, when defined for the traditional read-write API,  must imply either aborting concurrent transactions on shared objects or losing updates. The only way out is to offer transactions over higher-level shared abstractions beyond a read-write API. Conflict-free Replicated Data Types (CRDTs) are such an abstraction. But CRDTs and relational databases have been developed in two worlds apart. Existing CRDT databases have ad hoc non-relational implementations that are not easily combined with database systems, in particular, regarding query optimization which is the mainstay of SQL systems.
This tutorial covers how to bring these two worlds together. First, it provides solid coverage of what CRDTs are, and their main approaches, in a self-contained way. Then it addresses how CRDTs can be combined with the relational model, accessed by standard SQL, and implemented over standard relational databases, by the recent notion of Confilct-free Replicated Data Views.

## Slides

To appear.
