# Design Research Interview: Project "Swift Goliath"

**Date:** February 14, 2026
**Participants:** Sarah (Senior UX Researcher, Bank of Goliath) & Marcus (Candidate 1, Fintech Strategy Consultant)
**Duration:** 20 Minutes

---

## **Introduction**

**Sarah:** Alright, we’re recording. Marcus, thank you so much for joining us. As I mentioned, we’re at a bit of a crossroads at Bank of Goliath. Our "New-to-Bank" onboarding numbers are... well, they’re stable, but the drop-off rate is higher than we’d like. We want to pick your brain, especially given your background in finance.

**Marcus:** Happy to be here, Sarah. I’ve seen the "Goliath" flow from the outside, and honestly? It’s a beast. A bit of a dinosaur, if you’ll let me be blunt.

**Sarah:** (Laughs) Oh, we know. That’s why you’re here. To give you context for our discussion—and for the team listening later—our current process is a 10-step marathon. It starts with basic info, then swings into a heavy KYC (Know Your Customer) module, tax residency, employment history, and this complex conditional logic where if you’re self-employed, we basically send you down a rabbit hole of another four screens.

---

## **The Discussion**

**Marcus:** See, that’s the first mistake. You’re asking for the "whole life story" before you’ve even given them a reason to stay. If I’m a user, I want a bank account, not a mortgage application experience. Why is Step 4—let me guess, it’s the "Source of Wealth" section—even there before I’ve seen my dashboard?

**Sarah:** It is Step 4! Well, 4 through 6, actually, depending on how you answer the "Employment Type" question. We also have a "Card Preference" screen at Step 8 and a "Marketing Consent" screen at Step 9. It’s... exhaustive.

**Marcus:** It’s exhausting. Look, I’ve been thinking about this. You can get this down to **3 steps**. Ten minutes, tops. Probably five if the user is fast.

**Sarah:** Three steps? Marcus, our Compliance team would have a heart attack. How do you handle the backend logic that directs people to different paths? Currently, our system checks the zip code and employment status to decide if they need to see the "High-Risk/Enhanced Due Diligence" forms.

**Marcus:** You move the "logic" to the background. Step one: **The Identity Hook.** You use OCR (Optical Character Recognition). The user snaps a photo of their ID. The system pulls the name, address, and DOB automatically. No typing. If the ID is valid, they’re 80% there.

**Sarah:** Right, but what about the "Step 2" in our current flow where they have to manually verify their tax ID and residency status? It’s a legal requirement.

**Marcus:** No, Sarah, that’s Step 2 in _your_ world. In _my_ world, Step 2 is **"The Core Fit."** One screen. You ask for an email, a phone number, and a single dropdown for "Primary Use of Account." That’s it. You don't need the "10-year employment history" yet. You can "Progressively Disclose" that later when they actually try to move $50,000. For a standard checking account? It’s overkill.

**Sarah:** Progressive disclosure. I like the term. But wait, I need to backtrack to our current Step 7. That’s where we do the "Initial Funding." We’ve found that if we don't ask for the first $100 there, the account stays dormant. In your 3-step flow, where does the money come in?

**Marcus:** That’s **Step 3: "The Activation."** Once they hit "Submit" on Step 2, you show them their new IBAN or Account Number immediately. You give them a virtual card they can add to Apple/Google Pay _right there_. Then you say, "Fund your account to start spending." You’ve given them the "prize" before asking for the "payment."

**Sarah:** (Writing notes) So, ID snap, Core Info, then Activation. But what about the conditional paths? You know, the 10-step flow we have now has a specific branch for non-residents. If we skip those questions upfront, how do we know they aren't a regulatory nightmare?

**Marcus:** You use an API for a soft credit pull and a background AML (Anti-Money Laundering) check the second they finish Step 1. While they are busy choosing their "Step 2" preferences, your backend is already running the logic. If they flagged as "High Risk," _then_ you pop an extra screen. Don't punish the 95% of "easy" customers with a 10-step slog just because 5% of people are complicated.

**Sarah:** It’s a complete flip of our current philosophy. Right now, we gather everything—employment, tax, expected turnover, mother's maiden name—_then_ we run the check at the very end.

**Marcus:** Exactly. You’re making them do the work before you even tell them if they’re invited to the party. If you switch to my 3-step approach—OCR, basic contact, and immediate virtual issuance—you’ll cut that 20-minute abandonment rate by half. People just want to feel like they’ve "achieved" the account.

**Sarah:** I’m looking at our Step 10 right now, which is "Set Up Online Banking Password." It’s so late in the game.

**Marcus:** Put it in Step 2. Or better yet, use Biometrics from the phone. Why are we still making people type "P@ssword123" in 2026?

---

## **Closing**

**Sarah:** This has been incredibly insightful, Marcus. To summarize for my colleagues: you’re advocating for collapsing our 10-step conditional maze into a 3-step "Hook, Fit, and Activate" model, moving all the heavy-duty data gathering to a "post-onboarding" phase.

**Marcus:** Precisely. Make the "Goliath" feel like a "David"—lean and fast.

**Sarah:** Perfect. I think our diagrammers are going to have a fun time mapping this out. Thanks for your time!

**Marcus:** Anytime. Let’s kill those 10 steps.
