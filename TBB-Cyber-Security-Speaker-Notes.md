# Think B2B — Cyber Security Awareness Training 2026
## Facilitator Speaker Notes & Learner Study Guide
**Document ref:** TBB-TRN-ETH-004-SN | Version 2.0 | March 2026

---

> **HOW TO USE THESE NOTES**
> - **Facilitators:** use the talking points under each slide to brief the team verbally or via Teams. Click → on each slide to reveal content step by step.
> - **Self-study learners:** read the learning notes under each slide after viewing it — these expand on the on-screen content with context and examples specific to Think B2B.

---

## Slide 1 — Title & Introduction

**Key message:** This is a mandatory, legally-required training module. Every person at Think B2B must complete it.

**Talking points:**
- This training satisfies the ISO 27001 Annex A.7.2.2 requirement for information security awareness training
- Completion is recorded — the Microsoft Forms knowledge check at the end generates a completion certificate
- The training takes approximately 20 minutes and covers all the scenarios most relevant to our type of business
- You can pause and come back — but please complete within your allocated window

**Learner note:** Even if you've worked in marketing agencies before, this training is specific to Think B2B's tools, contacts and obligations. The scenarios are real — each one reflects a documented incident from a similar UK agency.

---

## Slide 2 — Learning Journey (Agenda)

**Key message:** We cover 8 practical sections — all directly relevant to your daily work.

**Talking points:**
- Section 1 (Threat Landscape) explains why we are a target — this matters before anything else
- Sections 2–4 are the highest-risk areas based on NCSC 2024 data
- Section 7 covers our legal obligations under UK GDPR and how they connect to EcoVadis
- The Knowledge Check is separate — accessed via Microsoft Forms after this deck

**Learner note:** If you already feel confident in one area, the click-by-click reveal on each slide means you can pause and reflect on each point before moving on. Use the → key or click anywhere on the slide to reveal the next item.

---

## Slide 3 — The Threat Landscape

**Key message:** UK agencies are actively targeted. These are not abstract risks.

**Talking points:**
- 32% of UK businesses experienced a breach in 2024 — that is roughly 1 in 3 (NCSC Cyber Security Breaches Survey 2024)
- 84% of those incidents started with a phishing email — making everything in Section 3 critical
- The average UK breach costs £3.4M when you include investigation, remediation, fines and client loss (IBM Cost of a Data Breach 2024)
- As a B2B agency, we are particularly attractive because we hold multiple clients' data simultaneously — one breach affects all of them

**Learner note:** The scenario box on this slide is based on a composite of documented UK agency breaches. The Teams login exploit is a known attack vector — attackers send a cloned Teams login page to harvest M365 credentials. The reason agencies are targeted is simple: we have access to large volumes of data belonging to well-known organisations, and our security posture is often weaker than those organisations themselves.

---

## Slide 4 — Data We Hold

**Key message:** Every category of data we handle is a regulatory asset with obligations attached.

**Talking points:**
- Client commercial data includes campaign strategies and pitch decks — commercially sensitive and sometimes covered by NDAs
- Contact and personal data falls under UK GDPR — the Mailchimp lists and Salesforce CRM contain "personal data" as defined by the DPA 2018
- Any API keys (for integrations like Power Automate, Mailchimp, or client portals) are system access credentials — treat them as passwords
- SharePoint and M365 hold all of the above — making those accounts extremely high-value targets

**Learner note:** UK GDPR defines "personal data" as any information that can identify a living individual — this includes email addresses in a Mailchimp list, phone numbers in Salesforce, and even LinkedIn profile links in a campaign brief. The fact that a client provided the list does not remove our obligations as a data processor. If we suffer a breach involving that data, we are legally required to notify both the client and potentially the ICO.

---

## Slide 5 — Password Security

**Key message:** 80% of breaches involve compromised credentials. A strong, unique password is your first line of defence.

**Talking points:**
- "Strong password" means: minimum 12 characters, mixing uppercase, lowercase, numbers and symbols
- The best method is a passphrase — three or four random words plus a number and symbol: `Coffee!Client$Brief2026`
- Every platform needs its own password — if you reuse the same password on Salesforce, Mailchimp and your personal accounts, one leaked password unlocks all three
- Ask about the approved password manager — it removes the burden of remembering unique passwords

