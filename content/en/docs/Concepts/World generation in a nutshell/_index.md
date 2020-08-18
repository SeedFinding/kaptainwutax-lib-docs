---
title: "World Generation in a nutshell"
linkTitle: "World Generation in a nutshell"
weight: 10
description: >
  The world generation described succinctly
---

Before anything, we need to agree to some notations since those will be used later on.

Let's rule out a few stuffs first: 
 - The Java Random class use a 48 bit LCG which mean any number inputted inside will be constrained to 48 bits 
 number (also known as modulo (2^48)-1).
 - The only place where the full 64 bits size of a `long` is used in the Biome [QLCG](http://statmath.wu.ac.at/software/prng/doc/prng.html#QCG).
 - When using a string seed you can only hit the 2^32 range.
 - When using a random seed you can only hit the 48 bit range and only 82% of it see [that]()