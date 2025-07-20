
# 🧪 OrangeHRM Playwright E2E Test Suite

![E2E Tests](https://github.com/kobenguyent/OrangeHRM-PlayTest/actions/workflows/e2e.tests.yml/badge.svg)
[![Allure Report](https://img.shields.io/badge/Allure--Report-View-blue?logo=allure)](https://kobenguyent.github.io/OrangeHRM-PlayTest)
[![Qase Test Run](https://img.shields.io/badge/Qase-Test%20Run-blue?logo=data:image/png;base64,iVBORw0KGgo)](https://app.qase.io/public/report/adb5c9b45d87cc8e250b235c88383fbbf92781ac)

End-to-end test automation for [OrangeHRM](https://opensource-demo.orangehrmlive.com/) using [Playwright](https://playwright.dev/).

This project follows the **Page Object Model** structure and uses **Playwright Test Runner** along with **Allure Reports** for detailed test reporting.

---

## 📁 Project Structure
```
OrangeHRM-PlayTest/
├── tests/                  # Test specs (with subfolders like login, search, etc.)
├── pages/                  # Page Object Models
├── fixtures/               # Test data
├── playwright.config.ts    # Playwright configuration
├── .github/workflows/      # GitHub Actions CI setup
└── …
```
---

## 🚀 Getting Started

### Install dependencies

```bash
npm install

Run tests locally

npx playwright test

Run tests with Allure report

npx playwright test --reporter=line,allure-playwright

Then generate and open the Allure report:

npx allure generate ./allure-results --clean -o ./allure-report
npx allure open ./allure-report
```

⸻

📊 Allure Report (Hosted)

View the latest test results here:
🔗 [Allure Report](https://kobenguyent.github.io/OrangeHRM-PlayTest)

⸻

🔄 Continuous Integration

This project uses GitHub Actions to run tests on every push to main and generate Allure reports.

The CI workflow:

	•	Installs dependencies
	•	Runs all Playwright tests
	•	Publishes Allure report to the gh-pages branch

See the workflow file in 
.github/workflows/e2e.tests.yml.

⸻

🧩 Technologies Used

	•	🎭 Playwrigh
	•	🧪 Playwright Test Runner
	•	🧱 Page Object Model
	•	📊 Allure Reports
	•	⚙️ GitHub Actions

⸻

📌 Todo

	•	Add more coverage for other modules
	•	Integrate with a test data service or API mocks
	•	Improve cross-browser test matrix

⸻

📄 License

MIT © kobenguyent