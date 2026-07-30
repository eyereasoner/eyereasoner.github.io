---
marp: true
theme: default
paginate: true
title: One Home, Three Doors
description: Eyeling, Eyeleng, and Eyepl — three ways into explainable reasoning
---

# One home, three doors

## Eyeling · Eyeleng · Eyepl

Three ways into explainable reasoning

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
| **Eyeleng** | SHACL and RDF rules | Standards-oriented RDF processing |
| **Eyepl** | Prolog and relational programming | Logic programs with RDF interchange |

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

**In one phrase:** linked-data reasoning that stays close to the Web stack.

---

# What happened in Eyeling

Eyeling became a more focused and capable N3 reasoner.

- RDF 1.2 support was broadened.
- Proofs became N3 data that can themselves be parsed and queried.
- RDF Message logs gained replay and streaming workflows.
- Parsing, indexing, memoization, and memory use were improved.
- The browser playground and collection of practical examples grew.
- SHACL and SRL work moved into the separate **Eyeleng** project.

---

# Door 2 — Eyeleng

**Eyeleng** means **EYE Logic Engine**.

It is a JavaScript implementation centered on **SHACL Rules**, with:

- a compact **SRL** rule syntax;
- an **RDF Rules** syntax;
- RDF 1.1 and RDF 1.2 support;
- W3C tests and machine-readable conformance reports;
- forward, backward, and automatically hybrid reasoning.

SHACL describes what good RDF data should look like. SHACL Rules can also derive new data from those descriptions.

**In one phrase:** standards-facing RDF rules with practical query planning.

---

# What happened in Eyeleng

Eyeleng grew from a SHACL Rules implementation into a practical hybrid engine.

- SHACL Rules, SRL, and RDF Rules were brought together.
- W3C conformance tests and EARL reports were added.
- RDF parsing and semantics were strengthened.
- Forward and backward reasoning were combined automatically.
- Recursion, generated identifiers, and selective indexes were improved.
- A playground, examples, and golden-output tests made behavior easier to explore.

---

# Door 3 — Eyepl

**Eyepl** combines EYE-style reasoning with **Prolog-like logic programming**.

Its core provides:

- facts, rules, unification, backtracking, arithmetic, and lists;
- explicit questions and inspectable proofs;
- automatic tabling for recursive problems;
- demand-driven clause indexing;
- tools that map RDF 1.2 datasets to and from relational facts.

Eyepl gives Prolog users a route to RDF—and linked-data users a compact relational rule language.

**In one phrase:** portable logic programs with an RDF 1.2 bridge.

---

# What happened in Eyepl

Eyepl became a standards-conscious Prolog-style reasoner with an RDF bridge.

- The core was aligned with ISO Prolog concepts and error behavior.
- Optional library predicates were separated clearly from the core.
- Automatic tabling and demand-driven indexes improved recursive workloads.
- RDF 1.2 conversion and round-trip tools were added.
- Proofs, explicit queries, safety checks, and inference fuses were developed.
- *The Art of Eyepl*, browser tooling, conformance tests, and examples made the language easier to learn and verify.

