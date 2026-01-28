## Experiment 1: Database using DDL, DML, and DCL (PostgreSQL)

**Student Name:** Gaurang Garg

**UID:** 25MCI10179

**Branch:** MCA (AI/ML)

**Section:** 25MAM-1A

**Semester:** II

**Subject:** Technical Training (25CAP-652)

**Date:** 05-01-2026

---

## Aim

To design and implement a sample database system using DDL, DML, and DCL commands with role-based access control.

## Objectives

* Practice DDL commands (CREATE, ALTER, DROP).
* Practice DML commands (INSERT, UPDATE, DELETE).
* Practice DCL commands (CREATE ROLE, GRANT, REVOKE).
* Understand constraints and secure read-only access.

## Database Used

* **PostgreSQL**

## Tables Created

1. **department**

   * department_id (PK)
   * department_name (UNIQUE, NOT NULL)
   * salary (CHECK salary >= 0)

2. **employee**

   * employee_id (PK)
   * employee_name (NOT NULL)
   * department_id (FK)
   * employee_contact
   * join_date
   * end_date (CHECK end_date >= join_date)
   * status (DEFAULT 'active')

3. **project**

   * project_id (PK)
   * project_name (UNIQUE, NOT NULL)
   * department_id (FK)
   * start_date
   * end_date (CHECK end_date >= start_date)

## Operations Performed

* Created tables with constraints (DDL).
* Inserted, updated, and deleted records (DML).
* Retrieved data using SELECT (DQL).
* Created a role and managed permissions (DCL).

## Role-Based Access

* Created role **reporting_user**.
* Granted SELECT permission on required tables.
* Revoked unnecessary permissions for security.

## Output

* Data displayed successfully using SELECT queries.
* Role-based access worked as expected.

## Learning Outcomes

* Learned PostgreSQL query writing.
* Understood DDL, DML, DCL commands.
* Used CHECK constraints correctly.
* Implemented role-based database security.

---

*This README describes the database experiment implementation and outcomes.*

