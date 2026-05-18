# MIL-STD-498 Project Template

## Quick Start

1. Copy this entire `template/` directory into your new project
2. Rename the copy to your project name
3. Fill out `CDRL.md` to select which DIDs apply to your project
4. Delete any DID document folders/files that do not apply
5. Fill in `[PROJECT NAME]`, `[DATE]`, and other placeholders in each document
6. Follow the workflow in `.windsurf/workflows/mil-std-498.md`

## Directory Structure

```
template/
├── README.md              # This file
├── CDRL.md                # Contract Data Requirements List (DID selection checklist)
├── docs/
│   ├── plans/             # Planning documents
│   │   ├── SDP.md         # Software Development Plan
│   │   ├── SIP.md         # Software Installation Plan
│   │   └── STrP.md        # Software Transition Plan
│   ├── requirements/      # Concept and requirements documents
│   │   ├── OCD.md         # Operational Concept Description
│   │   ├── SSS.md         # System/Subsystem Specification
│   │   ├── SRS.md         # Software Requirements Specification
│   │   └── IRS.md         # Interface Requirements Specification
│   ├── design/            # Design documents
│   │   ├── SSDD.md        # System/Subsystem Design Description
│   │   ├── SDD.md         # Software Design Description
│   │   ├── DBDD.md        # Database Design Description
│   │   └── IDD.md         # Interface Design Description
│   ├── test/              # Test documents
│   │   ├── STP.md         # Software Test Plan
│   │   ├── STD.md         # Software Test Description
│   │   └── STR.md         # Software Test Report
│   ├── manuals/           # User and support manuals
│   │   ├── SUM.md         # Software User Manual
│   │   ├── SIOM.md        # Software Input/Output Manual
│   │   ├── SCOM.md        # Software Center Operator Manual
│   │   ├── COM.md         # Computer Operation Manual
│   │   ├── CPM.md         # Computer Programming Manual
│   │   └── FSM.md         # Firmware Support Manual
│   └── product/           # Software product definition
│       ├── SPS.md         # Software Product Specification
│       └── SVD.md         # Software Version Description
└── src/                   # Source code directory (your code goes here)
```

## How to Use These Templates

Each document template follows the section structure defined by its MIL-STD-498 Data Item Description (DID). Sections contain:

- **Instructional text in italics** explaining what to write
- **Placeholder markers** like `[PROJECT NAME]` to replace with your values
- **Section numbering** matching the official DID structure

### Tailoring

Not every section applies to every project. When a section does not apply:
- Write "Not applicable." in the section body
- Do not delete the section heading (maintain document structure for auditors)

### Minimum Document Set (Small Projects)

For small or low-risk projects, the minimum recommended set is:
- **SDP** - Software Development Plan
- **SRS** - Software Requirements Specification
- **SDD** - Software Design Description
- **STP** - Software Test Plan
- **STD** - Software Test Description
- **STR** - Software Test Report
- **SUM** - Software User Manual
- **SVD** - Software Version Description

### Full Document Set (Large/High-Risk Projects)

Use all 22 DIDs and tailor each one via the CDRL.

## Conventions

- All dates use ISO 8601 format: YYYY-MM-DD
- Version numbers use MAJOR.MINOR format (e.g., 1.0, 1.1, 2.0)
- Requirement IDs use the format: `[PREFIX]-[NUMBER]` (e.g., SRS-001, SSS-042)
- Traceability is maintained through requirement ID cross-references
