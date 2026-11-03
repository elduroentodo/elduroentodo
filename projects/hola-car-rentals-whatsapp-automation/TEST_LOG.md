# Customer-side test log

Test date: 2 November 2026. Channel: verified Hola Car Rentals WhatsApp account. Tester: the booking owner. Original language: Spanish; one explicit English-language request was tested. Identifiers are omitted from this log.

| Scenario | Customer action | Observed response | Verification status |
| --- | --- | --- | --- |
| Reservation lookup | Supplied own order number, booking email, and guided confirmation | Bot returned a confirmed status and rental supplier | Successful customer-side path observed; underlying status semantics not independently verified |
| Incorrect order/email pairing | Not attempted; builder reports that the verification API rejects non-matching pairs | No live rejection response captured | Implementation behavior reported by builder, not independently verified in this walkthrough |
| Broad pickup question | Asked for place, address, and time together | Bot said it did not fully understand and requested a more specific question | Fallback observed; requested details not delivered |
| Focused pickup question | Asked where to collect the car | Bot returned supplier, pickup address, and airport guidance | Pickup-location answer observed; pickup time not delivered |
| Insurance clarification | Asked what coverage the booking included | Bot asked for destination country and confirmation | Clarification observed; no coverage answer verified |
| English-language request | Asked for English and booking-specific coverage | Bot returned a generic Spanish follow-up | English preference and coverage request not fulfilled in this test |
| Confirmation resend | Requested a booking-confirmation email resend | Bot offered same-email or new-email choices | Choice observed; resend and delivery not verified |
| Email change | Not attempted | No record change | Out of scope for this walkthrough |

The screenshots in `assets/` are privacy-safe derivatives of the original conversation. A redaction-generation script is included in `tools/` for transparency, but its original inputs are deliberately not published.
