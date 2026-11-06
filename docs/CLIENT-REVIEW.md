# Client Review: Lab 06 Identity Service Desk Operations

**Repository folder:** `lab-06-identity-service-desk-operations`
**Status:** Client review (not published)
**Purpose:** Third lab of the nine-lab portfolio, built in the same style and evidence approach as Labs 03 and 07.

This file is for internal review only. It can be removed before publication.

**How to review:** open [`preview.html`](preview.html) in any web browser. No installation or internet connection is needed: images, styling and the diagram renderer are embedded. It is a local approximation of the README, not an exact GitHub rendering, and `README.md` remains the deliverable. Use *Expand all steps* at the top of the preview to open every collapsible section at once. The links to the diagram PNGs are relative, so keep the package folder structure intact (`docs/` next to `assets/`). Like this file, `preview.html` is a review aid and should be removed before publication.

---

## 1. Decisions required before publication

| # | Decision | Options / notes | Client answer |
|---|---|---|---|
| 1 | **Approve style and content** | Approve as is, or list changes (tone, length, section depth, badge set, heading emojis, diagram style). | |
| 2 | **Hands-on completion** | Did the portfolio owner personally complete this lab? | |
| 3 | **Prerequisites** | Were Labs 1–4 completed first (provisioning with a deactivated leaver, MFA enrollment, WordPress SSO, group-gated WordPress)? | |
| 4 | **Own screenshots or evidence** | The source guide has **no screenshots**, so the package has none. Do you have your own screenshots or notes, for example event log entries, the inactive account state, the authenticator list, mover output or the bindings tab? Anything shared will be reviewed for personal data and secrets, and must not show passwords, QR codes, seeds or recovery codes. | |
| 5 | **Permission to republish source material** | The lab content comes from *Hands-On IAM Labs – Lab 6: Identity Service Desk Operations* by Andrew, All Things Identity. Please confirm you have permission to republish a summary of it publicly. | |
| 6 | **GitHub owner** | GitHub username or organization that will own the repository. | |
| 7 | **Repository name** | Proposed: `lab-06-identity-service-desk-operations`. Confirm or provide an alternative. | |
| 8 | **Repository visibility** | Public or private. Nothing will be created or pushed until this is confirmed. | |

---

## 2. How the answers change the README

- **If hands-on completion is confirmed with your own evidence:** the evidence-scope note will move to execution-based wording, your screenshots can be added to *Screenshots & Evidence* after a sensitivity review, and the status badge will change from *Client review* to a completion status.
- **If completion is confirmed without evidence:** the wording can say the lab was completed, while still noting that no screenshots or recorded results are included.
- **If completion is not confirmed:** the current wording stays. It describes what the guide describes, the expected behavior and the intended outcome, without claiming personal execution.
- **If republishing permission is not available:** the README will be reduced to a shorter, original summary of the skills and the custom diagrams.

---

## 3. Optional confirmations

- Should the README link to the prerequisite labs (Labs 1–4) and to Lab 07 once those repositories exist?
- Is there a preferred author name or profile link for the footer?
- Should the guide's interview talk track be summarized in more detail? It is currently referenced but not presented as the portfolio owner's own statement.

---

## 4. Evidence and safety decisions already applied

- **No screenshots:** the source PDF has 14 pages, no embedded images and no numbered figures. None were created, and rendered PDF pages are not presented as screenshots. The manifest's screenshot list is intentionally empty.
- **No invented records:** no ticket IDs, account names, timestamps, log exports, test results, approvals, caller-verification procedure or escalation outcomes are included.
- **No secrets:** no passwords, enrollment QR codes, seeds, recovery codes or tokens. The README advises never storing or sharing passwords in tickets or documentation.
- **Production guidance and lab exercises are kept separate:** for example, the Ticket 2 escalation (production) and the leaver reactivation (lab only).
- **The talk track is not reused as a claim:** the guide's first-person interview text is referenced as learner guidance, not as the portfolio owner's statement.
- **Editable diagrams:** the architecture and workflow diagrams are Mermaid diagrams written as text in `README.md`, with matching PNG exports in `assets/` linked below each diagram. Checksums are in [`evidence-manifest.json`](evidence-manifest.json).
- **No LICENSE file** has been added; that needs confirmed instructions.

---

## 5. Unresolved source limitations

- **Ticket 1 password inconsistency.** The section goal (p. 4) and testing checklist (p. 12) describe the user signing in with a credential the analyst never learned. On a fresh lab there is no recovery flow, so the guide falls back to the analyst setting the password directly (pp. 4–5). The README records the conflict and does not claim an analyst-unknown password.
- **Lab-only reactivation.** Ticket 2 tells the learner not to re-enable the leaver and to escalate, then has them reactivate the account for later labs (pp. 7–8). The README presents this as a controlled training step, separate from the production response, and does not claim it was performed. Lab 07 depends on this reactivated account.
- **Software version not stated.** The guide states no Authentik, OrangeHRM or WordPress version, no guide version and no capture date. It warns that menu labels change between releases.
- **Role mapping dependency.** The troubleshooting row on wrong WordPress permissions refers to group-based role mapping in Lab 4 Section 04. Whether the WordPress SAML plugin tier in use supports this, and how roles are configured, needs confirmation. (The Lab 7 guide notes a free-plugin setup that assigns one default role.)
- **Log behavior is the guide's report.** The finding that an inactive account's failed login is indistinguishable from a wrong password is stated for the guide's environment and has not been independently verified.
- **Caller verification and MFA exemptions.** The guide requires following the organization's verification standard and gives exemptions an expiry and a note, but defines neither procedure; none is invented.
- **No business scenario or metrics.** The guide describes no specific organization and gives no measurements, so none are reported.
