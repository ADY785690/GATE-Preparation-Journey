# Keys and Functional Dependency - GATE PYQs

---

## PYQ 1

Relation:

R(A, B, C)

Functional Dependencies:

A → B

B → C

Which of the following is true?

A) A → C

B) C → A

C) B → A

D) None

### Answer

✅ A) A → C

### Trick

A → B

B → C

Therefore

A → C

(Transitivity Rule)

---

## PYQ 2

Which of the following is always a Super Key?

A) Candidate Key

B) Primary Key

C) Alternate Key

D) All of the Above

### Answer

✅ D) All of the Above

### Trick

Primary Key ⊆ Candidate Key ⊆ Super Key

Alternate Key is also a Candidate Key.

---

## PYQ 3

Which key cannot contain NULL values?

A) Foreign Key

B) Alternate Key

C) Primary Key

D) Composite Key

### Answer

✅ C) Primary Key

### Why Others Are Wrong

A) Foreign Key → Can be NULL

B) Alternate Key → May be NULL

D) Composite Key → Depends on attributes

---

## PYQ 4

Which Normal Form removes Partial Dependency?

A) 1NF

B) 2NF

C) 3NF

D) BCNF

### Answer

✅ B) 2NF

### Trick

Partial Dependency → 2NF

Transitive Dependency → 3NF

---

## PYQ 5

Which Armstrong Axiom is used?

If:

A → B

Then:

AC → BC

A) Reflexivity

B) Augmentation

C) Transitivity

D) Decomposition

### Answer

✅ B) Augmentation

### Trick

Add same attribute on both sides.

A → B

AC → BC

---

## PYQ 6

Given:

A → B

B → C

Then:

A → C

This property is called:

A) Reflexivity

B) Augmentation

C) Transitivity

D) Closure

### Answer

✅ C) Transitivity

---

## PYQ 7

Consider:

STUDENT(ID, Name, Email)

Candidate Keys:

ID

Email

If ID is selected as Primary Key, then Email becomes:

A) Foreign Key

B) Alternate Key

C) Composite Key

D) Super Key

### Answer

✅ B) Alternate Key

### Trick

Candidate Key not chosen as Primary Key

= Alternate Key

---

# One-Line Revision

✓ Primary Key → No NULL

✓ Candidate Key → Minimal Super Key

✓ Alternate Key → Unused Candidate Key

✓ Foreign Key → References Primary Key

✓ Partial Dependency → 2NF

✓ Transitive Dependency → 3NF

✓ A → B, B → C ⇒ A → C

✓ Armstrong's Axioms are very important for GATE
