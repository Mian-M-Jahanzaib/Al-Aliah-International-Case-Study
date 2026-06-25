# Al Aliah International — Property Management System

> A fully offline-first desktop application built for Al Aliah International, a Dubai-based real estate client, to manage a 31-unit mixed-use building including apartments, offices, and retail units.

**Type:** Client Project (Freelance) · Desktop Application  
**Timeline:** March 2026 – May 2026  
**Role:** Sole Developer — requirements, architecture, design, development, deployment  
**Stack:** Electron.js · React.js · TypeScript · SQLite · Tailwind CSS · Vite

> ⚠️ Source code is private to protect client confidentiality. This repository documents the project scope, architecture, and outcome.

---

## The Problem

The client managed a 31-unit mixed-use property in Dubai with no centralized system — tenant records, contracts, payments, and legal documents were tracked manually. They needed a reliable, secure desktop solution that:

- Worked **completely offline** (no cloud dependency, no subscription)
- Could be used by non-technical staff
- Handled all financial and legal paperwork in one place
- Was portable across machines without data loss

---

## What I Built

A full-featured property management desktop application covering every aspect of the client's daily operations.

### Core Modules

**Dashboard**
- At-a-glance overview of total units, occupied/vacant status, active contracts, and total tenants
- Live alerts for expiring leases, bounced cheques, and pending refunds
- Configurable time-window filters (e.g., leases expiring in next 30 days)

**Unit & Tenant Management**
- Complete unit registry with type classification (apartment, office, retail)
- Tenant profiles with full contact, family, and Emirates ID details
- Unit-to-tenant assignment with occupancy history

**Contract Handling**
- Full contract lifecycle — creation, renewal, closure
- Status tracking with automated state changes
- Filter by unit, tenant, status, and date range

**Financial Ledger**
- Ledger-based rent and payment tracking per unit
- Bounced cheque management with replacement and clearance workflows
- Pending refund tracking with full history log
- Payment schedule generation (12-month breakdown per contract)

**Document Generation (5+ automated modules)**
- Contracts, offer letters, legal notices, handover certificates, and renewal documents
- Real-time document preview before printing
- Auto-populated with tenant and unit data — zero manual entry

**Security & Access Control**
- Password-protected login with hashed credential storage
- Account recovery via unique system-generated code
- Full database export/import with access control maintained across machines

---

## Screenshots

### Dashboard — Live Overview
![Dashboard](./screenshots/dashboard.png)
*Real-time property status: 31 units, 25 occupied, 29 tenants, 25 active contracts. Alerts for expiring leases, bounced cheques, and pending refunds.*

---

## Architecture Decisions

**Why Electron.js?**
The client explicitly required an offline-first solution with no recurring cloud costs. Electron allowed me to deliver a native desktop experience with a familiar web tech stack, while SQLite provided a self-contained, portable database that travels with the application.

**Why offline-first?**
Internet reliability in property management offices can be inconsistent, and the client needed guaranteed uptime for daily operations. A local-first architecture also removed any ongoing infrastructure costs or third-party data dependencies.

**Why TypeScript?**
The application's data model is complex — units, tenants, contracts, and payments are deeply interlinked. TypeScript's type safety significantly reduced runtime errors and made the codebase easier to extend as the client requested new modules throughout development.

---

## Outcome

- Delivered a fully production-ready system managing a live 31-unit property in Dubai
- Reduced manual paperwork through 5+ automated document generation modules
- Client actively uses the system for daily operations including rent tracking, contract management, and document printing
- System extended with new modules post-launch based on ongoing client requests

---

## What I Learned

This was my first fully independent client project — from initial requirements gathering through to production deployment. Key takeaways:

- Real clients come with unstructured requirements. Translating business needs into technical architecture is a skill in itself.
- Offline-first architecture introduces unique challenges around data portability, backup, and access control that cloud-based apps don't face.
- A production system is never "done" — building for extensibility from day one matters.

---

## Related

- [LinkedIn Post — Project Milestone & Lessons Learned](https://www.linkedin.com/posts/mian-m-jahanzaib_softwareengineering-development-freelancing-ugcPost-7460764983811866625-SY6s/?utm_source=share&utm_medium=member_desktop&rcm=ACoAAFj5BbwBwBvyrUEzbEBI-P4N4Yw01NZRONM)
- [Portfolio](https://mian-m-jahanzaib.github.io)
