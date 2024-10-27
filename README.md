## Introduction

Welcome to our project where we'll explore the capabilities of identifying bugs without needing direct knowledge of the internal workings of the system. The core idea is to determine "what" systems should accomplish, leveraging advanced testing methodologies.

## Objective

The primary goal of this project is to demonstrate that it is feasible to uncover bugs by focusing on the expected outcomes of the system, independent of understanding its implementation.

## Methodology

We'll utilize property-based testing and formal verification techniques. Although both possess unique qualities at a high level, they employ distinct approaches:

1. **Fuzzing**: This involves testing the entire state space randomly, or rather, using educated guesses since we learn from previous attempts.
2. **Formal Verification (FV)**: This contrasts fuzzing by employing mathematical reasoning and inductive logic to explore current and future states, offering a more structured approach.

Fuzzing represents modeling a problem with precision but determining an approximate solution. Conversely, formal verification involves constructing an estimated model and deducing a mathematically provable solution, even if the model isn't perfect. 

## Tools and Preferences

Although I am familiar with an array of tools such as Foundry's fuzzing tools, Echidna, Medusa, Certora, and TLA+ for formal verification, the focus will be on employing Echidna. The reasons are:

1. **Community and Reliability**: Echidna has a robust community and a proven track record.
2. **Mathematical Affinity**: For those who enjoy mathematics, Echidna's approach aligns well as it starts from an initial point like an EOA.
3. **Logical Design**: Crafting intermediate contracts for testing in Echidna aligns with mathematical sensibilities.

This project invites you to join this exploration of leveraging formal verification and property-based testing to enhance system reliability while challenging conventional coding practices. Let's dive in!