# Keys and Functional Dependency

## What is a Key?

A key is an attribute or set of attributes used to uniquely identify a tuple (row) in a relation (table).

---

# Types of Keys

## 1. Super Key

A set of one or more attributes that can uniquely identify a tuple.

### Example

STUDENT(ID, Name, Email)

Super Keys:

* ID
* Email
* {ID, Name}
* {ID, Email}

---

## 2. Candidate Key

A minimal Super Key.

### Example

STUDENT(ID, Name, Email)

Candidate Keys:

* ID
* Email

---

## 3. Primary Key

The Candidate Key selected to uniquely identify tuples.

### Example

Primary Key = ID

Properties:

* Unique
* Not Null

---

## 4. Alternate Key

Candidate Keys not selected as Primary Key.

### Example

Primary Key = ID

Alternate Key = Email

---

## 5. Composite Key

A key consisting of more than one attribute.

### Example

ENROLLMENT(StudentID, CourseID)

Primary Key:

(StudentID, CourseID)

---

## 6. Foreign Key

An attribute in one table that refers to the Primary Key of another table.

### Example

STUDENT(StudentID)

ENROLLMENT(StudentID)

StudentID in ENROLLMENT is a Foreign Key.

---

# Functional Dependency (FD)

Functional Dependency describes the relationship between attributes.

Notation:

A → B

Meaning:

If A is known, then B can be uniquely determined.

---

## Example

STUDENT(ID, Name, Department)

ID → Name

ID → Department

This means:

For each ID there is exactly one Name and one Department.

---

# Types of Functional Dependencies

## 1. Trivial Functional Dependency

A → B

where B is a subset of A.

### Example

{ID, Name} → Name

---

## 2. Non-Trivial Functional Dependency

A → B

where B is not a subset of A.

### Example

ID → Name

---

## 3. Completely Non-Trivial FD

A and B have no common attributes.

### Example

ID → Department

---

# Full Functional Dependency

An attribute depends on the entire key.

### Example

(StudentID, CourseID) → Grade

Grade depends on both StudentID and CourseID.

---

# Partial Dependency

An attribute depends on only part of a composite key.

### Example

(StudentID, CourseID) → StudentName

StudentName depends only on StudentID.

This causes violation of 2NF.

---

# Transitive Dependency

A → B

B → C

Therefore:

A → C

### Example

StudentID → DepartmentID

DepartmentID → DepartmentName

Therefore:

StudentID → DepartmentName

This causes violation of 3NF.

---

# Armstrong's Axioms

## Reflexivity

If B ⊆ A

Then:

A → B

---

## Augmentation

If A → B

Then:

AC → BC

---

## Transitivity

If:

A → B

B → C

Then:

A → C

---

# GATE Important Points

✓ Every Candidate Key is a Super Key

✓ Every Primary Key is a Candidate Key

✓ Every Candidate Key may not be Primary Key

✓ Foreign Key can have duplicate values

✓ Primary Key cannot be NULL

✓ Partial Dependency causes 2NF violation

✓ Transitive Dependency causes 3NF violation

✓ Armstrong's Axioms are frequently asked in GATE

---

# Quick Revision

Super Key → Uniquely identifies tuple

Candidate Key → Minimal Super Key

Primary Key → Selected Candidate Key

Alternate Key → Remaining Candidate Key

Composite Key → Multiple attributes

Foreign Key → References another table

FD → A → B

Partial Dependency → 2NF issue

Transitive Dependency → 3NF issue
