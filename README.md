# Audree Complaint Desk

Customer Complaint &amp; Feedback Management System — working Phase-1 prototype for distillery / alcobev clients.

## Files

| File | What it is |
|---|---|
| `index.html` | The application. Self-contained: open it in a browser, or serve the folder as a static site. |
| `flow.html` | Flow reference document — stages, owners, gate conditions, roles, SLAs. |
| `src-artifact.html` | Same app as a body fragment, for publishing into a host page. Not standalone. |

## Running it

Open `index.html` in any modern browser, or host the folder on any static web server (IIS, Netlify, GitHub Pages, Render).

A phone that scans the in-app QR needs a public `https://` address — set it in the app under **Customer Portal → Portal address encoded in the QR**.

## Scope

Consumer portal (active QR, complaint, feedback, status tracking, outcome confirmation) and the internal console: queue, classification, assignment, investigation (5 Whys, Fishbone 6M, Is/Is-Not, Gemba), RCA with QA Manager review, CAPA with separate effectiveness verification, approval, closure, duplicate linking, repeat and CAPA-failure detection, dashboards, six MIS reports, master data and audit trail.

## Prototype limits

Front-end only. Data lives in the browser (localStorage), authentication is a role switcher, email is a simulated outbox, and product/batch masters are seeded rather than read from an ERP. The deployed build targets .NET with Microsoft SQL Server.

Demo data is version-stamped — a newer build re-seeds itself automatically.
