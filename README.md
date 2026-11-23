# Support Operations Toolkit

A Persian, right-to-left web toolkit for streamlining repetitive support workflows, preparing standardized reports, and handling common operational tasks from a single interface.

Overview

Support Operations Toolkit brings frequently used support utilities together in one lightweight web application. It is designed around practical workflows: entering case details, generating consistent report text, converting numbers and keyboard-layout text, and keeping a simple count of incoming and outgoing calls.

The public release is a standalone frontend application. Organization-specific names, staff handles, internal destinations, and provider-specific API integrations have been removed or generalized.

Features

- Number conversion: Persian digits to English digits and English digits to Persian digits.
- Keyboard-layout conversion: Convert text typed with the wrong keyboard layout into Persian text.
- Transaction referral report: Build a structured referral message from transaction and customer details.
- Issue reporting: Prepare consistent incident and issue reports.
- Bank-document requests: Collect the details needed to prepare a bank-document request.
- Deposit and withdrawal templates: Generate structured templates for fiat and crypto-related support cases.
- Crypto recovery and empty-hash reports: Prepare repeatable report text for common crypto support scenarios.
- Withdrawal-cycle message builder: Generate customer-facing messages based on the selected processing scenario.
- Call counter: Track incoming and outgoing calls, with counts saved locally in the browser.
- Traffic correction form: Prepare a structured request using a selected date, time, and reason.
- Theme preference: Switch between the available themes; the preference is saved locally.
- Copy-to-clipboard actions: Copy generated reports for use in the team's chosen support system.

Technology

- HTML5
- CSS3
- Vanilla JavaScript
- Browser Clipboard API with a fallback for supported browsers
- "localStorage" for theme preference and call-counter values
- Font Awesome icons loaded from cdnjs (internet connection required for icons)

No framework, build step, package manager, backend, or database is required. Font Awesome is loaded from a public CDN for interface icons; the core tools remain usable if the icon CDN is unavailable.

Run locally

1. Download or clone this repository.
2. Open "index.html" in a modern browser.
3. Start using the tools. No installation or build command is needed.

For the best experience, use a current version of Chrome, Edge, Firefox, or Safari. Clipboard access may require a secure context (HTTPS or localhost) in some browsers.

Deploy with GitHub Pages

1. Push this repository to GitHub.
2. Open the repository's Settings → Pages.
3. Under Build and deployment, select Deploy from a branch.
4. Choose the "main" branch and the "/ (root)" folder, then save.
5. Wait for GitHub Pages to publish the site. The public URL will appear in the Pages settings.

Because the entry file is named "index.html", GitHub Pages can serve the application directly from the repository root.

Data handling and privacy

- The application has no backend and does not submit form contents to a server.
- Generated report text is copied to the clipboard only when the user selects a copy action.
- Theme preference and call-counter values are stored in the browser's "localStorage" on the device in use.
- Form values are not intentionally persisted by the application.
- Avoid entering real customer personal, banking, identity, or transaction information into a public demo. Use fictional/sample data when demonstrating the project.

Scope and limitations

- This public version does not connect to a CRM, ticketing platform, internal employee directory, or company database.
- Staff-specific names and identifiers have been replaced with a generic referral destination field.
- Provider-specific market, staking-pool, and currency-status API modules have been removed from this public build.
- Processing-cycle wording is generalized and should be reviewed and adapted before operational use in a real organization.
- The tool prepares text; it does not submit tickets, execute transactions, or verify customer information.

Project purpose

This project demonstrates practical frontend development and workflow-focused problem solving: turning repetitive operational tasks into a clear, reusable browser-based toolkit.

License

No open-source license is included in this repository yet. Unless a license is added, the default copyright rules apply and reuse, modification, and redistribution are not automatically granted. Choose and add a license only if you are comfortable granting those permissions.
