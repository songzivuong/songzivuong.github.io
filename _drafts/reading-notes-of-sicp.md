---
layout: post
title: "Reading Notes of SICP"
categories: Reading Programming
tags: lisp scheme
---

Reading notes of [*Structure and Interpretation of Computer Programs*, 2nd Edition](https://mitpress.mit.edu/sites/default/files/sicp/full-text/book/book.html) (Harold Abelson and Gerald Jay Sussman, 1996).

{% include toc %}

## Building Abstractions with Procedures
### The Elements of Programming
#### Expressions
#### Naming and the Environment
#### Evaluating Combinations
#### Compound Procedures
#### The Substitution Model for Procedure Application
#### Conditional Expressions and Predicates
#### Example: Square Roots by Newton's Method
#### Procedures as Black-Box Abstractions
### Procedures and the Processes They Generate
#### Linear Recursion and Iteration
#### Tree Recursion
#### Orders of Growth
#### Exponentiation
#### Greatest Common Divisors
#### Example: Testing for Primality
### Formulating Abstractions with Higher-Order Procedures
#### Procedures as Arguments
#### Constructing Procedures Using Lambda
#### Procedures as General Methods
#### Procedures as Returned Values
## Building Abstractions with Data
### Introduction to Data Abstraction
#### Example: Arithmetic Operations for Rational Numbers
#### Abstraction Barriers
#### What Is Meant by Data?
#### Extended Exercise: Interval Arithmetic
### Hierarchical Data and the Closure Property
#### Representing Sequences
#### Hierarchical Structures
#### Sequences as Conventional Interfaces
#### Example: A Picture Language
### Symbolic Data
#### Quotation
#### Example: Symbolic Differentiation
#### Example: Representing Sets
#### Example: Huffman Encoding Trees
### Multiple Representations for Abstract Data
#### Representations for Complex Numbers
#### Tagged data
#### Data-Directed Programming and Additivity
### Systems with Generic Operations
#### Generic Arithmetic Operations
#### Combining Data of Different Types
#### Example: Symbolic Algebra
## Modularity, Objects, and State
### Assignment and Local State
#### Local State Variables
#### The Benefits of Introducing Assignment
#### The Costs of Introducing Assignment
### The Environment Model of Evaluation
#### The Rules for Evaluation
#### Applying Simple Procedures
#### Frames as the Repository of Local State
#### Internal Definitions
### Modeling with Mutable Data
#### Mutable List Structure
#### Representing Queues
#### Representing Tables
#### A Simulator for Digital Circuits
#### Propagation of Constraints
### Concurrency: Time Is of the Essence
#### The Nature of Time in Concurrent Systems
#### Mechanisms for Controlling Concurrency
### Streams
#### Streams Are Delayed Lists
#### Infinite Streams
#### Exploiting the Stream Paradigm
#### Streams and Delayed Evaluation
#### Modularity of Functional Programs and Modularity of Objects
## Metalinguistic Abstraction
### The Metacircular Evaluator
#### The Core of the Evaluator
#### Representing Expressions
#### Evaluator Data Structures
#### Running the Evaluator as a Program
#### Data as Programs
#### Internal Definitions
#### Separating Syntactic Analysis from Execution
### Variations on a Scheme -- Lazy Evaluation
#### Normal Order and Applicative Order
#### An Interpreter with Lazy Evaluation
#### Streams as Lazy Lists
### Variations on a Scheme -- Nondeterministic Computing
#### Amb and Search
#### Examples of Nondeterministic Programs
#### Implementing the Amb Evaluator
### Logic Programming
#### Deductive Information Retrieval
#### How the Query System Works
#### Is Logic Programming Mathematical Logic?
#### Implementing the Query System
## Computing with Register Machines
### Designing Register Machines
#### A Language for Describing Register Machines
#### Abstraction in Machine Design
#### Subroutines
#### Using a Stack to Implement Recursion
#### Instruction Summary
### A Register-Machine Simulator
#### The Machine Model
#### The Assembler
#### Generating Execution Procedures for Instructions
#### Monitoring Machine Performance
### Storage Allocation and Garbage Collection
#### Memory as Vectors
#### Maintaining the Illusion of Infinite Memory
### The Explicit-Control Evaluator
#### The Core of the Explicit-Control Evaluator
#### Sequence Evaluation and Tail Recursion
#### Conditionals, Assignments, and Definitions
#### Running the Evaluator
### Compilation
#### Structure of the Compiler
#### Compiling Expressions
#### Compiling Combinations
#### Combining Instruction Sequences
#### An Example of Compiled Code
#### Lexical Addressing
#### Interfacing Compiled Code to the Evaluator