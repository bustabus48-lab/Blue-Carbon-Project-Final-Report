# Prompt: Authoring Layer for Final Report and Standalone Source Reports

Use this prompt after extraction, synthesis, and chapter drafting are complete.

## Objective
Turn evidence-based draft material into a readable report output for:
- policy makers
- academics
- development partners

This prompt can be used for:
1. a final-report chapter polishing pass;
2. a standalone National MRV Report;
3. a standalone Drone Survey / EOSDA monitoring report; or
4. a standalone Carbon Inventory Report.

## Inputs
- approved blueprint
- relevant chapter draft or drone-survey draft
- completed National MRV Report in markdown, if MRV findings are being carried into the Final Report
- completed Drone Survey / EOSDA Report in markdown, if drone-monitoring findings are being carried into the Final Report
- completed Carbon Inventory Report in markdown, if carbon findings are being carried into the Final Report
- extraction notes and synthesis matrix entries used for that draft
- issue log and decision log entries that affect the text
- any approved figures, tables, screenshots, or polygon inventories

## Instructions
- Preserve all evidence-backed findings and remove unsupported wording.
- Rewrite technical guidance into plain, decision-oriented prose without adding new facts or deleting essential scientific meaning.
- Define acronyms on first use.
- Keep detailed methods short in the main text and move technical detail to annex notes or placeholders.
- Mark missing information with bracketed placeholders and name the missing source or missing implementation input.
- If one of the three standalone reports is still incomplete, keep the text at placeholder status rather than implying that the evidence package is complete.
- Distinguish clearly between:
  - completed evidence
  - pending inputs
  - interpretive synthesis
  - recommendations
- When preparing a standalone National MRV Report, distinguish national framework design from site-specific implementation depth.
- When drafting the Drone Survey / EOSDA monitoring report, state whether the following are completed, pending, or unknown:
  - EOSDA account setup
  - Uploaded areas of interest / polygons
  - Drone orthomosaics or imagery packages
  - Screenshots or interface evidence for continuous monitoring
  - Reporting workflow for recurring updates
- When preparing a standalone Carbon Inventory Report, identify whether full carbon stock tables, methods, and approved numbers have been supplied by the carbon team.
- Do not claim continuous monitoring is operational unless the evidence explicitly shows setup and use.

## Output requirements
- Use headings and short paragraphs.
- Use tables where they reduce repetition.
- End with a concise section titled `Decisions, pending inputs, and next actions`.
- Make the text readable as a report, not as process notes.
