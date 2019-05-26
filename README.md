# pliss2019

Titles and abstracts taken from https://pliss2019.github.io/talks.html and augmented with references.

## Secure Languages Now

Property | Value
---|---
Speaker | Cristina Cifuentes

In the cloud world, the attack surface for an application is much larger than in an on-premise deployment. Current commonly used languages provide limited support for security, with vulnerabilities such as Injection attacks (e.g., SQL injection, cross-site scripting, etc), and Leaks of sensitive data being the most representative vulnerabilities exploited in web applications over the past 5 years. Combined with the trend towards micro services, where services are language agnostic and hence are implemented by various languages at a time, we have a growing security problem that needs to be addressed now.

In this talk I give an overview of the problem, I’ll review some solutions that have practical applications, and we’ll embark on the first steps to develop a new language that addresses the lack of security concepts provided in today’s commonly used languages for web and cloud applications.

## Starting with Semantics

Property | Value
---|---
Speaker | Sylvan Clebsch

A programming language is a user interface to an abstract machine. Designing a new programming language for an existing abstract machine is an important and useful task (e.g. Scala on the JVM, F# on the CLR, etc.), but sometimes we want to design a new abstract machine, perhaps to cope with custom hardware, to provide a new approach to concurrency, or to provide new runtime guarantees to the source language. Let's talk about writing a small-step operational semantics and designing a runtime, using Pony (and a hypothetical extension to the Pony abstract machine) as an example.

## Polyhedral compilation as a compiler construction design pattern

Property | Value
---|---
Speaker |  Albert Cohen

...leveraging high-performance computing experience to program the next generation machine learning accelerators.

## First-Class Continuations

Property | Value
---|---
Speaker | Arjun Guha
Website | https://plasma-umass.org/pliss2019/

## A little (more) about V8 and WebAssembly

Property | Value
---|---
Speaker | Ben L. Titzer

This talk will focus on details about V8's approach to running JavaScript and WebAssembly code.

## Crafting a responsive compiler

Property | Value
---|---
Speaker | Nicholas Matsakis
Speaker Affiliation | Mozilla Research
Slides | https://nikomatsakis.github.io/pliss-2019/responsive-compilers.html
Slides sources | https://github.com/nikomatsakis/pliss-2019
Related implementation | https://github.com/rust-analyzer/rust-analyzer

Many compiler textbooks and courses treat compilation as a "batch process", where the compiler takes in a bunch of input files, executes a suite of comiler passes, and ultimately produces object code as output. Increasingly, though, users expect integration with IDEs like VSCode, which requires a different structure. Moreover, many languages have recursive constructs where the correct processing order is difficult to determine statically. Nicholas will discuss some of the work the Rust team has been doing on restructuring the compiler to support incremental compilation and IDE integration.

## Static Program Analysis

Property | Value
---|---
Speaker | Anders Møller
Related Course | https://cs.au.dk/~amoeller/spa/

Static program analysis is the art of reasoning about the behavior of computer programs without actually running them. This is useful not only in optimizing compilers for producing efficient code but also for automatic error detection and other tools that can help programmers.

This lecture will present essential principles and algorithms for static program analysis, based on material from http://cs.au.dk/~amoeller/spa/. We take a constraint-based approach where suitable constraint systems conceptually divide analysis into a front-end that generates constraints from program code and a back-end that solves the constraints to produce the analysis results. If time permits, the lecture will be accompanied by theoretical exercises and by practical exercises based on a Scala implementation of the algorithms.

## Theory & Practice - Language tooling development in Industry

Property | Value
---|---
Speaker | Joe Pamer

The approach to language and compiler design taken by industry can differ greatly from the state of the art documented in academic literature (or even open source). Runtime performance and reusability often take a back seat to scalability, affinity for tooling, and even product marketing. This difference in priorities can result in design or implementation decisions that feel counter-intuitive to the uninitiated, but are necessary for staying ahead of the steep adoption curves we often experience. After years of indoctrinating new hires in this different and scantly documented point of view, I'd like to open up a bit and maybe even open up some new lines of inquiry.

In this lecture I'll be enumerating the differences between the "theory" and "practice" of language development as I've experienced them in my years in industry. In doing so I'll be taking you on a tour of the entire stack - from VMs and back-end code generators, to type checkers, parsers, standard libraries, and IDEs - explaining how approaches may differ from what you'd expect, and how seemingly minor language design decisions can result in massive opportunity costs. Along the way I'll provide plenty of anecdotes about the pleasant surprises and regretable mistakes behind some of today's more popular developer tools, and outline where I think things are going in the decade to come.


## The coming persistence apocalypse 

Property | Value
---|---
Speaker | Mario Wolczko

DRAM’s dominance may be coming to an end, and sooner than you think. New memory technologies promise increased density, decreased cost and most importantly, an end to volatility, since they do not need power to maintain state. The consequences for the way we program — and on the design of programming languages — will be profound. In this presentation I’ll describe the opportunities and challenges that arise from Non-Volatile RAM, and the plethora of PhD-worthy problems that will need to be solved.
