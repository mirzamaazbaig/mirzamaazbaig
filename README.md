# Mirza Maaz Baig

**Senior Automation Engineer (SDET)** · ISTQB® CTFL & CTAL-TAE · Milan, Italy

4+ years in test automation for web products and Node.js APIs. I decide what to automate and why (risk first), build maintainable Playwright, Cypress and Selenium frameworks, and run them in CI so results are reproducible. I also work with LLMs (RAG, agents) and apply them to QA.

Currently Senior Automation Engineer at CoreView. Earlier: Kantar XTEL, Xcelliti (core banking).

## Featured project

### [ecommerce-test-automation: E2E, API and accessibility tests for a full-stack shop](https://github.com/mirzamaazbaig/ecommerce-test-automation)

A React, Express and PostgreSQL application used as the system under test for a three-layer Playwright suite.

- **141 automated tests:** 59 UI end-to-end tests (page objects, including the admin dashboard), 66 API tests and 16 accessibility checks (axe-core, WCAG 2.1 AA). The UI tests run on desktop and at phone size in Chromium, and in Firefox and WebKit; everything runs on every push in GitHub Actions against a PostgreSQL service container, and the HTML report is published as a build artifact.
- **API testing:** authentication and session handling, role-based access control, input handling including SQL injection attempts, order transactions (all-or-nothing, stock rules, concurrent orders), and SQL checks on the persisted rows.
- **Defects found, reported and fixed:** six functional defects written up with requests, expected and actual behaviour in [`docs/KNOWN_DEFECTS.md`](https://github.com/mirzamaazbaig/ecommerce-test-automation/blob/HEAD/docs/KNOWN_DEFECTS.md). I then fixed all six (starting with orders that exceeded stock and client-controlled prices), each time proving the new test failed on the old code and passes on the fix.
- **Accessibility:** the first axe-core scan failed on all 11 customer pages (unlabeled form controls, low-contrast buttons) and later found a nearly invisible admin tab (white text on light grey). Running the UI tests at phone size then found three more defects (filters hidden on phones, admin buttons overlapped, an unlabeled menu button). I fixed the markup and styles and the scans now pass. A written [test strategy](https://github.com/mirzamaazbaig/ecommerce-test-automation/blob/HEAD/docs/TEST_STRATEGY.md) ties the tests to product risks.
- **Maintainable test design:** page objects, isolated test data per test, fixtures that sign in through the API, web-first assertions with no fixed sleeps, and UI results cross-checked against the API. I hunted down flaky tests (animations measured mid-fade, stale lists, order-dependent data) instead of retrying them.

## More test projects

All of them test the same shop (React, Express, PostgreSQL), each with a different tool or layer, and each runs in GitHub Actions.

| Project | What it shows |
|---|---|
| [ecommerce-ui-selenium-testng](https://github.com/mirzamaazbaig/ecommerce-ui-selenium-testng) | Java, Selenium and TestNG: page objects, parallel runs, explicit waits only |
| [ecommerce-ui-bdd-cucumber](https://github.com/mirzamaazbaig/ecommerce-ui-bdd-cucumber) | Gherkin scenarios driven by Playwright and TypeScript |
| [ecommerce-api-postman-newman](https://github.com/mirzamaazbaig/ecommerce-api-postman-newman) | Postman collections run with Newman, including data-driven runs |
| [ecommerce-api-pytest](https://github.com/mirzamaazbaig/ecommerce-api-pytest) | Python and pytest API framework with schema and security checks |
| [ecommerce-db-pytest](https://github.com/mirzamaazbaig/ecommerce-db-pytest) | PostgreSQL schema, constraint, data-integrity and migration tests |
| [ecommerce-performance-locust](https://github.com/mirzamaazbaig/ecommerce-performance-locust) | Locust load tests that fail the build when latency or error thresholds are missed |
| [ecommerce-qa-documentation](https://github.com/mirzamaazbaig/ecommerce-qa-documentation) | Test plan, risk register, requirements and a generated traceability matrix |

## Skills

| Area | What I use |
|---|---|
| Test automation | Playwright (UI and API), Cypress, Selenium WebDriver, Cucumber (BDD), Mocha, Jest |
| Test design | Risk-based test strategy, testability analysis, test data management, negative and boundary cases, defect reporting |
| API and database | REST, gRPC, Postman, SQL verification |
| CI/CD | GitHub Actions, Azure DevOps, Jenkins |
| Languages | TypeScript, JavaScript (Node.js), Python, SQL |
| Tools | Git and GitHub, JIRA, TestRail, Allure, Extent Reports |
| AI for QA | RAG, LangChain, Chroma, prompt engineering, LLM output evaluation |

## Education and certifications

- M.Sc. Electrical and Electronics Engineering, Università di Bologna (2018 to 2022); B.Sc. Electrical and Power Engineering, Usman Institute of Technology (2013 to 2017)
- ISTQB Certified Tester Advanced Level, Test Automation Engineering (CTAL-TAE), Dec 2025
- ISTQB Certified Tester Foundation Level (CTFL), Dec 2025

## Contact

- LinkedIn: [linkedin.com/in/mirzamaazbaig](https://www.linkedin.com/in/mirzamaazbaig)
- Email: engr.mirzamaaz@gmail.com
