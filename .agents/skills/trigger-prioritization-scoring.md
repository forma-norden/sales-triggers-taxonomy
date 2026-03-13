# trigger-prioritization-scoring

Use this skill to rank incoming triggers so your team works the highest
converting signals first, ignoring the noise.

## The "Time to Pain" (TTP) Scoring Model

Score every incoming intent signal/trigger on a scale of 1-10 based on these three factors. 

### 1. Actuality (Weight: Strongest)
Did the event *actually* happen, or is it implied?
- **Actual Event (Score 3):** They installed Marketo yesterday. (Fact).
- **Stated Intent (Score 2):** They watched a webinar on "Fixing Marketo." (Interest).
- **Implied Intent (Score 1):** The Bombora Co-op says they are researching "Marketing Automation." (Vague).

### 2. Immediacy of Pain (Weight: Strong)
How fast does this event create a problem they must solve?
- **Immediate (Score 3):** Server outage, massive data breach, competitor won huge deal. Fix it today.
- **Short-Term (Score 2):** New VP hired (90-day plan), Fundraise announced (Quarter-end goals).
- **Long-Term (Score 1):** Opened a new office, added a new feature.

### 3. Financial Capacity (Weight: Moderate)
Does this trigger equal new budget?
- **High (Score 3):** Series A/B/C funding, acquired by PE, new fiscal budget year.
- **Neutral (Score 1):** Standard daily operations.
- **Negative (Score 0):** Layoffs announced, missed earnings, Chapter 11. 

## The Action Matrix

Calculate the Total Score (Actuality + Immediacy + Capacity). Max score is 9.

| Total Score | Classification | SLA (Time to Action) | Execution |
|-------------|----------------|----------------------|-----------|
| **7 - 9**   | Tier 1: Red Hot| < 2 Hours | Manual, highly customized AE/SDR outreach. Multi-threaded. |
| **4 - 6**   | Tier 2: Warm   | < 24 Hours | Automated AI-assisted sequence. 1 manual touch. |
| **1 - 3**   | Tier 3: Cold   | Batch Weekly | Purely automated, segmented nurture sequence. |
| **0**       | Do Not Contact | N/A | Exclude from all outreach due to negative capacity. |

## Signal Decay (The Timing Factor)
A Tier 1 signal degrades automatically to Tier 3 if not acted upon rapidly.
- **Inbound/Pricing Visit:** Decays to Tier 3 after 48 hours.
- **Change of Roles:** Decays to Tier 3 after 60 days.
- **Funding Round:** Decays to Tier 3 after 45 days.

## Output Contract
When asked to prioritize triggers, provide:
- The Actuality/Immediacy/Capacity score calculation.
- The recommended Tier (1-3).
- The strict SLA and channel strategy based on the score.
