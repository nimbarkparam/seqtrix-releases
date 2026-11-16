# Seqtrix Privacy Policy

**Version:** 1.2
**Effective date:** 14 November 2026
**Applies to:** the Seqtrix desktop application and the seqtrix.com
website.

---

We at Seqtrix ("we", "us", "our") respect your privacy. This
policy explains what data Seqtrix collects, why, where it is stored,
who it is shared with, and how to exercise your rights over it.

If anything here is unclear, email us at help@seqtrix.com.

## 1. Who we are

Seqtrix

We are the data controller for the personal data described in this
policy.

## 2. What data we collect - and what we DON'T

### Data that stays on your computer

When you use the Seqtrix desktop application, the following stays on
your computer and is **never transmitted** to us unless you turn on
cloud sync or publish a share (both described below):

- Your sequences (action graphs, names, settings).
- Your schedules (triggers, target sequences).
- Local preferences (theme, mini-mode position, master-password
  configuration, EULA acceptance flag).
- Local execution reports (which actions ran, when, success/failure).

This data lives in `%APPDATA%\app.seqtrix.desktop\` on Windows.

### Data the app sends on its own

The app sends the following without you turning anything on:

- **Update check:** the app fetches a small version file from our
  release server. No identifier is attached.
- **Plan check:** on launch, when its window comes to the front, when
  you sign in or out, and about every 30 minutes, the app sends a
  one-way hash of your PC's Windows machine ID, and your sign-in
  token if you are signed in, to check your plan and trial. It
  carries nothing about your sequences. Our server keeps a record of
  every check: that hash, your account if you are signed in, the
  plan and trial it answered, your IP address, the app's user agent
  (a line of text that names the app's built-in browser and your
  Windows version) and the time. We use these records to spot misuse
  of trials and passes. They are not deleted automatically yet (see
  section 6).
- **Monthly totals** (signed in only, on by default): four numbers a
  month (runs, estimated time saved, plan-limit hits and paused
  runs), so a reinstall keeps your Time Saved meter. Never a
  sequence, path or command. Switch it off in Settings > Time Saved.

### Data Seqtrix collects only with your active opt-in

No telemetry by default. Crash reports and anonymous usage stats are
off until you turn them on in Settings > Privacy.

#### Crash reports (default: OFF, opt-in)

If you have turned crash reports on and the app crashes, we send a
report containing:
- The crash stack trace.
- App version and Windows version.
- The screen you were on and the error type.

A report never contains your sequences, file paths, vault or anything
you typed.

We use our crash-reporting provider for crash reports.

It is off until you turn it on. You can turn it on or off at any time
in **Settings → Privacy → Send anonymous crash reports**.

#### Anonymous usage analytics (default: OFF, opt-in)

If you turn this on, we collect anonymised events that help us
improve the product:
- App launch.
- Sequence created / run.
- Schedule created (with trigger TYPE only - e.g. "hotkey" - NEVER
  the configuration like which chord or which app).
- Settings panel opened, feature used.
- Approximate time-zone (for scheduling-feature analysis).

We do NOT collect:
- Sequence names, sequence contents, or action parameters.
- File paths, folder paths, command-line strings.
- Hotkey chord values or watched file paths.
- Any text the user has typed inside the app.

We use our analytics provider for usage analytics.

You can enable / disable this in **Settings → Privacy → Help improve
Seqtrix**.

### Data Seqtrix collects when you create a Seqtrix account

If and when you choose to create a Seqtrix account (required only to
buy a pass, sync or share):

- Email address - used as your account identifier and for
  service-related email (e.g. password resets, important notices).
- Authentication tokens - managed by our authentication provider.
- Sign-in metadata - device label and last-seen timestamp. Our
  authentication provider also records the IP address and user agent
  of each signed-in session, and removes them when that session is
  signed out.

If you sign in with a third-party provider, that provider
shares your email and basic profile (name, avatar URL) with us;
nothing more.

### Data we collect when you cloud-sync sequences (opt-in)

Only when you turn on cloud sync, your sequences (names, action graphs,
schedules) are encrypted in transit (TLS) and stored in our database
hosted by our database provider. We name the provider and its region
on request.

Encryption-at-rest is provided by the underlying database. End-to-end
encryption is on the roadmap.

### Data we collect when you publish a sequence (your action)

Publishing to the share gallery sends the one sequence you publish,
after you review what it contains, with your display name. Typed
text is left out by default and anything marked as a password is
refused.

### Data we collect when you buy a pass

Payments are processed by our payment partner. Your card, UPI or bank
details go to the payment partner and never reach us. We receive only
the payment reference, the amount, the currency, the payment method
type (card or UPI) and the email you gave at checkout, and we record
which pass you bought and when it ends.

Our payment partner's own privacy policy applies to the data they hold.

## 3. Why we use this data

| Purpose | Data used | Lawful basis (GDPR) |
|---|---|---|
| Run the app | Local data only | N/A - never leaves device |
| Check your plan, your trial and a pass's device limit | One-way hash of your PC's Windows machine ID | Legitimate interest |
| Spot misuse of trials and passes | Plan-check records: the machine-ID hash, your account if signed in, the plan answered, IP address, user agent and time | Legitimate interest (security) |
| Keep your Time Saved meter across reinstalls | Monthly run totals (signed in, on by default) | Legitimate interest |
| Diagnose crashes | Crash reports (opt-in) | Consent |
| Improve the product | Usage analytics (opt-in) | Consent |
| Operate your account | Email, auth tokens, and the IP address and user agent of each signed-in session | Contract |
| Sync your sequences | Sequence data (opt-in) | Consent |
| Run the share gallery | Sequences you publish, your display name | Contract (you chose to publish) |
| Unlock what you bought; receipts and the records tax law requires | Plan and payment records | Contract; legal obligation |
| Stop abuse (rate limiting the plan check and some website requests, and counting each report of a shared sequence once) | IP address; for a report, a one-way hash of your IP address and the page's address | Legitimate interest (security) |
| Send service emails | Email | Legitimate interest |

We do not use your data for advertising, ad personalisation, or
sale to third parties. Ever.

## 4. Who we share data with

These are the only categories of provider that handle data for us,
and what each one does. We name each provider on request: email
help@seqtrix.com.

| Provider | Purpose | Region |
|---|---|---|
| Account database | Accounts, sign-in, plans, cloud sync, share gallery | Named on request |
| Payment partner | Payments. Card, UPI and bank details go to the payment partner, never to us | India |
| Website host | Serving seqtrix.com and keeping its server logs | Global network |
| Bot-check provider | Telling people from bots on sign-in forms | Global network |
| Rate-limit store | Counters keyed by IP address or account for some website requests, and its log of the requests it counted | Named on request |
| Email provider | Sign-in and account emails from help@seqtrix.com, and our inbox | Provider data centres |
| Third-party sign-in provider | Only if you choose the third-party sign-in | The provider's data centres |
| Site-statistics service | Site statistics, only after you accept cookies | United States |
| Privacy-first, cookie-free page analytics service | Cookie-free page analytics, with no personal data | Global network |
| Crash-report service | Crash reports from the app, only if you opt in | United States |
| Usage-statistics service | Usage events from the app, only if you opt in | United States |
| Release server | Anonymous update checks and downloads | United States |

We will not share your data with any other third party without your
consent, except where required by law (e.g. valid court order).

## 5. Where data is stored

Local app data: on your computer at
`%APPDATA%\app.seqtrix.desktop\`.

Cloud-synced data: with our account database provider. We name the
provider and its region on request.

We do not transfer data to countries outside the storing region
without using appropriate safeguards (Standard Contractual Clauses
where required).

## 6. How long we keep data

| Data | Retention |
|---|---|
| Local app data | As long as the app is installed; deleted on uninstall |
| Crash reports | 90 days, then deleted |
| Usage analytics | 12 months, then aggregated and anonymised |
| Account data | As long as your account exists + 30 days after deletion |
| Plan-check records (IP address, user agent, machine-ID hash) | No automatic deletion yet; kept until we delete them |
| Plan-check rate-limit counters (one per IP address) | No automatic deletion yet |
| Website rate-limit counters | Up to about 2 hours |
| The rate-limit store's log of counted requests (IP address or account) | No automatic deletion yet |
| Report records (a one-way hash of your IP address and the page's address) | As long as the shared sequence exists |
| Signed-in session records (IP address, user agent) | Until you sign out of that session |
| Server logs (they include IP addresses) | Each hosting provider's standard retention |
| Cloud-synced sequences | Until you delete them or close the account |
| Published sequences and ratings | Until you unpublish or delete your account |
| Payment and receipt records | 8 years, as Indian tax and accounting rules require |

## 7. Your rights

If you have a Seqtrix account, you can at any time:

- **Access** the data we hold about you and get a copy - email
  help@seqtrix.com.
- **Correct** inaccurate data - Settings > Account, or email us.
- **Delete** your account and all associated data - email
  help@seqtrix.com. All cloud data is removed within 30 days;
  payment records may be retained for legal compliance.
- **Restrict or object** to processing - email help@seqtrix.com.
- **Port** your data to another service - email help@seqtrix.com for
  a copy of your data.
- **Withdraw consent** for analytics or crash reports - toggle them
  off in Settings > Privacy at any time. Turn cloud sync off in
  Settings > Sync.
- **Lodge a complaint** with your local data-protection authority
  (e.g. ICO in the UK, your state's Attorney General in the US, the
  CNIL in France).

For a request by email, we check that it comes from the account
holder, usually by replying to the account email, and answer within
30 days. There is no charge.

If you do not have an account, your sequences and settings exist only
on your computer, and you can delete them by uninstalling Seqtrix.
The plan check (section 2) still sends the one-way hash of your PC's
Windows machine ID.

For users in the European Economic Area, the United Kingdom, and
Switzerland, your rights under the GDPR / UK GDPR apply.

For users in California, your rights under the CCPA / CPRA apply,
including the right to know, the right to delete, the right to
correct, and the right to opt out of the sale or sharing of personal
information (we do neither).

For users in India, your rights under the Digital Personal Data
Protection Act 2023 apply.

## 8. Children

You must be 18 or older to use Seqtrix. We do not knowingly collect
data from anyone under 18. If you think we have, email
help@seqtrix.com and we will delete it.

## 9. Security

We use industry-standard measures to protect your data, including
encryption in transit (TLS), encryption at rest where supported by
the underlying provider, and least-privilege access controls. No
system is perfectly secure, however; if you suspect a breach of your
account, email help@seqtrix.com immediately.

If a breach affects your personal data, we tell the affected users by
email without undue delay, with what happened, what data was involved
and what we are doing about it, and we notify the authorities the law
requires.

## 10. Changes to this policy

We may update this policy from time to time. If we change it, the
date at the top changes, and we announce material changes at
seqtrix.com/privacy and, for registered users, by email before they
apply. The full policy is at
[seqtrix.com/privacy](https://seqtrix.com/privacy), the page the app
links to.

## 11. Contact

Privacy questions, data-rights requests, or complaints:
help@seqtrix.com

Seqtrix
