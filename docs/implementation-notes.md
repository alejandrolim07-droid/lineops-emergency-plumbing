# Implementation Notes

## 1. Niche and offer

The selected niche is emergency and residential plumbing. It was chosen because the customer problem is urgent, the value of a booked job can justify paid acquisition, and the local service area makes campaign outcomes easier to measure.

The offer uses a pain-point angle around small leaks becoming larger repairs, paired with a free inspection call to action.

## 2. Landing-page journey

The page was assembled in WordPress with Elementor and organized around one primary conversion:

1. The hero states the homeowner problem and presents the offer.
2. Trust points reduce hesitation.
3. Service cards make the scope easy to scan.
4. The primary button links to `#booking`.
5. The booking section contains the WPForms lead form.
6. Successful submission redirects to a dedicated thank-you page.

## 3. Responsive decisions

- Desktop uses a two-column hero with the message and CTA beside the plumber image.
- Tablet changes service cards to two columns.
- Mobile stacks content into one column.
- The mobile CTA uses a full-width, touch-friendly target.
- Fixed widths and negative margins were removed where they caused overflow.
- The form and name fields stack on small screens.

## 4. Form journey

WPForms was used for the inspection request because a free form solution was required. The form is visually contained in a high-contrast booking card and leads to a separate thank-you page after submission.

The thank-you page includes a clear confirmation message and a return action back to the LineOps landing page.

## 5. Tracking

The Meta Pixel base script was added and checked in the browser. The `fbq` function loaded and the configured Pixel ID appeared in the page runtime.

This confirms local script installation, not production event delivery. Public verification should be repeated after deployment to a permanent domain.

Recommended events:

| Event | Trigger |
| --- | --- |
| `PageView` | Landing-page load |
| `ViewContent` | Meaningful landing-page view |
| `Lead` | Successful form submission or thank-you-page load |
| Custom booking event | Confirmed appointment, when the scheduling layer exists |

## 6. AI follow-up concept

An AI receptionist demo and Twilio code were tested separately. The intended production behavior is:

1. Receive a validated form submission.
2. Send an immediate confirmation text.
3. Start an AI-assisted call or text qualification flow.
4. Escalate emergencies or uncertain cases to a human.
5. Record the interaction and appointment state in a CRM.

This integration is a planned next step and is not represented as production-complete.

