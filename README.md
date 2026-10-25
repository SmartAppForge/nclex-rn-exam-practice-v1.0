# NCLEX-RN Exam Practice — v1.0

A standalone, responsive HTML/CSS/JavaScript educational practice app for GitHub Pages. The supplied 40 questions are kept in their original order and wording. This is independent practice material, not an official NCLEX examination or endorsement.

## Files

- `index.html` — application structure
- `styles.css` — responsive styling
- `config.js` — app identity, Level 2 unlock threshold, and all four commercial links
- `questions.js` — original 40-question bank
- `app.js` — navigation, answer state, scoring, review, sharing, and unlock logic

## Updated results-page resource banner

The four colorful commercial resource cards now appear inside the Results screen after a practice level is completed. They are no longer rendered as a shared section on the home or quiz screens. The banner uses blue, green, orange, and purple cards with visual arrows and responsive layouts for desktop, tablet, and mobile. The existing result calculation, question bank, unlock threshold, and sharing behavior are retained.
- `TEST-CHECKLIST.md` — validation checklist
- `TEST-RESULTS.md` — recorded checks and outstanding manual tests

## Run locally

Open `index.html` in a modern browser. For the most representative test of sharing and browser storage, use a local static server or GitHub Pages (native share and clipboard support vary by browser and security context). No build step or package installation is required.

## Publish to GitHub Pages

1. Sign in to GitHub and create a **new, separate** repository named `nclex-rn-exam-practice`. Do not reuse or modify another application's repository.
2. Keep the repository public if using a GitHub Pages setup that requires public repositories on your plan, or follow the Pages options available to your account.
3. Upload all eight project files to the repository root. Confirm `index.html` is at the root, not inside a nested project folder.
4. Open the repository's **Settings → Pages**.
5. Under the build/deployment source, select **Deploy from a branch**, choose the default branch (usually `main`) and the `/ (root)` folder, then save.
6. Wait for GitHub Pages to finish deployment. Open the Pages URL shown in Settings → Pages.
7. Test the published URL on desktop and mobile. Verify the questions, scoring, all four commercial destinations, sharing fallback, and Level 2 gate.

## Configuration

Edit `config.js` to change `unlock.minimumPercent`. Level 2 is unlocked by the Level 1 score threshold and stored in the current session's in-memory result; the saved localStorage flag is informational only. This is a client-side educational gate, not secure access control: users can inspect or modify client-side JavaScript and local storage. No referral verification or server-side validation is implemented.

All four commercial URLs are exactly those supplied in the project brief. External offer links open in a new tab with `rel="noopener noreferrer"`.

## Question-bank note

Question wording, option text, order, and keyed answers are preserved from the supplied prompt. Explanations were not supplied, so none are invented. The key is reproduced as supplied and should be reviewed by a qualified nursing educator before being relied on for clinical exam preparation.
