
# Wesal (وصال) — Graduation Research Workspace

> **A unified digital workspace designed to guide health science students from research idea to final submission.**

[![Hackathon](https://img.shields.io/badge/SSCP-Hackathon-7C4DFF)](https://github.com/)
[![Status](https://img.shields.io/badge/Status-Functional%20Prototype-success)](https://github.com/)

---

## Overview

**Wesal** is a unified digital workspace designed to connect **students, supervisors, and institutional requirements** in one structured research workflow.

Instead of relying on fragmented channels such as **email, WhatsApp, and manual spreadsheets**, Wesal provides an end-to-end platform for:

- Research idea registration
- Supervisor discovery and matching
- Research milestone tracking
- Cross-college co-supervision
- Contextual communication and task management
- Institutional research governance

Wesal was developed for the **SSCP Hackathon** to demonstrate the institutional feasibility and technical architecture of a structured graduation research workflow for health science faculties.

---

## The Problem

Graduation research can become difficult to manage when communication, supervision, documents, and academic requirements are spread across multiple tools.

Students may struggle to:

- Find a suitable supervisor
- Understand research requirements
- Track their progress
- Communicate effectively with supervisors
- Collaborate with experts from other colleges

At the institutional level, coordinators and faculty members also need better visibility into research progress, delays, and inactive projects.

**Wesal brings the entire journey into one workspace.**

---

## Key Features

### 1. Instant Verification & Idea Registration

Wesal automatically creates a unique project record such as:

`WESAL-2026-XXXX`

Each project record includes a timestamp and a **SHA-256 cryptographic hash** to document the registration event and help prevent duplicate research topics within departments.

---

### 2. Rule-Based Compatibility Matching

Our matching engine compares:

- Student research interests
- Study methodology
- Clinical specialty
- Faculty expertise
- Current supervision capacity

This helps students discover supervisors who are a better fit for their research needs.

---

### 3. Five-Stage Research Journey

Wesal organizes the research process into five main stages:

```text
Research Idea
     ↓
Proposal
     ↓
IRB Approval
     ↓
Data Collection
     ↓
Analysis
     ↓
Final Submission
````

Students and supervisors can track progress throughout the journey.

---

### 4. Cross-College Co-Supervision

Wesal supports collaboration across health science colleges.

For example, a pharmacy research project can formally request a co-supervisor from:

* Medicine
* Nursing
* Dentistry
* Public Health

Both supervisors and the student can work within the **same research workspace**.

---

### 5. Contextual Communication & Tasks

Each research project includes tools for:

* Task management
* Supervisor feedback
* File versioning
* Review queues
* Research-specific communication

This keeps important discussions and actions connected to the research project itself.

---

### 6. Governance & Early Alerts

Wesal provides an institutional dashboard for deans and research coordinators to monitor:

* Project progress
* Project health
* Inactive workflows
* IRB delays
* Research activity across departments

This gives institutions better visibility into the overall research pipeline.

---

## AI Research Support

Wesal is designed to include an AI-powered **Research Copilot** to support students and supervisors throughout the research journey.

The AI layer is intended to help with:

* Identifying missing requirements
* Reviewing research drafts
* Highlighting important ethics or submission requirements
* Generating quick summaries for supervisors

We are also working toward structuring a **dedicated AI layer for the Wesal research workflow**, tailored specifically to academic and health research requirements.

---

## Product Architecture

Wesal was designed as a **modular platform**, allowing institutions to adapt workflows and requirements based on their own academic policies.

The architecture also supports future expansion across multiple colleges and institutions.

### Main Roles

```text
Student
   │
   ├── Research Idea
   ├── Supervisor Matching
   ├── Research Workspace
   └── Progress Tracking
   │
Supervisor
   │
   ├── Research Review
   ├── Feedback
   ├── Tasks
   └── Co-Supervision
   │
Institution
   │
   ├── Governance Dashboard
   ├── Progress Monitoring
   └── Early Alerts
```

---

## Tech Stack

### Frontend

* Next.js
* React
* Tailwind CSS
* Shadcn UI
* Lucide Icons

### Backend

* Node.js
* FastAPI

### Database & Architecture

* PostgreSQL
* Modular Component Architecture

### Security & Verification

* SHA-256 cryptographic hashing
* Timestamped project registration

---

## Project Structure

```text
wesal-platform/
├── app/
│   ├── auth/            # Role-based onboarding & sign-in
│   ├── student/         # Student research wizard & dashboard
│   ├── faculty/         # Supervisor workspace & review queue
│   └── admin/           # Governance & institutional network
│
├── components/
│   ├── wizard/          # Multi-step taxonomy matching form
│   ├── workspace/       # Milestone pipeline & task checklist
│   └── ui/              # Buttons, badges, modals, dialogs
│
├── lib/
│   ├── sha256.ts        # Record hashing & timestamp utilities
│   └── taxonomy.ts      # Pharmacy & health science tag structures
│
└── public/              # Static assets & brand logos
```

---

## Getting Started

### Prerequisites

Make sure you have:

* Node.js `18.x` or later
* npm, pnpm, or yarn

### Installation

Clone the repository:

```bash
git clone https://github.com/your-username/wesal-platform.git
cd wesal-platform
```

Install dependencies:

```bash
npm install
```

Run the development server:

```bash
npm run dev
```

Open:

```text
http://localhost:3000
```

---

## Prototype

Wesal is currently available as a **functional prototype** demonstrating the core research workflow and platform architecture.

The prototype focuses on validating the main user journey:

```text
Research Idea → Supervisor Matching → Research Workspace
→ Progress Tracking → Final Submission
```

---

## Roadmap

### Phase 1 — Functional Prototype

* Core research workflow
* Student and supervisor interfaces
* Research project registration
* Supervisor matching

### Phase 2 — Pilot

* Pilot deployment at a local university
* Real-world workflow testing
* User feedback and iteration
* Validation of supervisor matching speed

### Phase 3 — AI & Optimization

* Dedicated AI research layer
* Smarter research assistance
* Automated requirement checks
* Improved matching and recommendation models

### Phase 4 — Expansion

* Cross-college collaboration
* Multi-university support
* Expansion across Saudi Arabia
* Future GCC expansion

---

## Validation

Wesal has been presented to **Dr. Khalid Al-Amer**, Head of the Clinical Trials Unit at the Medical Sciences Research Center, who reviewed the concept and prototype and strongly supported the need for a solution like Wesal.

---

## Business Model

Wesal follows an **institutional subscription model** designed for universities and colleges.

The platform is intended to help institutions:

* Reduce administrative overhead
* Improve research coordination
* Increase visibility across research projects
* Improve communication between students and supervisors
* Support cross-disciplinary collaboration

---

## Team

### Jumana Ali Alaseel

**Founder & Project Lead**

Product • Clinical Research • Strategy

### Joud Balkhair

**Co-Founder & Full-Stack Developer**

Platform Architecture • Cryptographic Integrations

### Maryam Almayouf

**Co-Founder & Business Lead**

Business Model • Financial Logic

---

## Built for the SSCP Hackathon

Wesal was developed as part of the **SSCP Hackathon**, with the goal of improving the graduation research experience across health science faculties.

> **One journey. One workspace. Wesal.**

---

## License

This project is currently a hackathon prototype.

All rights reserved unless otherwise stated.

```

