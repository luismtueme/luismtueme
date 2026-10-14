# Luis Morales Tueme

Test automation. I publish frameworks a team can clone and point at their own application, and a tool for reading the same test run in more than one report.

## Frameworks

One design, six stacks. Start with [playwright-typescript-framework](https://github.com/luismtueme/playwright-typescript-framework) unless the team needs Gherkin, Python, Java, or mobile.

| Repository | Tests are written as | Language | Choose it when |
| --- | --- | --- | --- |
| [playwright-typescript-framework](https://github.com/luismtueme/playwright-typescript-framework) | Playwright specs | TypeScript | Engineers write and read the tests. The most features and the simplest toolchain |
| [playwright-cucumber-typescript-framework](https://github.com/luismtueme/playwright-cucumber-typescript-framework) | Gherkin scenarios and Playwright specs | TypeScript | Product owners, analysts, or manual QA read or write scenarios in Given/When/Then |
| [playwright-cucumber-automation-framework](https://github.com/luismtueme/playwright-cucumber-automation-framework) | Gherkin scenarios and Playwright specs | JavaScript | Cucumber without a TypeScript toolchain |
| [playwright-python-framework](https://github.com/luismtueme/playwright-python-framework) | Pytest | Python | The same Playwright checks, without Node |
| [selenium-java-cucumber-framework](https://github.com/luismtueme/selenium-java-cucumber-framework) | Gherkin scenarios | Java | The team works in Java, or needs Selenium Grid or WebDriver-based tooling |
| [appium-java-cucumber-framework](https://github.com/luismtueme/appium-java-cucumber-framework) | Gherkin scenarios and JUnit specs | Java | Native Android and iOS |

Each repo includes a demo app so the suite passes out of the box, GitHub Actions, and an MIT license. The TypeScript framework covers UI, API, database, accessibility, and visual checks, with role-based users and Allure reporting.

Live reports:

- [Allure report](https://luismtueme.github.io/playwright-typescript-framework/allure-report/) for the TypeScript Playwright framework
- [Cucumber report](https://luismtueme.github.io/selenium-java-cucumber-framework/) for the Selenium Java framework

## ReportBridge

[report-bridge](https://github.com/luismtueme/report-bridge) imports one test run into a shared intermediate representation and previews it as Cucumber-style, Allure-like, and Extent-like reports. Importers cover Cucumber JSON, Allure results, JUnit XML, TestNG XML, Playwright JSON, Jest JSON, and pytest JSON.
