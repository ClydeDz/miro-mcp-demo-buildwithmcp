# Design Research Interview: Project "Instant Zenith"

**Date:** February 16, 2026
**Participants:** Leo (Lead Product Designer, Zenith Finance) & Elena (Fintech Product Lead & Former Investment Banker)
**Duration:** 20 Minutes

---

## **Introduction**

**Leo:** Testing, one, two... okay, we’re live. Elena, thanks for making the time. At Zenith Finance, we pride ourselves on being "premium," but our onboarding feels more like a "premium headache." We’re seeing a 60% drop-off at what we call "The 48-hour Void."

**Elena:** (Smiling) Let me guess—that’s the part where you tell the user, "Thanks for the info, now sit tight while our back-office team manually reviews your utility bill from 2024"?

**Leo:** Exactly that. We have an 8-step flow, but Step 3 and Step 4 are where the real friction is. We ask for manual address verification and a PDF upload of a bank statement. Then we hit them with Step 5: a 20-question survey about their "Investment Appetite."

---

## **The Discussion**

**Elena:** Leo, it’s 2026. If I have to find a PDF on my phone while I’m sitting on a bus trying to open a bank account, you’ve already lost me. Why are you asking for a bank statement to prove I have money?

**Leo:** Well, currently, our Step 5—the Financial Goals section—requires that data so our AI can suggest a portfolio. But because the user manually types their income and then uploads a separate document, our compliance team has to manually cross-reference them. That’s what creates the 48-hour delay.

**Elena:** You’re building a wall and then asking the user for a ladder. Here’s how you fix this: **The "Data-Sync" Strategy.** **Leo:** I'm listening. How do we get around the manual cross-referencing?

**Elena:** You scrap Step 2 (Manual Details) and Step 3 (Address Upload). Instead, Step 1 should be **"The Digital Handshake."** You use Open Banking APIs. The user just logs into their _existing_ old bank account via your app.

**Leo:** Wait, we currently have "Account Type Selection" as Step 1. You’d move that?

**Elena:** Absolutely. Don’t ask them what account they want until you know who they are. If they sync their data via Open Banking, you instantly get their verified name, address, and three months of transaction history. No PDFs. No manual typing. No "48-hour Void."

**Leo:** (Nodding) That would certainly kill the manual review. But our Compliance lead, Sarah, always insists on Step 4: the "Identity Selfie" and ID scan.

**Elena:** Keep the selfie, but make it **Step 2.** But here’s the kicker: combine it with liveness detection. While they are taking the selfie, your backend is already categorizing the transaction data you pulled in Step 1.

**Leo:** Interesting. So by the time they finish the selfie, we already know their "Investment Appetite" without asking the 20 questions in Step 5?

**Elena:** Exactly! Why ask me "How much do you save monthly?" when you can _see_ I save $1,200 monthly? Your Step 5—that long-form survey—should be replaced by **Step 3: "The Goal Swipe."** Show them three beautiful, pre-filled cards based on their actual data. "We see you're a saver—want the High-Yield Path?" They swipe right. Done.

**Leo:** I love the "swipe" idea. Currently, our Step 6 is "Employment Verification" where they have to type their employer's address. It's a huge friction point.

**Elena:** Why? You already saw their salary deposit in Step 1. You know they work at "TechCorp." Just show a button that says "Is this still your employer?" and let them tap "Yes." You're turning "data entry" into "data confirmation."

**Leo:** You’re essentially suggesting we collapse Steps 2 through 6 into a single automated flow driven by the initial API sync.

**Elena:** You got it. And Step 7—your "Legal Disclosures"? In your current app, it’s a wall of text that people just scroll past.

**Leo:** It is. It’s Step 7 of 8, and by then, users are just tapping "Agree" without looking.

**Elena:** Make it a 15-second "Video Summary" or an interactive checklist. If they’ve done the first three steps in under three minutes, they won't mind spending 30 seconds on the legalities. Then Step 4—the final step—is just "Set your Biometric Lock." No password setup. Use the FaceID they already have on their phone.

**Leo:** So we go from 8 steps with a 2-day wait, to 4 steps with an instant "Welcome" screen?

**Elena:** 100%. You remove the "Void," you remove the PDFs, and you treat the user's time like the "premium" asset you claim Zenith is.

---

## **Closing**

**Leo:** Elena, this is gold. You've essentially turned our "Survey-heavy" process into a "Data-driven" one. Moving the API sync to the very beginning changes everything.

**Elena:** It’s about trust, Leo. If you show the user you already "know" them (securely), they trust you more than if you ask them for the same info five times.

**Leo:** This is going to give our engineers a lot to think about—especially the "Goal Swipe" concept. Thank you!

**Elena:** My pleasure. Good luck with the "Void"!
