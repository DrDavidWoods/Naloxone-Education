# RESPOND — Naloxone & Opioid Overdose Recognition

An offline-capable single-file browser learning game for **public health nurses and aides**.

## Run locally

1. Download `index.html`.
2. Open it in Chrome, Safari, Edge, or Firefox. No install, account, or network connection needed after download.
3. Choose **Nurse** or **Aide**, select **Start the simulation**, and make eight decisions.

On iOS, the easiest use is to host the site and open it in Safari. The standalone HTML file can also be saved and opened with a compatible local-file browser/viewer, though iOS local-file behavior varies.

## Host using GitHub Pages

1. Create a new repository, for example `naloxone-response-training`.
2. Upload `index.html` to the repository root (you can upload this README too).
3. In **Settings → Pages**, choose **Deploy from a branch**, `main`, `/ (root)`, and save.
4. Visit the Pages URL shown by GitHub after deployment.

This is a static app; no server or database is needed. Once hosted, GitHub Pages loads from the internet. The downloaded HTML works offline independently; this release does **not** include an offline service worker for hosted use.

## Features

- Accessible, responsive mobile / desktop layouts
- Nurse and aide pathways, including appropriately different resuscitation decision points
- Eight decisions in a continuous clinical scenario
- Instant rationale and feedback after every decision
- Practice mastery scoring (all eight safety-critical decisions must be correct) with remediation of missed steps
- Four short lessons, recognition mini-challenge, and device-sequencing practice
- Quick-reference notes with source URLs
- Print-to-PDF completion summary, locally generated CSV results
- No trackers, external scripts, analytics, network calls, or transmitted learner information
- No data is stored between page loads; **CSV / print are optional and user initiated**

## Clinical sources

- CDC: https://www.cdc.gov/overdose-prevention/reversing-overdose/about-naloxone.html
- AHA 2025 BLS: https://cpr.heart.org/en/resuscitation-science/cpr-and-ecc-guidelines/adult-basic-life-support
- AHA 2025 special circumstances: https://cpr.heart.org/en/resuscitation-science/cpr-and-ecc-guidelines/adult-and-pediatric-special-circumstances-of-resuscitation
- FDA 2026 4 mg NARCAN labeling: https://www.accessdata.fda.gov/drugsatfda_docs/label/2026/208411Orig1s010lbl.pdf

Reviewed against sources in **October 2026**. Source material or local protocols may subsequently change.

## Safety / deployment review

**Educational prototype, not a real-time medical decision-support device, accreditation, CPR/BLS certification, or substitute for in-person clinical skills validation.**

The scenario involves an adult; pediatric response can differ. Review with your medical director, nurse educator, pharmacy leadership and local standing orders before deploying for mandatory employee competency. Some actions, including aid-level interventions, depend on training and departmental authorization. Keep actual naloxone product-specific instructions available. The game uses simulated case milestones, not real timers or guaranteed patient response outcomes.

The app does not capture verifiable staff identities or centrally log completions. For audited training you would need to incorporate it into an authenticated learning management system or backend. The printable summary and CSV are *self-reported learner outputs*, not tamper-resistant compliance records.

## Project structure

- `index.html` — the entire interactive app (HTML, CSS, JavaScript)
- `README.md` — run, hosting, clinical and privacy notes
