---
marp: true
theme: default
paginate: true
title: Four Ways to Make Knowledge Reason
description: Eyeling, Eyeleng, Eyeron, and Eyepl — what they are and recent progress
---

# Four ways to make knowledge reason

## Eyeling · Eyeleng · Eyeron · Eyepl

What they are, why they exist, and how they have developed

---

# First: what is a reasoner?

A reasoner is software that combines:

- **facts** — what we know;
- **rules** — how conclusions follow;
- **questions** — what we want to discover.

It produces new conclusions—and, in these projects, can preserve enough evidence to explain where those conclusions came from.

> Think of a spreadsheet whose formulas can work over a web of knowledge, not just cells.

---

# A tiny example

```text
Fact:     Socrates is a person.
Rule:     Every person is mortal.
Result:   Socrates is mortal.
```

The interesting part is not this toy conclusion. It is applying the same pattern to:

- linked data from several organizations;
- policies, permissions, and compliance;
- scientific and engineering calculations;
- live streams of RDF messages;
- recursive searches, planning, and validation.

---

# One family, four different doors

| Project | Main language | Implementation | Best fit |
|---|---|---|---|
| **Eyeling** | Notation3 (N3) | JavaScript | Web-native linked-data rules and proofs |
| **Eyeleng** | SHACL Rules, SRL, RDF Rules | JavaScript | Standards-oriented RDF rule processing |
| **Eyeron** | Notation3 (N3) | Rust + WebAssembly | Native speed, safety, embedding, and browsers |
| **Eyepl** | ISO-style Prolog + RDF 1.2 | JavaScript | Logic programming with linked-data interchange |

They overlap deliberately, but optimize for different languages, environments, and audiences.

---

# Eyeling: reasoning in the language of the Web

**Eyeling** is a compact JavaScript reasoner for **Notation3**.

Notation3 extends RDF with rules and quoted graphs. That makes it possible to express both knowledge and transformations of knowledge in a Web-friendly form.

Eyeling emphasizes:

- forward and goal-directed reasoning;
- N3 proofs that are themselves parseable data;
- RDF 1.2 and RDF Message workflows;
- command-line, JavaScript API, and browser playground use;
- a broad library of executable examples.

**In one phrase:** linked-data reasoning that stays close to the Web stack.

---

# What happened in Eyeling

Eyeling became a more focused and capable N3 reasoner.

- RDF 1.2 support was broadened.
- Proofs became N3 data that can themselves be parsed and queried.
- RDF Message logs gained replay and streaming workflows.
- Parsing, indexing, memoization, and memory use were improved.
- The browser playground and collection of practical examples grew.
- SHACL/SRL work moved into the separate **Eyeleng** project.

---

# Eyeleng: rules for RDF standards

**Eyeleng** means **EYE Logic Engine**.

It is a JavaScript implementation centered on **SHACL 1.2 Rules**, with:

- a compact **SRL** rule syntax;
- an **RDF Rules** syntax front end;
- RDF 1.1/1.2 parsing and entailment support;
- W3C manifest runners and machine-readable EARL reports;
- forward, backward, and automatically hybrid reasoning.

For a wide audience: SHACL starts as a way to describe what good RDF data should look like. SHACL Rules adds the ability to derive new data from those descriptions.

**In one phrase:** standards-facing RDF rules with practical query planning.

---

# What happened in Eyeleng

Eyeleng grew from a SHACL Rules implementation into a practical hybrid engine.

- SHACL Rules, SRL, and RDF Rules were brought together.
- W3C conformance tests and EARL reports were added.
- RDF 1.1 and RDF 1.2 parsing and semantics were strengthened.
- Forward and backward reasoning were combined automatically.
- Recursion, generated identifiers, and selective indexes were improved.
- A playground, runnable examples, and golden-output tests made behavior easier to explore.

---

# Eyeron: N3 reasoning forged in Rust

**Eyeron** combines “Eye” with the sound of “iron.”

It brings N3 reasoning to Rust:

- native command-line and library use;
- memory-safe systems implementation;
- WebAssembly for browser use;
- forward and backward rules;
- proof output;
- RDF 1.1/1.2 input;
- RDF Message replay and streaming;
- indexed lookup and optimized rule execution.

Rust makes Eyeron attractive where predictable deployment, native integration, and performance matter.

**In one phrase:** an explainable N3 engine for native and WebAssembly environments.

---

# What happened in Eyeron

Eyeron established a Rust and WebAssembly implementation of N3 reasoning.

- N3 and W3C RDF conformance suites were added.
- Explainable proofs gained golden regression coverage.
- Native RDF lists and a broad set of built-ins were implemented.
- RDF Message replay and message-at-a-time streaming were added.
- A browser playground and reusable WebAssembly interface were created.
- Performance, safety limits, proof traversal, and RDF output were hardened.

---

# Eyepl: logic programming meets linked data

**Eyepl** combines EYE-style reasoning with **Prolog-like logic programming**.

Its core is aligned with the familiar ISO Prolog model:

- facts, rules, unification, backtracking, arithmetic, lists, and dynamic predicates;
- explicit queries and inspectable proofs;
- automatic tabling for recursive problems;
- demand-driven clause indexing;
- tools that map RDF 1.2 datasets to and from ordinary relational facts.

Eyepl gives Prolog users a direct route to RDF—and linked-data users a compact relational rule language.

**In one phrase:** portable logic programs with an RDF 1.2 bridge.

---

# What happened in Eyepl

Eyepl became a standards-conscious Prolog-style reasoner with an RDF bridge.

- The core was aligned with ISO Prolog concepts and error behavior.
- Optional library predicates were separated clearly from the core.
- Automatic tabling and demand-driven indexes improved recursive workloads.
- RDF 1.2 conversion and round-trip tools were added.
- Proofs, explicit queries, safety checks, and inference fuses were developed.
- *The Art of Eyepl*, browser tooling, conformance tests, and a large example collection made the language easier to learn and verify.
