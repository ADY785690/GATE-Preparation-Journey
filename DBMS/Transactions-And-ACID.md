# Transactions and ACID Properties

## What is a Transaction?

A transaction is a sequence of database operations that performs a single logical unit of work.

Example:

Transfer ₹1000 from Account A to Account B

1. Deduct ₹1000 from A
2. Add ₹1000 to B

Both operations must complete successfully.

---

# Transaction States

1. Active
2. Partially Committed
3. Committed
4. Failed
5. Aborted

---

# ACID Properties

## A - Atomicity

Either all operations execute or none execute.

Example:

Money deducted from A but not added to B.

This should not happen.

---

## C - Consistency

Database must remain in a valid state before and after transaction.

---

## I - Isolation

Concurrent transactions should not interfere with each other.

---

## D - Durability

Once committed, data remains permanent even after system failure.

---

# Example

Transaction:

Read(A)

A = A - 100

Write(A)

Read(B)

B = B + 100

Write(B)

Commit

---

# GATE Important Points

✓ Atomicity = All or Nothing

✓ Consistency = Valid Database State

✓ Isolation = No Interference

✓ Durability = Permanent Storage

✓ ACID questions are frequently asked
