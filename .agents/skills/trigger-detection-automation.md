# trigger-detection-automation

Use this skill to design the infrastructure required to listen for
triggers in the market. A trigger is useless if you find out about it three months late.

## The Tiered Detection Approach

### Level 1: Native Alerts (The Floor)
- **Tool:** LinkedIn Sales Navigator (Saved Searches / Account Lists).
- **Triggers:** Job changes within your saved leads, company news alerts, funding rounds.
- **Workflow:** Daily 30-min SDR block to review the "Alerts" tab.
- **Limitation:** Highly manual, relies on rep discipline.

### Level 2: Platform Subscriptions (The Standard)
- **Tools:** Apollo, Cognism, ZoomInfo.
- **Triggers:** Funding rounds, specific tech stack changes, hiring velocity spikes.
- **Workflow:** Set up automated "Plays" or saved searches that automatically add qualifying accounts to a sequence.
- **Limitation:** Data is often delayed by 7-14 days.

### Level 3: Programmable Workflows (The Advanced)
- **Tools:** n8n, Clay, PhantomBuster, Zapier.
- **Triggers:** Granular job board scraping (e.g., looking for specific keywords in a JD), website visitor deanonymization (RB2B/Clearbit), G2 category intent.
- **Workflow:** 
   1. RB2B deanonymizes a visitor on your pricing page.
   2. Webhook fires to n8n.
   3. n8n searches Clay for that person's direct manager.
   4. Clay enriches the contact and pushes to Outreach.
   5. SDR receives a Slack alert: "High Intent Target added to sequence."

## The "False Positive" Defense
Automation generates noise. You must build filters.
- **The "Intern" Rule:** A company hiring 10 interns is not a "growth trigger." Filter out non-ICP job titles from hiring velocity metrics.
- **The "Small Round" Rule:** Exclude Seed and Pre-Seed funding rounds if your ACV is over $50k. The budget simply isn't there despite the signal.
- **The Competitor Rule:** Always exclude known competitors, partners, and current customers from automated intent routing.

## Output Contract
When advising on trigger automation, provide:
- The optimal tool stack for the specific trigger.
- A high-level workflow diagram (e.g., Trigger -> Tool A -> Tool B -> CRM).
- Specific data filters to apply to prevent false positives.
