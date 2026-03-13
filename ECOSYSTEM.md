# Ecosystem: sales-triggers-taxonomy

How this repo connects to the rest of the Forma Norden GTM library.

## Works With

| Repo | Relationship | When to use together |
|------|-------------|---------------------|
| ``gtm-plays-collection`` | Downstream | Once a trigger is identified and prioritized here, you select the matching "Play" from the plays collection to execute it. |
| ``signal-based-list-building-workflow`` | Parallel | The list building workflow handles the physical scraping and data aggregation; this taxonomy defines WHAT data should be scraped. |
| ``outbound-personalization-playbook`` | Downstream | The messaging frameworks provided here dictate the "Hook" that is written during the personalization workflow. |

## Suggested Skill Chains

1. Trigger Execution End-to-End: ``trigger-identification-framework`` (define the event) > ``trigger-detection-automation`` (build the scrape) > ``signal-triggered-plays`` (execute the sequence) > ``copy-atl-executive-messaging`` (write the email).
