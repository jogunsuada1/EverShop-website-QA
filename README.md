# EverShop QA Portfolio Project

End-to-end QA portfolio project built on the [EverShop open-source e-commerce demo platform](https://demo.evershop.io/). Completed as part of **Buildgem Cohort 2**, mentored and reviewed by **Kingsley Udoh**.

## About

This project demonstrates full-cycle QA competency — from planning to automation to reporting — against a live demo e-commerce application (storefront + admin panel).

## Project Phases

1. **Test Planning** — PRD review and System Test Plan
2. **Manual Testing** — 119 test cases across 9 functional areas
3. **API Testing** — Postman collection + dedicated API Test Strategy Document
4. **E2E Automation** — Playwright test suite (JavaScript)
5. **Defect Reporting** — Bug Report and Final Test Summary Report

## Repo Structure

```
├── docs/
│   ├── PRD.docx
│   ├── System_Test_Plan.docx
│   ├── API_Test_Strategy.docx
│   ├── Bug_Report.docx
│   └── Test_Summary_Report.docx
├── postman/
│   └── evershop-api-collection.json
├── tests/
│   └── *.spec.js
├── playwright.config.js
└── README.md
```

## Tech Stack

- **Playwright** (JavaScript) — E2E automation
- **Postman** — API testing
- **EverShop Demo** — [demo.evershop.io](https://demo.evershop.io/) (system under test)

## Running the Tests

```bash
npm install
npx playwright test
```

Report:
```bash
npx playwright show-report
```

## Key QA Principles Followed

- Dynamic waits only (`toBeVisible()`, `waitForLoadState()`, etc.) — no fixed `waitForTimeout()`
- Case-insensitive regex locators for cross-browser stability
- Single `playwright.config.js`; specs isolated under `/tests`

## Deliverables

- Product Requirements Document (PRD)
- System Test Plan
- API Test Strategy Document
- Postman Collection
- Playwright E2E Automation Suite
- Bug Report
- Final Test Summary Report

## Author

**Ogunsuada Joseph** — QA Engineer, Buildgem Cohort 2
