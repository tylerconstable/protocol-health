# Protocol Health — Booking Funnel Spec

## Objective

A high-converting multi-step survey that guides visitors to book and pay for a **Protocol Optimization Assessment**. Should feel like a quick health assessment, not a medical intake form.

## Design Principles

- **Mobile-first** — large tap targets, card-based answers, vertical layout, minimal typing
- **No personal info on first screen** — start with goals, not contact details
- **Short pre-booking flow** — 6–7 steps max before booking; medical intake collected after
- **One flow with conditional logic** — not separate forms per service
- **Progress bar** throughout: `Start → Goals → Symptoms → Health Profile → Booking`

---

## Funnel Steps

### Step 1 — Primary Goals

> *Start Your Personalized Health Assessment*
> Answer a few quick questions so our clinicians can understand your goals and recommend the right next step.
> *Takes about 60 seconds*
> Physician-led clinic | Personalized protocols | Advanced biomarker testing

**Question:** What brings you to Protocol Health today?
**Format:** Multi-select cards with icons

Options:
- Weight loss
- Hormone optimization
- Improve energy
- Improve libido / sexual health
- Longevity & healthy aging
- Pain or injury recovery
- Athletic performance
- Hair restoration
- General health optimization
- Not sure — I want expert guidance

---

### Step 2 — Desired Improvements

**Question:** What are you hoping to improve right now?
**Format:** Multi-select

Options: Lose weight / Increase energy / Improve focus / Balance hormones / Improve libido / Build muscle & performance / Recover from injury / Reduce pain / Support longevity / Improve confidence / Improve hair health / Optimize overall wellness

---

### Step 3 — Symptoms

**Question:** Which symptoms are you experiencing?
**Format:** Multi-select

Options: Weight gain / Fatigue / Brain fog / Low libido / Poor sleep / Mood changes / Hair thinning / Joint pain / Muscle pain / Slow recovery / Reduced endurance / Low motivation / Difficulty concentrating / None

---

### Step 4 — Basic Qualifiers

- **Age range:** 18–29 / 30–39 / 40–49 / 50–59 / 60+
- **Sex assigned at birth:** Male / Female *(helps recommend appropriate treatment pathways)*

---

### Step 5 — Conditional Goal Questions

Displayed based on Step 1 & 2 selections.

**Weight Loss Path** *(triggered by: weight loss, lose weight, weight gain)*
- Are you interested in medical weight loss treatment? → Yes / No / Maybe
- How much weight would you ideally like to lose? → 10–20 lbs / 20–40 lbs / 40–60 lbs / 60+ lbs / Not sure

**Hormone Path** *(triggered by: hormone optimization, libido issues, fatigue, improve energy)*
- Have you had hormone levels tested before? → Yes / No / Not sure
- Are you currently on hormone therapy? → Yes / No / Not sure

**Pain / Recovery Path** *(triggered by: pain recovery, injury, joint pain, muscle pain, performance)*
- Are you currently dealing with pain or injury? → Yes / No
- What best describes it? → Joint pain / Muscle strain / Back pain / Sports injury / Chronic inflammation / Slow recovery

---

### Step 6 — Height & Weight

- Height: Feet + Inches
- Current weight: Number field

*This helps us better understand your health profile.*

---

### Step 7 — Contact Information

> *Almost done*
> Please enter your information so we can save your results and help schedule your assessment.

Fields: First name / Last name / Email / Phone / City / State / ZIP / Date of birth

*Your information is kept private and used only to coordinate your care.*

---

### Step 8 — Confidence Step

> **You may be a great fit for Protocol Health**
>
> Based on your responses, patients like you often benefit from:
> - Medical weight loss
> - Hormone optimization
> - Peptide therapy
> - Longevity optimization
> - Recovery & performance support
>
> Our clinicians will review your goals and symptoms to design a personalized plan.

**CTA:** `Continue to Schedule Your Assessment`

---

### Step 9 — Booking

> *Schedule Your Protocol Optimization Assessment*
> Choose a time that works best for you.

- Calendar booking widget
- Visit type: In-person or Telehealth

---

### Step 10 — Payment

> *Confirm Your Protocol Optimization Assessment*
>
> Your assessment includes:
> - Comprehensive consultation
> - Personalized treatment recommendations
> - Lab review if available

Fields: Card number / Expiration / CVV / Billing ZIP
**Button:** `Confirm & Pay`

---

### Step 11 — Bloodwork

> *Help Us Prepare for Your Appointment*

**Question:** Have you had blood work done in the past 12 months?

**If Yes:**
- Upload labs now (PDF, PNG, JPG) or email them later
- Optional: Would you like to complete our Comprehensive Biomarker Panel (50+ biomarkers)? → Yes / Maybe / No

**If No / Not sure:**
- Your clinician may recommend our Comprehensive Biomarker Panel to better evaluate hormones, metabolic health, inflammation, and longevity markers
- Options: Yes / Maybe / No

---

### Step 12 — Confirmation

> **Your assessment is booked**
>
> Thank you for scheduling your Protocol Optimization Assessment.
> Please check your email and phone for appointment details and preparation instructions.

---

## Important Notes

Detailed medical intake is **intentionally excluded** from the pre-booking flow. The following are collected **after booking:**
- Medication list
- Allergies
- Family history
- Detailed medical history

**UX Goal:** Users should feel — *this clinic understands my goals, the process is fast and personalized, booking is the natural next step.*
