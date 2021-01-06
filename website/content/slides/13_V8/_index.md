---
title: "V8"
date: 2018-08-02T17:45:53+03:00
draft: false
outputs: ["Reveal"]
---
# Contents

- Introduction
- The V8 architecture
- Turbofan

---
# Introduction

---
# Parsing

---
# The Ignition interpreter

---
# The object heap

---
# Runtime and builtins (CSA, Torque)

---
# Code generation

---
# Object memory layout and Smi/double representation

---
# GC

---
# Wasm pipeline - Liftoff
---
# Part 2: Turbofan

---
# Optimization pipeline

---
# Operator types (high to low level)

- JavaScript operators
  - Express semantics of JavaScript’s overloaded operators
  - Produce and consume effects in the graph
- Simplified operators
  - Express VM-level operations, such as allocation, bounds checks
  - Arithmetic independent of number representation
- Machine operators
  - Correspond closely to single machine instructions
  - Most are side effect free
  - Must be supported by platform-specific backends

---
# Operator types - examples

- JavaScript operators
  - JSAdd, JSBitwiseAnd, JSCall
- Simplified operators
  - NumberAdd, StringAdd, {Load|Store}Field, ChangeTaggedToInt32
- Machine operators
  - Int32Add, Float64Add, Load, Store, Call

---
# Some important reductions

- Constant folding
- Strenght reduction
- Load elimination
- Redundancy elimination
- Typed lowering

---
# Reductions

![Constant folding](/IPL/images/01-constant-folding.png)

---
# Type and range analysis

---
# Typed lowering

---
# Global value numbering (GVN)

---
# Function inlining

---
# Optimized code generation

---
# A simple types example - from JS to x86 assembly

---
# Thank you!

GitHub: Maya Lekova
Twitter: zmayski@
