# Prompt 3: Customer Retention & Loyalty System

## Instructions
Run this prompt to build a complete retention engine. No third-party loyalty platform required — all copy works with email, SMS, and your POS system's basic customer list.

---

## The Prompt

You are a restaurant retention specialist. Generate a complete customer loyalty and retention system for the restaurant below. Every output must be TCPA, CAN-SPAM, and FTC compliant at generation time.

**RESTAURANT DETAILS:**
- Restaurant name: [NAME]
- Cuisine type and price range: [E.g., "Japanese ramen, $$"]
- Location: [CITY, STATE]
- Signature dish/drink: [ITEM]
- Average check per person: $[AMOUNT]
- Email platform (if any): [Mailchimp / Constant Contact / Square / Toast / other / none]
- SMS platform (if any): [Twilio / EZTexting / OpenPhone / Square / other / none]
- Do you take reservations? [Yes — OpenTable/Resy/direct / Walk-in only]
- Do you have a loyalty program? [Yes — describe / No]
- Owner/GM first name: [NAME]

**GENERATE ALL OF THE FOLLOWING:**

**1. 5-Email Post-Visit Sequence**
Triggered after first visit (or reservation completion). CAN-SPAM required: unsubscribe + physical address in footer of every email.

- **Email 1 — Receipt Follow-Up (send same evening or next morning)**
  Subject: "How was your [NAME] experience, [FIRST NAME]?"
  Preview: "We'd love to hear from you."
  Body (100–150 words): warm thank you, specific dish mention, plain review ask (no conditional language per FTC 2023)
  CTA: Google review link placeholder + Yelp link placeholder

- **Email 2 — Review Amplification (send Day 3 if no review, skip if review left)**
  Subject: "Still thinking about that [SIGNATURE DISH]?"
  Body (75–100 words): light follow-up, social media follow ask, "tag us" CTA
  No second review ask (avoid "review bombing" pattern)

- **Email 3 — Birthday/Anniversary Capture (send Day 7)**
  Subject: "A gift for you from [NAME]"
  Body (100 words): ask for birthday month (not day — avoids CCPA over-collection) and anniversary if applicable
  Offer: "We'll send you something special when your month arrives"
  Data collection note: explain what you'll do with the info (CAN-SPAM transparency)

- **Email 4 — Win-Back (send Day 45 if no return visit)**
  Subject: "[FIRST NAME], we've missed you at [NAME]"
  Body (100–150 words): "it's been a while" warm tone, new menu item or seasonal item highlight, bounce-back offer (% off or BOGO appetizer, no "free" standalone item — coupon law risk)
  Expiry: "[30 days from send date] — exact date required by FTC"
  CTA: reservation link or "show this email" instruction

- **Email 5 — VIP Upgrade (send after 3rd visit or $200+ lifetime spend)**
  Subject: "You're officially a [NAME] regular"
  Body (150 words): acknowledge loyalty, name the VIP benefit (priority reservation, off-menu item preview, birthday dessert), no purchase requirement to join (FTC)
  CTA: "Reply to this email to be added to the VIP list" — manual gate keeps list quality high

**2. SMS Loyalty System (TCPA Compliant)**
Every message requires: sender ID, opt-out instruction, no marketing on first message (opt-in confirmation only).

- **Opt-In Confirmation (send immediately after signup):**
  "[NAME]: Thanks for joining! You'll get exclusive offers & updates. Reply STOP to opt out. Msg & data rates may apply."

- **Welcome Offer (send 24 hours after opt-in):**
  "[NAME]: Welcome gift — [OFFER, e.g., 'free dessert on your next visit']. Valid [DATE RANGE]. Show this text. Reply STOP to opt out."
  Note: Free dessert on next visit (not "free meal") keeps acquisition cost under $5. Set exact expiry — FTC requires specific end dates.

- **Monthly Engagement (1x per month max — TCPA best practice):**
  "[NAME]: [MONTH] special — [LTO ITEM] available through [DATE]. Reserve: [LINK]. Reply STOP to opt out."

- **Birthday Message (send on first day of birthday month):**
  "[NAME]: Happy birthday month, [FIRST NAME]! Your gift: [OFFER]. Valid all [MONTH]. Show at checkout. Reply STOP to opt out."

- **Win-Back SMS (send Day 60 if no return, to customers who haven't opted out):**
  "[NAME]: We miss you, [FIRST NAME]! [OFFER] expires [DATE]. Reply STOP to opt out."

**3. Reservation Confirmation + Reminder Sequence**
For restaurants taking reservations (skip if walk-in only):
- **Confirmation email:** Subject: "Your [NAME] reservation is confirmed — [DATE] at [TIME]"
  Body: date, time, party size, address, parking notes, cancellation policy (24-hour notice recommended), "reply to this email with any special requests"
- **24-hour reminder email:** Subject: "See you tomorrow at [NAME] — [TIME]"
  Body: reminder details + "running late? Call us: [PHONE]" + cancellation link
- **2-hour reminder SMS (under 160 chars):** "[NAME]: See you at [TIME] today! Address: [ADDRESS]. Reply STOP to opt out."
- **No-show follow-up email (send next morning):** Soft re-booking ask, no shaming language

**4. Catering Inquiry Response Templates (5 scenarios)**
All responses within 2 business hours of inquiry — studies show response speed is the #1 catering conversion factor.

- **Template A — Corporate Lunch Inquiry:**
  Subject: "Re: Catering Inquiry — [NAME] for [COMPANY]"
  Body: confirm receipt, menu options, per-person pricing range, minimums, lead time, next step (call or tasting)

- **Template B — Wedding/Private Event:**
  Subject: "Congratulations! Let's talk catering for [EVENT DATE]"
  Body: congratulations, packages overview, deposit policy (clearly state — FTC contract transparency), tasting invitation

- **Template C — Large Party In-Restaurant (12+ guests):**
  Subject: "Private dining at [NAME] — let's get you set up"
  Body: room capacity, prix fixe vs. à la carte options, gratuity policy disclosure (FTC: service charges must be disclosed upfront), deposit terms

- **Template D — Pickup Order (corporate, recurring):**
  Subject: "Re: Regular catering order — [COMPANY]"
  Body: order confirmation format, lead time, payment terms, account setup for recurring clients

- **Template E — Inquiry Outside Service Area / Capacity:**
  Subject: "Thank you for reaching out to [NAME]"
  Body: gracious decline, referral if applicable, invitation to dine in-restaurant

**5. Review Response Templates**
- **5-Star response (under 75 words):** Thank by name, echo a specific detail from their review (shows you read it), invite return, mention specific item or staff member
- **3-Star response (under 100 words):** Thank, acknowledge the specific issue, no excuses, specific corrective action ("we retrained our servers on table timing"), invite return with a specific ask ("ask for [MANAGER NAME] when you come back")
- **1-Star response (under 120 words):** Thank, de-escalate, take accountability without admitting legal liability ("we're sorry this wasn't up to our standard"), move offline ("please email [CONTACT] directly so we can make this right"), no arguing, no counter-claims
Note: Yelp's 2023 policy prohibits offering incentives in review responses. Google does not allow incentives tied to star ratings. Both policies reflected in all templates above.
