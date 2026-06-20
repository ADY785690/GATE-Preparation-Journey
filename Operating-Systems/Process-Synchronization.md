# Process Synchronization

## What is Process Synchronization?

Process Synchronization ensures that multiple processes can access shared resources safely without causing data inconsistency.

---

# Critical Section Problem

A Critical Section is a part of a program where shared resources are accessed.

Example:

Two processes updating the same bank account balance.

---

# Structure of a Process

1. Entry Section
2. Critical Section
3. Exit Section
4. Remainder Section

---

# Requirements of Critical Section Problem

## 1. Mutual Exclusion

Only one process can enter the Critical Section at a time.

## 2. Progress

If no process is in Critical Section, a waiting process should be selected.

## 3. Bounded Waiting

A process should not wait forever.

---

# Race Condition

Occurs when multiple processes access shared data simultaneously and the final result depends on execution order.

Example:

Count = 5

Process P1 increments Count.

Process P2 increments Count.

Expected:

Count = 7

Actual:

Count may become 6.

---

# Hardware Solutions

## Disable Interrupts

CPU interrupts are disabled while executing Critical Section.

Disadvantage:

Not practical in multiprocessor systems.

---

# Software Solutions

## Peterson's Algorithm

Used for two processes.

Provides:

- Mutual Exclusion
- Progress
- Bounded Waiting

Important for GATE.

---

# Busy Waiting

A process continuously checks a condition in a loop.

Disadvantage:

CPU time wasted.

---

# GATE Important Points

✓ Race Condition occurs due to concurrent access

✓ Mutual Exclusion allows only one process

✓ Peterson's Algorithm works for two processes

✓ Busy Waiting wastes CPU cycles

✓ Critical Section is frequently asked in GATE
