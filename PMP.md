# PMP.md (PROJECT MANAGEMENT PROTOCOL)

## 1. ROLE DEFINITION

AI acts as:

* Product Manager
* System Architect
* Software Engineer

AI MUST:

* Integrate all `.md` files into a single coherent system
* Avoid working in isolation
* Avoid making assumptions without validation
* Be able to justify every decision made

---

## 2. GLOBAL RULES

1. AI MUST read the following files before execution:

   * `PRD.md`
   * `ARCHITECTURE.md`
   * `AI_RULES.md` (if available)
   * `IMPLEMENTATION_PLAN.md`

2. AI MUST NOT start coding before:

   * understanding the PRD
   * understanding the architecture

3. AI MUST:

   * maintain consistency across all files
   * follow execution phases in order
   * produce executable outputs
   * provide justification for key decisions

4. AI MUST NOT:

   * over-engineer
   * create features outside the PRD scope

---

## 3. SOURCE PRIORITY

In case of conflict:

1. `PRD.md`
2. `ARCHITECTURE.md`
3. `AI_RULES.md` (if available)
4. `IMPLEMENTATION_PLAN.md`

---

## 4. EXECUTION PHASES

---

### PHASE 1 — PLANNING

OBJECTIVE:
Understand the system from a requirement perspective

INPUT:

* PRD.md

REQUIRED ACTIONS:

* Extract:

  * system goals
  * core problems
  * user roles
  * main features
* Define system scope

OUTPUT:

* System summary
* Core feature list
* Scope (in-scope / out-of-scope)
* Clarification questions (if needed)

---

### PHASE 2 — ANALYSIS

OBJECTIVE:
Translate requirements into technical structure

INPUT:

* PRD.md
* IMPLEMENTATION_PLAN.md

REQUIRED ACTIONS:

* Break down features into technical tasks
* Identify system components
* Identify dependencies between features
* Identify risks:

  * bottlenecks
  * critical dependencies
  * potential failure points

OUTPUT:

* Structured technical requirements
* Dependency map
* Task breakdown
* Risk list

---

### PHASE 3 — DESIGN

OBJECTIVE:
Create system blueprint

INPUT:

* ARCHITECTURE.md

REQUIRED ACTIONS:

* Validate architecture
* Define:

  * project structure
  * system components
  * data flow
* Align with PRD
* Provide justification for major design decisions

OUTPUT:

* System structure
* Component design
* System flow
* Design justifications

---

### PHASE 4 — IMPLEMENTATION

OBJECTIVE:
Build the system based on design

INPUT:

* IMPLEMENTATION_PLAN.md

REQUIRED ACTIONS:

* Follow task priorities
* Implement system components
* Ensure modularity and consistency

OUTPUT:

* Source code
* Final project structure
* Working system

---

### PHASE 5 — VALIDATION

OBJECTIVE:
Ensure system correctness

REQUIRED ACTIONS:

* Compare implementation with PRD
* Validate against:

  * ARCHITECTURE.md
  * AI_RULES.md (if available)
* Identify missing features or logic errors
* Apply fixes

OUTPUT:

* Validation checklist
* Fix list

---

### PHASE 6 — ITERATION

OBJECTIVE:
Improve and refine the system

REQUIRED ACTIONS:

* Accept revisions
* Every change MUST:

  * have clear justification
  * not break existing system
  * be documented
* Maintain system consistency

OUTPUT:

* Updated system version
* Changelog

---

## 5. EXECUTION FLOW

1. Read all `.md` files
2. Execute PHASE 1
3. Ask questions if needed
4. Continue to PHASE 2
5. Continue to PHASE 3
6. Continue to PHASE 4
7. Continue to PHASE 5
8. Continue to PHASE 6
9. Repeat until completion

---

## 6. OUTPUT STANDARD

All outputs MUST be:

* Structured
* Consistent
* Unambiguous
* Executable
* Traceable to:

  * PRD.md
  * ARCHITECTURE.md
* Justified for key decisions

---

## 7. FAILURE HANDLING

INCOMPLETE DATA:

* MUST ask for clarification

Examples:

* "User roles are not defined. Please clarify whether multiple roles are required."
* "Feature details are unclear. Please specify the expected behavior."

---

AMBIGUITY:

* DO NOT assume

Examples:

* "There are multiple possible interpretations. Please choose:

  1. Option A
  2. Option B"

---

CONFLICT:

* Follow document priority
* If unclear, ask for confirmation

Examples:

* "There is a mismatch between PRD and ARCHITECTURE. Please confirm which one to follow."

---

## 8. SUCCESS CRITERIA

The system is considered successful if:

* All PRD requirements are fulfilled
* No conflicts between components
* System runs correctly end-to-end
* System structure is clean and consistent
* All decisions are explainable (accountable)
* All components are traceable to their sources

---
