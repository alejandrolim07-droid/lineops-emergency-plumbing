# Testing Checklist

## Completed prototype checks

- [x] Hero headline, supporting copy, and CTA are visible.
- [x] CTA scrolls to the booking section.
- [x] Booking section uses the `booking` CSS ID without `#` in the field.
- [x] WPForms accepts a test submission.
- [x] Successful submission reaches the thank-you page.
- [x] Thank-you-page return action routes back to LineOps.
- [x] Desktop layout reviewed.
- [x] Tablet and mobile stacking reviewed.
- [x] Mobile CTA and form controls use touch-friendly sizing.
- [x] Horizontal overflow fixes applied.
- [x] Meta Pixel base function detected in the browser.

## Required before production launch

- [ ] Deploy to a permanent HTTPS domain.
- [ ] Remove temporary LocalWP Live Link password protection.
- [ ] Confirm `PageView` in Meta Test Events.
- [ ] Confirm one `Lead` event per successful submission.
- [ ] Validate Pixel and Conversions API deduplication.
- [ ] Connect the form to a CRM or automation platform.
- [ ] Connect and test AI voice/text follow-up with consent controls.
- [ ] Add failure alerts and a manual fallback queue.
- [ ] Test real email/SMS delivery with approved sender details.
- [ ] Run accessibility, performance, privacy, and cross-browser checks.
- [ ] Replace demo business details with the final client information.

