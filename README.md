# LEDGER — Blacksite Network Legal Site

A responsive, self-contained Terms of Service and Privacy Policy website for the LEDGER Discord bot. Uses no JavaScript, tracking scripts, analytics, cookies, external fonts, or external CDN files.

## MUST EDIT BEFORE YOU PUBLISH

1. Search all `.html` files and **replace `YOUR-CONTACT-EMAIL@example.com`** with a real, monitored contact address you control. This is a placeholder; messages sent to it will not reach you. This appears in `index.html`, `terms/index.html`, and `privacy/index.html`.
2. Verify that the person or organization operating the bot is accurately described as the **R.E.A.P.E.R. Divers community operator**. Update that wording if someone else is legally responsible for data.
3. Review the statements about Discord evidence storage, Railway SQLite storage, retention, moderators, purchases, and deletion. Only publish facts that match your actual deployed bot and practices. If your policies differ (for example, you introduce an external AI service), revise the policy.
4. Consider legal review, especially if the bot is used beyond a private community or if you serve people in regions with specific privacy requirements. These are practical draft policies, not a legal certification.
5. Update the “Effective / Last updated” dates if you publish on a later date.

## Publish to GitHub Pages — simplest setup

1. On GitHub, create a **new public repository** named `ledger-legal` (separate from your private LEDGER bot source).
2. Open the extracted `LEDGER-Legal-Website` folder and upload its **contents**, including `index.html`, `terms/`, `privacy/`, `assets/`, and `.nojekyll`, to the repository root.
3. In the repo, go to **Settings → Pages → Build and deployment → Source: Deploy from a branch**.
4. Choose **main** branch and **/(root)** directory, then **Save**.
5. After GitHub Pages publishes, open your site's URL and check both pages.
6. Copy these URLs into the Discord Developer Portal (Applications → LEDGER → General Information):

   - **Terms of Service URL:** `https://YOUR-GITHUB-USERNAME.github.io/ledger-legal/terms/`
   - **Privacy Policy URL:** `https://YOUR-GITHUB-USERNAME.github.io/ledger-legal/privacy/`

Replace `YOUR-GITHUB-USERNAME` with the GitHub account that owns the repository. These links are examples until you publish.

## Structure

```text
LEDGER-Legal-Website/
├── index.html
├── terms/
│   └── index.html
├── privacy/
│   └── index.html
├── assets/
│   ├── style.css
│   ├── mark.svg
│   └── ledger-logo.webp
├── .nojekyll
└── README.md
```

## How to update later

Edit the HTML text, commit changes to `main`, then GitHub Pages will republish. Do not upload your `.env`, token, SQLite database, screenshots, or any other secret files to this public repository.

## Note about Discord discovery

Public Terms and Privacy pages are part of app-discovery eligibility, but publishing them **does not** guarantee that the application meets all Discord App Discovery content requirements. In particular, ensure your public app description and branding are appropriate for Discord's policies.
