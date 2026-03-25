# Connectors — UK SMB Legal Plugin

Skills in this plugin reference tool categories using `~~placeholder` syntax. When you see a placeholder like `~~case-law-database`, it means the skill expects an MCP server providing that type of data. Connect your preferred platform to unlock automatic data retrieval.

## Tool Categories

| Category | Placeholder | Recommended UK Platforms |
|----------|-------------|------------------------|
| **Case Law Database** | ~~case-law-database | BAILII, Westlaw UK, LexisNexis, Practical Law |
| **Legislation** | ~~legislation | legislation.gov.uk, Westlaw UK |
| **Companies House** | ~~companies-house | Companies House API (free, API key required) |
| **Land Registry** | ~~land-registry | HM Land Registry (Business Gateway or portal) |
| **HMRC** | ~~hmrc | HMRC MTD API (OAuth 2.0), HMRC Developer Hub |
| **ICO** | ~~ico | ICO Register of Fee Payers, ICO guidance portal |
| **FCA Register** | ~~fca-register | FCA Financial Services Register API |
| **CMA** | ~~cma | CMA case database |
| **Court Forms** | ~~court-forms | HMCTS Form Finder |
| **Document Management** | ~~document-management | iManage, NetDocuments, SharePoint, Egnyte |
| **Practice Management** | ~~practice-management | Clio, LEAP, Smokeball, PracticeEvolve |
| **Office Suite** | ~~office-suite | Microsoft 365 (Word, Outlook, Teams) |
| **Communication** | ~~communication | Slack, Microsoft Teams, email |

## Connection Notes

- **Companies House API:** Free API key from developer.company-information.service.gov.uk. Provides company search, officer details, filing history, PSC register, and charges.
- **HMRC MTD API:** Requires OAuth 2.0 registration at developer.service.hmrc.gov.uk. Provides VAT obligations, returns, and ITSA quarterly updates.
- **Land Registry:** Business Gateway for bulk searches, or portal for individual searches. Practice account required.
- **BAILII:** Free access to UK case law at bailii.org. No API — use web scraping or manual search.
- **legislation.gov.uk:** Free API available. Provides full text of UK primary and secondary legislation.

> **Note:** The plugin works without any MCP connections — you can paste documents, describe scenarios, or ask questions directly. MCP connections enhance the experience by providing live data lookup.
