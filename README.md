# Vibe Coding SOP - Newbie Only
![image](https://github.com/user-attachments/assets/231363f1-e252-43b9-ab73-7c9fe887fc09)

## About This Repository

This repository contains a standard operating procedure (SOP) that I use to build applications using a document-based, AI-driven approach. This method shifts the paradigm from *manual coding* to *AI-driven system development*, where AI is not just an assistant, but an engineering partner capable of reading context, understanding architecture, and executing systems end-to-end.

I am a Master's student in Digital Transformation Intelligence (DTI), applying this approach to real-world systems ranging from ERP, monitoring dashboards, to AI-integrated platforms.

Website: [80xstudio.com](https://80xstudio.com)

Instagram: [@LUCASMEVOYEZ](https://instagram.com/LUCASMEVOYEZ)

LinkedIn: [Muhammad Abiyyu Rahman](www.linkedin.com/in/muhammadabiyyurahman)

---

## Core Concept

Instead of writing code directly, this approach starts by structuring system documents. The AI then reads these documents, understands the full context, and executes the system development based on a predefined protocol.

---

## Document Structure

Each project MUST include the following five files:

**PRD.md** — Product Requirements Document
Defines system goals, problems being solved, user roles, main features, and relevant use cases.

**ARCHITECTURE.md**
Describes the technical system design, including frontend, backend, database, technology stack, data flow, and component integrations.

**AI_RULES.md**
Defines AI behavior within the system, operational constraints, expected output format, and guardrails.

**IMPLEMENTATION_PLAN.md**
Contains task breakdown, execution order, development priorities, as well as timeline and execution strategy.

**PMP.md** — Project Management Protocol
Defines how AI reads and executes the project. This file is universal and reusable across projects.

---

## Usage Guide

### Step 1 — Describe Your App to AI

Start a new session with your AI, then describe the application you want to build as clearly and specifically as possible.

You MUST include:
- Application purpose and core problem
- Target users and roles
- Main features (list them clearly)
- Preferred tech stack (e.g., Next.js, Flutter, Node.js, Supabase, PostgreSQL, etc.)
- System type (web app, mobile app, SaaS, internal tool, etc.)
- Data requirements (what data is stored, processed, or analyzed)
- Key workflows (step-by-step user or system flows)
- Integrations (APIs, third-party services, etc.)
- Constraints (performance, security, offline support, etc.)

Avoid vague descriptions. Be explicit and structured.

Then use the following prompt to generate the four core documents:

```
From this conversation, generate the following files:

PRD.md  
Contains:
- System goals  
- Problems being solved  
- User roles  
- Main features  
- Use cases  

Additional rules:
- Assign a unique Feature ID (F-XXX) for every feature
- Every Feature ID MUST be documented in FEATURE_SPEC.md using this exact format:

  F-XXX Feature Name  

  Description:  
  <non-technical explanation>  

  How it works:  
  <simple system flow>  

  Role:  
  <user/admin/system>  

  Status:  
  <Active / Updated / Deprecated>  

---

ARCHITECTURE.md  
Contains:
- System design (frontend, backend, database)  
- Technology stack  
- Data flow  
- System integrations  

Additional rules:
- Each component MUST reference at least one Feature ID (F-XXX)
- Any structural, logic, or integration change MUST be recorded in CHANGELOG_SYSTEM.md using this exact format:

  [DATE] F-XXX FEATURE_NAME  

  Type: ADD / MODIFY / DELETE  
  Files: <list of affected files>  
  Purpose: <reason for change>  
  Impact: <effect on system behavior>  

---

AI_RULES.md  
Contains:
- AI behavior within the system  
- Constraints  
- Output format  
- Guardrails  

Additional rules:
- AI MUST generate a CHANGELOG_SYSTEM.md entry for every:
  - new feature
  - logic change
  - bug fix affecting behavior

- Each entry MUST follow this exact format:

  [DATE] F-XXX FEATURE_NAME  

  Type: ADD / MODIFY / DELETE  
  Files: <list of affected files>  
  Purpose: <reason for change>  
  Impact: <effect on system behavior>  

- AI MUST update FEATURE_SPEC.md if the change:
  - introduces a new feature
  - modifies feature behavior

- FEATURE_SPEC.md MUST follow this exact format:

  F-XXX Feature Name  

  Description:  
  <non-technical explanation>  

  How it works:  
  <simple system flow>  

  Role:  
  <user/admin/system>  

  Status:  
  <Active / Updated / Deprecated>  

- AI MUST reject completion if:
  - CHANGELOG_SYSTEM.md is not updated
  - FEATURE_SPEC.md is missing or inconsistent

---

IMPLEMENTATION_PLAN.md  
Contains:
- Task breakdown  
- Execution order  
- Development priorities  
- Timeline and execution strategy  

Additional rules:
- Every task MUST include:
  - Feature ID (F-XXX)

- Every task MUST enforce this workflow:

  1. Implement code  
  2. Update CHANGELOG_SYSTEM.md (required format)  
  3. Update FEATURE_SPEC.md (if feature is affected)  

- A task is NOT considered DONE unless:
  - CHANGELOG_SYSTEM.md entry exists and is valid
  - FEATURE_SPEC.md reflects the latest feature state
```

---

### Step 2 — Save the Files

Copy the AI output and save each file as:

* `PRD.md`
* `ARCHITECTURE.md`
* `AI_RULES.md`
* `IMPLEMENTATION_PLAN.md`

---

### Step 3 — Prepare Project Folder

Create a project folder and place all four files along with `PMP.md` from this repository.

---

### Step 4 — Run AI via CLI

Call your AI through a CLI interface, then instruct it to read all `.md` files and follow the protocol defined in `PMP.md`.

---

## Benefits of This Approach

This document-driven approach is designed to:

* Improve consistency and structure in system development
* Reduce trial-and-error through explicit planning
* Position AI as an engineering partner, not just a tool
* Produce systems that are traceable, auditable, and scalable

---

## License

This repository is open for reference and adaptation. Attribution is appreciated but not required.
