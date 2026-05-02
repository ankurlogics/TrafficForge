# Chrome Web Store — Privacy practices questionnaire (draft answers)

**Important:** The dashboard wording changes over time. Match each answer to the **exact** question shown. If a question does not apply, answer honestly. Keep this file in sync with `../privacy-policy.html`.

**Contact / support email:** ankur.logics@gmail.com  
**Privacy policy URL:** After GitHub Pages is enabled (see `../README.md`), use the HTTPS URL to `privacy-policy.html`.

---

## Does this extension handle user data?

**Yes** — in the sense that it processes browsing-related **metadata** locally to implement user-configured rules and optional local logs. It does **not** send that data to the developer’s servers (no telemetry in the shipped code).

---

## Data types (check only what you actually collect / process)

Typical selections that fit TrafficForge:

- **Website content** — *Sometimes / Yes* if the form treats “URLs and request metadata shown in local logs” as website content. If the form distinguishes “content” vs “history,” prefer the narrower option that still matches: often **“User activity”** or **“Web history”** if available, for URLs stored locally in logs.

- **No** for health, financial, authentication passwords, etc., unless you add such features later.

If the store offers **“Customer content”** or **“Diagnostics”** for locally stored technical metadata, prefer that if it matches better than “Web history.”

---

## How data is used

- **App functionality** — Rules, scoping, match logs, and captured request suggestions only exist to operate the extension the user installed.

- **Not** for marketing, personalized ads, creditworthiness, or sale.

---

## Is data encrypted in transit?

**Not applicable** for data sent to *your* servers — the extension does not implement uploads of user traffic or rules to a backend you operate.  
HTTPS requests the user makes to **websites** are between the user and those sites (standard browser behavior).

---

## Can users request deletion?

**Yes** — Users can clear rules and logs with the extension’s **Reset** control, clear site data for the extension in Chrome, or uninstall the extension.

---

## Is data shared with third parties?

**No** — The extension does not sell or share user data with third parties for their own purposes. (Chrome/Google operates the store and browser; link to Google policies where the form requires.)

---

## Certification / declarations

Read each certification checkbox carefully. Do not check “certifies compliance” with laws (GDPR, COPPA, etc.) unless you understand your obligations as the developer/trader.

If asked whether the extension is **only for a narrow audience** (e.g. children): TrafficForge is aimed at **developers and testers**, not children.

---

## Data retention

- Data is kept **locally** until the user clears it, resets the extension, or uninstalls.
- No server-side retention by the developer for traffic content (there is no server component in the shipped extension).
