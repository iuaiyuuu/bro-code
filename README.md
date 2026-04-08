# Vibe Coding SOP - Newbie Only

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

Start a new session with your AI, then describe the application you want to build. Use the following prompt to generate the four core documents:

```
From this conversation, generate the following files:

PRD.md  
Contains:
- System goals  
- Problems being solved  
- User roles  
- Main features  
- Use cases  

ARCHITECTURE.md  
Contains:
- System design (frontend, backend, database)  
- Technology stack  
- Data flow  
- System integrations  

AI_RULES.md  
Contains:
- AI behavior within the system  
- Constraints  
- Output format  
- Guardrails  

IMPLEMENTATION_PLAN.md  
Contains:
- Task breakdown  
- Execution order  
- Development priorities  
- Timeline and execution strategy  
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
