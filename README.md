## Introduction

Welcome to this project, where we’re cutting through the fluff to find bugs without needing to know a single line of a system's internals. The whole point is simple: define "what" systems should achieve, then let advanced testing methodologies tear through them to see if they hold up. This project builds on top of Damn Vulnerable DeFi, thanks to Tincho and his team. Massive shoutout to Tincho—he's a true legend and deserves serious respect. Check out his [Damn vulnerable Defi Repo](https://www.damnvulnerabledefi.xyz/), [Blog](https://blog.theredguild.org/author/tincho/), or [YouTube](https://www.youtube.com/@watchtheredguild) if you haven’t already.

## Objective

Our main goal? Prove that you can catch bugs by focusing purely on a system's expected behavior—no need to understand every line of its code.

## Methodology

We’re diving into property-based testing and formal verification. These techniques are powerhouses in their own right but take different approaches:

1. **Fuzzing**: Think brute-force on steroids. It probes the entire state space, or close to it, using informed guesses that improve with each test. (I’m assuming you have a brain and are using a generator-shrinker, not just throwing dice)
2. **Formal Verification (FV)**: FV, on the other hand, uses hard math and logic to analyze both current and future states, giving a more structured insight.

In simple terms, fuzzing is like building an ultra-detailed problem model to get a rough solution. Formal verification, on the other hand, involves creating an estimated model to derive a mathematically sound solution—even if that model isn’t perfect. (Why isn’t it perfect? Because modeling your protocol in exact specifications isn’t possible. And if you think it is, you’re delusional.)

## Tools and Preferences

I’ve worked with tools like Foundry, Echidna, Medusa, Certora, and TLA+ for formal verification. But here, we’ll focus on Echidna. Why?

1. **Community and Reliability**: Echidna's community is strong, and it's proven itself time and again.
2. **Mathematical Affinity**: For math fans, Echidna’s approach fits nicely as it starts from a simple point like an EOA.
3. **Logical Design**: Designing intermediate contracts for Echidna tests aligns with a mathematically rigorous mindset.

Join us as we take formal verification and property-based testing to new heights in bug detection while pushing back against the status quo. Let’s get started.