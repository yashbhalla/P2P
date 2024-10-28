# P2P

## Team Members
- Shrey Gupta
- Yash Bhalla

## Overview

The Chord protocol is designed to efficiently locate nodes responsible for storing a particular data item in a distributed system. This implementation uses consistent hashing to assign keys to nodes and provides a scalable solution for peer-to-peer systems.

The project consists of two main actor types:

- `ChordNetwork`: Manages the overall network, including node creation, initialization, and lookup routing.
- `ChordNode`: Represents individual nodes in the Chord network, handling lookups and maintaining successor information.

Key features of the implementation include:
- Consistent hashing for node ID assignment
- Finger table initialization and usage for efficient routing
- Bubble sort algorithm for sorting node IDs

## Failure Models

This implementation includes two types of failure models:
1. Node Failure: Simulated in the `ChordNetwork` actor with a 10% probability during lookups.
2. Connection Failure: Simulated in the `ChordNode` actor with a 5% probability during lookups.

These failure models help test the resilience of the Chord network under adverse conditions.
