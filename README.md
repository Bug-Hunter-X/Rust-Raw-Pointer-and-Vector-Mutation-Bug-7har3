# Rust Raw Pointer and Vector Mutation Bug

This repository demonstrates a common error in Rust programming involving the unsafe use of raw pointers with vectors. The `bug.rs` file shows the incorrect usage, which can lead to undefined behavior and potential crashes. The `bugSolution.rs` file provides a corrected and safer approach.

## Problem

The original code attempts to modify a vector's contents via a raw pointer. This is generally unsafe because it bypasses Rust's memory safety mechanisms.  If the vector goes out of scope or is modified in other ways, the pointer becomes invalid.  Accessing an invalid pointer can lead to crashes or unpredictable behavior.

## Solution

The solution emphasizes using safer methods provided by the Rust standard library, ensuring memory safety and avoiding the risks associated with raw pointers. The use of safer methods avoids potential memory corruption and undefined behavior, making the code more robust and reliable.