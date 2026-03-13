# trigger-to-message-mapper

Use this skill to convert raw trigger data into a compelling premise. If
you just mention the trigger without attaching it to pain, you sound like a creepy stalker.

## The "Catalyst to Pain" Hierarchy

You must map the specific trigger to the specific downstream pain it causes.

### Scenario A: New Executive Hired (e.g., New VP Sales)
- **The Stalker Premise (Bad):** "Congrats on the new role as VP Sales at Acme."
- **The Catalyst Premise (Good):** "Usually when a new VP of Sales joins, the immediate focus is auditing pipeline health. If you're currently trying to scrub bad data out of Salesforce..."

### Scenario B: Funding Round (e.g., Series B)
- **The Stalker Premise (Bad):** "Saw you just raised $20M. You must be growing. We have a tool you can buy."
- **The Catalyst Premise (Good):** "Assuming the board is demanding faster efficient growth post-Series B. Typically, that means ramping 10+ new SDRs this quarter. If ramp time is the current bottleneck..."

### Scenario C: Technographic Shift (e.g., Installed Shopify)
- **The Stalker Premise (Bad):** "I saw you use Shopify. So do we!"
- **The Catalyst Premise (Good):** "Lots of ecommerce teams migrating to Shopify right now. The biggest complaint we hear post-migration is getting inventory sync'd with physical stores. Are you guys running into that wall yet?"

## The Trigger Translation Formula

1. **Acknowledge the Event:** "Saw [Trigger Event]." (Short, factual).
2. **Introduce the 'Usually':** "Usually/Typically/Often, when companies do this, they run into [Pain Point]."
3. **The Pivot:** "If your team is actively trying to mitigate [Pain Point], we help by [Value Prop]."

## Output Contract
When asked to map a message to a trigger, provide:
- Extracted Catalyst: What downstream pain this event actually creates.
- 1 x Short email hook using the Trigger Translation Formula.
- Warnings on specific phrases to avoid (e.g., "Congrats on the funding").
