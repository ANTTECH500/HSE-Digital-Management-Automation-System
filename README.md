# HSE-Digital-Management-Automation-System
Integrated HSE management and workflow automation system built with Google Apps Script, Google Sheets and Smartsheet API.

# HSE Digital Management & Automation System

## Overview

The HSE Digital Management & Automation System is an integrated
Google Apps Script and Google Sheets-based solution designed to
automate HSE data management, Corrective and Preventive Action (CAPA)
tracking, departmental workflows, data integration, and record
synchronization.

The system integrates multiple automation modules into a centralized
HSE digital workflow, reducing manual data entry and improving the
accessibility, consistency, and management of operational records.

---

## System Modules

### 1. Smartsheet Integration

**Repository Module:** `smartsheet-google-sheets-integration`

Automates the transfer of data from Smartsheet into Google Sheets
using the Smartsheet API and Google Apps Script.

#### Key Features
- Smartsheet API integration
- Automated data retrieval
- Google Sheets data population
- Automatic header formatting
- Automatic column resizing
- Frozen header rows
- Import status notifications
- Error handling
- Manual and trigger-based execution

---

### 2. CAPA Automation

**Repository Module:** `hse-capa-management-automation`

Automates the management and notification workflow for Corrective
and Preventive Actions (CAPA).

#### Key Features
- CAPA record management
- Responsible-person identification
- Priority management
- Due-date tracking
- Automated email notifications
- CAPA confirmation workflow
- Overdue action highlighting
- HTML-formatted notifications
- HSE action follow-up

---

### 3. CAPA Search

**Repository Module:** `hse-capa-search-system`

Provides a department-based search interface for retrieving and
reviewing CAPA records from a centralized backend database.

#### Key Features
- Department-based searching
- Backend CAPA database
- Dynamic result display
- Search result counting
- Custom Google Sheets menu
- Automated column resizing
- Department-specific CAPA retrieval

---

### 4. Department Navigation

**Repository Module:** `hse-department-navigation`

Provides a centralized navigation interface for accessing
department-specific worksheets stored within an external Google
Sheets workbook.

#### Key Features
- Department dropdown selection
- Centralized spreadsheet access
- Automatic worksheet identification
- External spreadsheet navigation
- Department validation
- Custom user interface

#### Supported Departments

- Administration
- RO250 & RO500
- HSE
- Laboratory
- Procurement
- Planning
- Pompora
- STP
- AWTP
- NWTP
- Electrical & Instrumentation
- Mechanical

---

### 5. CAPA Library

**Repository Module:** `capa-data-entry-automation`

Provides a standardized CAPA data-entry structure for recording HSE
corrective and preventive actions.

#### Standard CAPA Fields

- Identify Date
- Site
- Source of Issue
- Deviation Description
- Preventive Action
- Issue Focus Area
- Type
- Priority
- Responsible Person

#### Key Features
- Automated CAPA template creation
- Standardized data fields
- Automatic header formatting
- Prepared data-entry row
- Custom CAPA Tools menu
- Structured data-entry workflow

---

### 6. CAPA Synchronization

**Repository Module:** `capa-google-sheets-sync`

Synchronizes CAPA records between separate Google Sheets to maintain
consistent records across different HSE workbooks.

#### Key Features
- Cross-spreadsheet synchronization
- Automatic row insertion
- Existing-record updates
- Edit detection
- Target worksheet validation
- Automated data transfer

---

# System Architecture

The overall workflow can be represented as:

Smartsheet
    |
    | API Integration
    v
Google Apps Script
    |
    v
Google Sheets
    |
    +----------------------+
    |                      |
    v                      v
CAPA Library         Department Data
    |                      |
    v                      v
CAPA Automation      Department Navigation
    |
    +----------------------+
    |
    v
CAPA Search
    |
    v
Reporting / Review

CAPA Records
    |
    v
CAPA Synchronization
    |
    v
Central / Secondary HSE Sheets

---

# Core Technologies

- Google Apps Script
- JavaScript
- Google Sheets
- Smartsheet API
- Google Workspace
- HTML
- Spreadsheet automation
- API integration
- Event-driven triggers

---

# Functional Areas

## HSE Management

The system supports:

- Corrective and Preventive Actions
- HSE action tracking
- Responsible-person assignment
- Priority management
- Due-date management
- CAPA notifications
- Departmental HSE records

## Data Management

The system provides:

- Automated data import
- Structured data entry
- Data synchronization
- Department-based searching
- Centralized record access
- Automated spreadsheet updates

## Workflow Automation

Automation is used to:

- Retrieve external data
- Create and format records
- Notify responsible personnel
- Search departmental records
- Synchronize information
- Navigate between departmental workbooks

---

# Project Objectives

The primary objectives of the system are to:

1. Reduce manual HSE data entry.
2. Improve CAPA tracking and follow-up.
3. Standardize HSE record structures.
4. Improve accessibility of departmental records.
5. Automate communication and notifications.
6. Synchronize information between spreadsheets.
7. Improve the efficiency of HSE data management.
8. Provide a foundation for further HSE digital transformation.

---

# Project Structure

```text
hse-digital-management-automation/
│
├── smartsheet-integration/
│   └── Smartsheet API → Google Sheets
│
├── capa-automation/
│   └── CAPA notification and workflow automation
│
├── capa-search/
│   └── Department-based CAPA search
│
├── department-navigation/
│   └── Department spreadsheet navigation
│
├── capa-library/
│   └── Standardized CAPA data entry
│
├── capa-sync/
│   └── Cross-spreadsheet CAPA synchronization
│
└── README.md
