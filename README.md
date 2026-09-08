# VisaGuardian AI

VisaGuardian AI (`x_snc_visaguardi_0`) is an enterprise case management platform for international student services on ServiceNow, built to streamline visa advising, document verification, and compliance monitoring.

## Project Overview

- **Application Name:** VisaGuardian AI
- **Scope:** `x_snc_visaguardi_0`
- **Application Type:** Scoped ServiceNow application
- **Primary Domain:** International student visa case operations

## Core Features

### 1) Advisor Workspace
- Tailored advisor experience built for ServiceNow Next Experience / workspace-driven operations.
- Centralized case handling for advisor queues, student risk visibility, and advisory actions.

### 2) Intelligent Workflows & Automation
Includes Flow Designer and action-driven automation for advisory lifecycle execution:

- **Advisor Decision Notification Flow**
- **Advisor Review Workflow**
- **Get Current Student Risk Assessment**
- **Get Current Student Documents**
- **Get Current Student Context**

These automations support guided review, decisioning, contextual retrieval, and communication to keep cases moving with consistent process controls.

### 3) Data Model & Architecture
Custom data model entities include:

- **Visa Cases** (`x_snc_visaguardi_0_visa_case`)
- **Advisor Profiles** (`x_snc_visaguardi_0_advisor_profiles`)
- **Student Notifications** (`x_snc_visaguardi_0_student_notifications`)
- **Request Type Configuration** (`x_snc_visaguardi_0_request_type_configuration`)
- **Document Configuration** (`x_snc_visaguardi_0_document_configuration`)

Supporting tables in the app also include student profile, visa document, and risk assessment records to power end-to-end case workflows.

### 4) Compliance & Role-Based Access
- Granular ACL definitions and role bindings are included for advisor/student personas.
- Security controls are scoped to application data and workspace access patterns for regulated case operations.

## Repository & Tech Stack

- **Platform:** ServiceNow (Xanadu / Washington release family)
- **Architecture:** Scoped application metadata package
- **Source Format:** ServiceNow XML payload metadata and dictionary definitions
- **Source Control Model:** Native ServiceNow Studio Git integration (including update artifacts and application metadata)

## PDI Installation & Setup Guide

### Prerequisites
- ServiceNow Personal Developer Instance (PDI)
- Admin access to the instance
- Access to this repository URL

### Import from Source Control
1. Log in to your PDI.
2. Open **ServiceNow Studio**.
3. Select **Import From Source Control**.
4. Paste the repository HTTPS URL.
5. Provide/select your source control credentials.
6. Choose the **main** branch.
7. Complete the import.

### Post-Import Validation
1. Confirm the application scope is **`x_snc_visaguardi_0`**.
2. Open **Advisor Workspace** and verify workspace pages load correctly.
3. Open Flow Designer and ensure the listed flows/actions are available and activated as needed.

## Visuals

### Architecture Diagram
![Architecture Diagram Placeholder](docs/images/architecture-diagram-placeholder.png)

### Advisor Workspace Interface
![Advisor Workspace Interface Placeholder](docs/images/advisor-workspace-placeholder.png)

### Flow Designer Logic
![Flow Designer Logic Placeholder](docs/images/flow-designer-placeholder.png)

## Notes for Evaluators

- This repository follows ServiceNow application source export conventions, where configuration and logic are represented as metadata XML records.
- If importing into a clean PDI for evaluation, ensure required dependencies in the packaged app metadata are available before activation.