**Learner note — why uniqueness matters:** In 2024, a major UK email marketing database was sold on the dark web containing 2.4 million plaintext credentials. Anyone who used the same email/password combination on that platform and on their work systems was instantly compromised across both. Password managers eliminate this risk entirely — they generate and store unique passwords for every service. The approved tool for Think B2B is specified in the IT Acceptable Use Policy on BrightHR.

**Common excuses (and why they don't hold):**
- "I can't remember lots of passwords" → Use a password manager, you only need one master password
- "It's just an internal tool, it doesn't matter" → Internal tools often have wider access to client data than external tools
- "I share login with a colleague for convenience" → Shared logins make it impossible to audit who accessed what — this is a GDPR issue

---

## Slide 6 — Multi-Factor Authentication (MFA)

**Key message:** MFA stops 99.9% of automated attacks — it is non-negotiable on all business platforms.

**Talking points:**
- MFA means you need two things to log in: something you know (password) and something you have (phone/authenticator app)
- Microsoft Authenticator app is recommended — it is free and takes under 5 minutes to set up
- The most important MFA habit: if you receive an unexpected MFA prompt, DENY IT and call Emma or Singularitee immediately
- Unexpected MFA prompts are the earliest warning sign that your password has already been compromised

**Learner note — the MFA fatigue attack:** A technique called "MFA bombing" involves attackers flooding you with repeated MFA prompts hoping you approve one just to stop the notifications. Never approve an MFA request unless you personally just pressed "Sign in." If you receive repeated prompts, treat it as an active compromise attempt.

**Setting up MFA — step by step:**
1. On your phone, download Microsoft Authenticator from the App Store or Google Play
2. In any M365 app, go to your account security settings
3. Select "Add sign-in method" and follow the QR code setup
4. Contact Singularitee (support@singularitee.co.uk) if you need help

---

## Slide 7 — Phishing, Vishing & Smishing

**Key message:** Phishing is not just email — attackers use phone calls and text messages too. The trigger is always urgency.

**Talking points:**
- Phishing: fraudulent emails designed to get you to click a link or open an attachment. The most common disguises are Microsoft, HMRC, DHL, and colleagues
- Vishing: a phone call from someone pretending to be IT support, a supplier or a manager asking for credentials or urgent action
- Smishing: SMS or WhatsApp messages from fake senders with malicious links. These have increased significantly since 2022
- The common thread is urgency — attackers always create time pressure to prevent you from thinking

**Learner note — spear phishing:** The most dangerous form is "spear phishing" — a targeted email that appears to come from someone you know, using accurate details about your work. For an agency, this could look like: "Hi [name], can you review the updated brief for [real client name]? I've shared it here: [fake link]." The attacker researches targets on LinkedIn and the company website before sending. The email may come from a domain that looks almost identical to a genuine one — always check the full email address, not just the display name.

**Red flag practice — real vs fake domains:**
- Real: `info@microsoft.com`
- Fake: `info@micros0ft.com` (zero instead of o) or `info@microsoft-support.net`
- Always hover over any link before clicking to see the actual URL

---

## Slide 8 — Phishing Email Example

**Key message:** Phishing emails often look genuine. Train your eye on the warning signs.

**Talking points:**
- The main visual clues in phishing emails: sender domain mismatch, generic greeting ("Dear user"), artificial urgency, mismatched links
- Always go directly to the site (office.com, salesforce.com) by typing it in the browser rather than clicking email links
- Forward suspected phishing emails to support@singularitee.co.uk — do not click anything in them first
- If you accidentally clicked a link, report it immediately — no blame, but the faster we know, the faster we can respond

**Learner note — what happens if you click:**
Clicking a phishing link does not always cause immediate, visible damage. Often it silently harvests your session cookies (keeping you "logged in") and gives the attacker access without you noticing. This is why it is critical to report even if nothing visible happened. IT can check access logs and revoke tokens before damage is done.

**The "test yourself" habit:** Before clicking any link in an email, ask: "Would I be comfortable if Emma or a client could see exactly what I'm about to do?" If not — don't click.

---

## Slide 9 — Social Engineering & AI Scams

**Key message:** Attackers use AI to make scams indistinguishable from genuine communications.

**Talking points:**
- CEO fraud is when an attacker impersonates a senior person (like Emma) requesting an urgent payment, share of credentials, or confidential information
- AI voice cloning can now replicate a known voice from a 30-second audio sample — a Teams call or LinkedIn video post is enough
- Fake SharePoint pages are pixel-perfect copies of our actual login — the only difference is the URL
- The verification rule: if any request involves money, credentials, or sensitive data — verify through a completely different channel regardless of how real it seems

**Learner note — the £25 million deepfake case:** In February 2024, a Hong Kong finance worker transferred £25 million after a video call with what he believed were colleagues — all were deepfake avatars. While this is an extreme case, the technique is increasingly accessible. At Think B2B, any request for payment to a new or amended bank account must be verified by phone call to a known number before processing — not by replying to the email that requested it.

**The pause-and-verify rule in practice:**
- Received a Teams message from "Emma" asking for the Salesforce login? Call Emma's mobile before responding.
- Client asking for campaign budget transfer to a new account? Call your client contact at their known number.
- IT asking for your password to fix an issue? Never — legitimate IT never asks for your password.

---

## Slide 10 — Remote Working

**Key message:** The same security standards apply at home. There are no relaxed rules for remote environments.

**Talking points:**
- Screen positioning is often overlooked — visible screens in video calls, coffee shops, or open-plan home spaces can expose client data to unintended viewers
- Personal devices and personal cloud storage must never hold work files — even temporarily
- Public Wi-Fi networks (cafés, hotels, train stations) are frequently monitored — use a mobile hotspot instead
- The auto screen lock setting should be a maximum of 5 minutes — check yours now (Windows: Settings > Lock screen > Screen timeout)

**Learner note — the "shoulder surfing" risk:** In a study by 3M in 2019, 82% of respondents said they had witnessed someone else's confidential information on a screen in a public space. At Think B2B this could mean a campaign budget spreadsheet, a client brief or a Salesforce pipeline visible to anyone seated nearby. Lock your screen whenever you step away, even for a few seconds.

**Home network security check:**
- Log into your router admin page (usually 192.168.1.1 or 192.168.0.1)
- Check: is Wi-Fi encryption set to WPA2 or WPA3? (Not WEP — that is outdated and easily cracked)
- Change the default admin username and password on the router if you haven't already
- Contact Singularitee if unsure — this takes under 10 minutes

---

## Slide 11 — Cloud & Data Handling

**Key message:** Microsoft 365 is our only approved platform. Shadow IT creates invisible GDPR liability.

**Talking points:**
- "Shadow IT" means using a tool for work without IT or management approval — even with good intentions
- Personal cloud services (personal Google Drive, personal iCloud, Dropbox) are not covered by our data processing agreements and create GDPR liability the moment client personal data touches them
- Any new tool that will process personal data requires a Data Processing Agreement (DPA) before first use — this includes AI tools like ChatGPT when pasting client contact information
- Approved tools list: SharePoint, Microsoft Teams, Outlook, Salesforce, Mailchimp, Power Automate, Notebook LM (for non-personal data research)

**Learner note — AI tools and GDPR:** Using an AI tool (ChatGPT, Claude, Gemini, etc.) and pasting in client contact names, email addresses or campaign briefs constitutes data processing. Without a DPA in place between Think B2B and that AI provider, this is a potential GDPR breach. The safest rule: never paste personal data (names, emails, phone numbers) into any AI tool not on the approved list. Anonymise or pseudonymise data first.

**If you want to use a new tool:**
1. Identify what data it will touch (personal? client-confidential?)
2. Raise with Emma Czirok before first use
3. Emma reviews and raises with Singularitee for DPA check
4. Get written approval, then proceed

---

## Slide 12 — Legal & Compliance

**Key message:** Non-compliance has financial, contractual and reputational consequences that directly affect Think B2B's ability to operate.

**Talking points:**
- UK GDPR / DPA 2018: ICO can issue fines up to £17.5 million or 4% of global annual turnover — whichever is higher. These are not theoretical — UK businesses received over £7.5 million in ICO fines in 2023/24
- ISO 27001 Annex A.7.2.2 specifically requires documented security awareness training for all staff — this training is that control
- EcoVadis Business Ethics pillar: our score here directly impacts our ability to win procurement-gated contracts (increasingly common in corporate B2B clients)
- Computer Misuse Act 1990: accessing any system without authorisation — including using a colleague's password "to help" — is a criminal offence

**Learner note — the 72-hour ICO notification rule:** Under UK GDPR Article 33, if Think B2B suffers a personal data breach that is likely to result in a risk to individuals' rights and freedoms, we must notify the ICO within 72 hours of becoming aware. This is why internal reporting speed is critical — not to trigger a fine, but to give the company time to assess and notify within the legal window. Delayed internal reporting removes that window.

---

## Slide 13 — Incident Reporting

**Key message:** Report immediately. Speed of response determines the severity of the outcome.

**Talking points:**
- The 5-step protocol is: Stop → Report → Notify → Document → Await guidance
- "Stop" means close the affected browser, email or app — not shut down the computer, as that can destroy forensic evidence
- The two immediate contacts are Emma Czirok and Singularitee IT support
- "Document" means write down what happened (even on paper) before taking any other action — this supports the ICO notification process

**Learner note — what counts as an incident to report:**
- Clicked a phishing link (even if nothing visible happened)
- Received an unexpected MFA prompt
- Sent an email with client data to the wrong address
- Found a USB stick and plugged it in
- Lost or had stolen any work device or phone with work accounts
- Noticed someone else's unusual behaviour on systems
- Accidentally shared a SharePoint document with an external person

**The "no blame" culture:** Cyber security incidents happen to skilled, experienced professionals. The NCSC acknowledges this. What matters is the speed and honesty of reporting. Think B2B's policy explicitly provides no disciplinary action for genuine, good-faith mistakes reported promptly. Concealment is a different matter entirely.

**Contacts:**
- Emma Czirok: emma.czirok@thinkb2bmarketing.com | 01977 708643
- Singularitee IT: support@singularitee.co.uk

---

## Slide 14 — Responsibilities & Commitments

**Key message:** Completing this training is a formal commitment to comply with Think B2B's cyber security policy.

**Talking points:**
- Policy reference: TBB-POL-012 on BrightHR — take 5 minutes to read the full policy
- By passing the knowledge check, you are confirming you have understood and will follow these requirements
- Annual refresh is mandatory — a reminder will be sent in Q1 2027
- Line managers are responsible for confirming their team has completed training and for escalating any non-completion

**Learner note — personal accountability:** Under UK GDPR, both the data controller (Think B2B) and individual employees can face consequences for deliberate or reckless data mishandling. While civil penalties sit with the organisation, the Computer Misuse Act creates individual criminal liability for deliberate breaches. Completing and adhering to this training is both a professional obligation and a personal protection.

---

## Slide 15 — Training Complete

**Next step:** Complete the knowledge check at **TBB-TRN-ETH-004-KC** via Microsoft Forms (link shared separately by Emma Czirok).

**Pass mark:** 8 out of 10. Retakes are permitted with no limit.

**Questions or concerns after completing this training?**
Contact Emma Czirok: emma.czirok@thinkb2bmarketing.com | 01977 708643

---

## Quick Reference Card
*(Print or save to your phone)*

| Situation | Action |
|-----------|--------|
| Suspicious email | Do not click. Forward to support@singularitee.co.uk. Tell Emma. |
| Unexpected MFA prompt | Deny. Call Emma immediately. |
| Clicked a phishing link | Stop. Call Emma + Singularitee now. |
| Lost or stolen device | Call Singularitee immediately. They can remote-wipe. |
| CEO fraud / payment request | Stop. Call the requester on their known number. |
| New tool for work | Do not use until Emma has approved it. |
| Data shared with wrong person | Tell Emma within the hour. |

---

*Think B2B Marketing Ltd | TBB-TRN-ETH-004-SN | Version 2.0 | March 2026 | CONFIDENTIAL*
