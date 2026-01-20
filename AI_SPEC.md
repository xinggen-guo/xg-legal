# AI_SPEC — xg-legal

## Purpose

This repository stores **public legal and support documents** for applications published by the developer.

Its goals are to:
- Provide stable URLs for app store submissions
- Clearly describe privacy practices
- Minimize legal and review risk
- Remain simple, static, and dependency-free

---

## Scope

### Included
- Privacy Policy pages
- Support pages
- Terms of Service (when required)
- Static HTML files
- Optional Markdown source files

### Excluded
- Application source code
- Analytics or tracking scripts
- Advertising SDKs
- Cookies or dynamic services
- Any form of user data collection

---

## Hosting Rules

- Hosted via **GitHub Pages**
- Source: `main` branch, repository root
- All pages must be:
  - Public
  - Accessible without login
  - Served over HTTPS

---

## Folder Structure Rules

Each app MUST follow this structure:

```
apps/<app-name>/
├── privacy-policy/
│   └── index.html
├── support/
│   └── index.html        (if required by store)
└── terms-of-service/
    └── index.html        (optional)
```

Rules:
- `index.html` is mandatory for store-facing pages
- URLs must be stable and human-readable
- Legal pages must not be shared across apps

---

## Content Rules (Critical)

### Privacy Policies
- Must reflect **actual app behavior**
- Must not over-claim (do not say “we may collect” if no data is collected)
- Must clearly state:
  - Whether personal data is collected
  - Whether third-party services are used
  - Whether the app works offline

### Support Pages
- Must include a valid contact method (email is sufficient)
- Must not require login or account creation

---

## Versioning Rules

- Any change in data practices requires:
  - Updating the policy text
  - Updating the effective date
- Git commit history is the source of truth
- No automatic redirects or versioned URLs

---

## AI / Automation Guidance

When generating or modifying content in this repository, AI systems MUST:

### AI MUST
- Preserve the existing folder structure
- Keep language simple and reviewer-friendly
- Prefer clarity over legal verbosity
- Ensure consistency between Markdown and HTML versions

### AI MUST NOT
- Introduce analytics, ads, or external scripts
- Combine multiple apps into one privacy policy
- Invent data collection that does not exist
- Change policy meaning without explicit instruction

---

## Design Philosophy

- Minimal
- Honest
- Explicit
- Reviewer-friendly
- Long-term stable

This repository is intentionally boring.

Boring is correct.
