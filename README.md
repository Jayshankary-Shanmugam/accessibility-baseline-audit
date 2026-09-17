# Accessibility Baseline & Repository Architecture Audit

## Overview

This project documents an accessibility audit of a real public-facing service website and provides a maintainable monorepo-style full-stack project foundation.

## Audited Website

**Tamil Nadu e-Sevai Citizen Portal**

## Audit Methods

- Google Chrome Lighthouse Accessibility audit
- Manual keyboard-only navigation
- Tab and Shift + Tab navigation testing

## Lighthouse Result

**Accessibility Score: 70**

## Key Findings

The audit documented five accessibility findings:

1. Insufficient color contrast
2. Positive tabindex values
3. Link without a discernible name
4. Insufficient touch target size or spacing
5. Missing HTML language attribute

## Repository Structure

```text
accessibility-baseline-audit/
├── client/
│ └── README.md
├── server/
│ └── README.md
├── docs/
│ ├── audit-report.md
│ ├── architecture.md
│ └── screenshots/
├── tests/
│ └── README.md
├── README.md
└── .gitignore

Deliverables

Accessibility audit report
Lighthouse evidence screenshots
Keyboard-only navigation test
Repository architecture documentation
Monorepo-style project skeleton

Project Status

This repository provides the foundation for extending the audited service into a maintainable full-stack application.
