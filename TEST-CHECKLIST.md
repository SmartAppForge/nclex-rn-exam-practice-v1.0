# Test checklist

## Question bank
- [x] Parse exactly 40 source questions (`q1`–`q40`) in source order.
- [x] Confirm unique IDs.
- [x] Confirm each question has an A, B, C, and D option.
- [x] Confirm each supplied answer key points to an existing option.
- [x] Confirm Level 1 uses q1–q20 and Level 2 uses q21–q40.
- [x] Preserve supplied question and option text; do not add unsupplied explanations.

## Functional checks to perform in a browser
- [ ] Home screen loads without console errors.
- [ ] Start Level 1 and navigate forward/backward.
- [ ] Prevent advancing without choosing an answer.
- [ ] Verify chosen answers remain selected when navigating back and forth.
- [ ] Complete a Level 1 run and manually verify score/count/percentage.
- [ ] Verify threshold behavior below, at, and above the configured percentage.
- [ ] Complete Level 2 after unlocking and verify its score/review.
- [ ] Test native share on a supported browser/device.
- [ ] Test clipboard/prompt fallback when native share is unavailable.
- [ ] Verify all four commercial buttons open their exact supplied URLs.
- [ ] Test responsive layout at phone, tablet, and desktop widths.
- [ ] Test keyboard navigation and visible focus states.
- [ ] Test published GitHub Pages URL after deployment.

## Publication
- [ ] `index.html` is at repository root.
- [ ] All script and stylesheet paths work on GitHub Pages.
- [ ] Confirm deployed page has no 404s or JavaScript errors.
