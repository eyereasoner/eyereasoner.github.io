---
layout: slides
marp: true
theme: default
paginate: true
title: One Home, Two Doors
description: Eyeling and Eyelang — two ways into explainable reasoning
---

# One home, two doors

## Eyeling · Eyelang

Two ways into explainable reasoning

---

# First: what is a reasoner?

A reasoner is software that combines:

- **facts** — what we know;
- **rules** — how conclusions follow;
- **questions** — what we want to discover.

It produces new conclusions—and can preserve enough evidence to explain where those conclusions came from.

> Think of a spreadsheet whose formulas can work over a web of knowledge, not just cells.

---

# A tiny example

```text
Fact:     Socrates is a person.
Rule:     Every person is mortal.
Result:   Socrates is mortal.
```

The same pattern can be applied to:

- linked data from several organizations;
- policies, permissions, and compliance;
- scientific and engineering calculations;
- live streams of RDF messages;
- recursive searches, planning, and validation.

---

# One home, three different doors

The home is **explainable reasoning**:

> Facts and rules become conclusions that people can inspect.

| Door | Way in | Best fit |
|---|---|---|
| **Eyeling** | Notation3 and the Semantic Web | Linked-data rules and proofs |
| **Eyelang** | Prolog and relational programming | Logic programs with RDF interchange |

The projects share ideas, but each offers a different language and starting point.

---

# Door 1 — Eyeling

**Eyeling** is a compact JavaScript reasoner for **Notation3**, or N3.

Notation3 extends RDF with rules and quoted graphs. It can express both knowledge and transformations of knowledge in a Web-friendly form.

Eyeling emphasizes:

- forward and goal-directed reasoning;
- N3 proofs that are themselves parseable data;
- RDF 1.2 and RDF Message workflows;
- command-line, JavaScript API, and browser use;
- a broad library of executable examples.

---

## What happened in Eyeling

Eyeling became a more focused and capable N3 reasoner.

- RDF 1.2 support was broadened.
- Proofs became N3 data that can themselves be parsed and queried.
- RDF Message logs gained replay and streaming workflows.
- Parsing, indexing, memoization, and memory use were improved.
- The browser playground and collection of practical examples grew.

---

# Door 2 — Eyelang

Standards are crucial for durable, interoperable reasoning.

**Eyelang combines ISO Prolog and W3C RDF 1.2** to turn portable rules and linked data into answers and inspectable proofs—without inventing another proprietary language or data model.

Its core provides:

- facts, rules, unification, backtracking, arithmetic, and lists;
- explicit questions and inspectable proofs;
- automatic tabling for recursive problems;
- demand-driven clause indexing;
- tools that map RDF 1.2 datasets to and from relational facts.

Eyelang gives Prolog users a route to RDF—and linked-data users a compact relational rule language.

---

## What happened in Eyelang

Eyelang brought two established standards together in one reasoner.

- The reasoning language was aligned with standard ISO Prolog behavior.
- Optional library predicates were separated clearly from the core.
- Automatic tabling and demand-driven indexes improved recursive workloads.
- RDF 1.2 conversion and round-trip tools were added.
- Proofs, explicit queries, safety checks, and inference fuses were developed.
- **The Art of Eyelang** book, browser tooling, conformance tests, and examples made the language easier to learn and verify.
