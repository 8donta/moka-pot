# Baseline, experiments, taste diagnosis, and memory

## Intake and measurements

Collect the setup described in SKILL.md in small batches. Include the stove in the opening questions, for example: "Which pot/model and cup size do you have? What stove or heat source do you use: gas, electric coil, ceramic/radiant glass, induction, or the pot's own electric base? What roast and exact grinder are you using, and do you have a scale, timer, and thermometer?" Ask whether to use a local brew journal or chat-only tracking during the same setup exchange. Adapt to what is already known rather than repeating this verbatim.

Follow up on the stove's burner size, power controls or numbered settings, and any adapter plate before suggesting a heat schedule. An induction-compatible pot does not establish that the user has an induction stove. If the heat source is unknown, continue other intake but defer heat-specific recommendations until it is identified.

Unknown capacity: inspect the marking/manual and measure water and coffee independently. If the model is uncertain, do not infer its valve, fill limit, or heat compatibility. Missing measurement tools: prepare the profile and explain general technique, but defer controlled comparisons. A timer can be a phone; temperature measurement must not involve opening a pressurized pot.

Use grams, degrees C, and seconds internally; accept and convert other units while retaining the user's original reading. Do not invent precision beyond the scale, thermometer, or grinder. A protective trivet can be tared with a cup to weigh the decanted beverage. Use equipment rated for the temperature and measure promptly and consistently.

Define the clock consistently:

- `t0`: pot placed on the active heat source (record whether the burner/plate was preheated).
- `t1`: first visible coffee at the outlet.
- `t2`: final removal/switch-off to end brewing, distinct from temporary heat cycling.
- `t3`: flow actually stops under the chosen stop/cooling method.
- Time to first flow = `t1 - t0`; flow duration = `t3 - t1`; total duration = `t3 - t0`. Record `t2` and any flow continuing afterward. Do not redefine these between trials.

Measure water mass and its temperature immediately before final assembly, coffee dose, and decanted beverage mass. Record the pot's starting condition (cooled to room temperature versus still warm), basket prep, paper filter, stove/plate state, heat settings, control rule, endpoint, cooling method, and serving additions. Cool and reset the pot and heat source consistently between comparison brews; a hot second pot/plate can confound a water-temperature test.

Coffee-to-input-water and coffee-to-beverage-output ratios are different derived values. Neither is extraction percentage. An input change can alter the loose basket volume or beverage yield; record those effects rather than silently changing another input to compensate.

## Choosing and specifying a trial

Stabilize leaks, stalls, violent flow, and inconsistent assembly/preparation before taste optimization. Once stable, select the input most relevant to the user's observations. There is no compulsory sequence, but grind is a useful first taste trial when adjustable and flow is controlled; starting temperature can then test the creators' disagreement. Water/dose/filter/endpoint/serving experiments are optional, not required milestones.

A trial card should contain:

| Field | Required meaning |
| --- | --- |
| Reference | ID of the current preferred recipe/brew; baseline B0 before a preference exists. |
| Hypothesis | The observed problem and why this one change might help. |
| Changed input | Old value -> new value in meaningful equipment units. |
| Constants | Same beans, water source, pot state, other recipe inputs, heat rule, endpoint, and serving, except the named input. |
| Expected observations | Tentative taste/flow effects and which measurements to report. |
| Stop rule | Observable endpoint and model-approved handling. |

Choose the smallest useful, repeatable adjustment. For a known stepped grinder this may be one documented step; for an unknown dial, establish its direction and units before naming a number. Never force beyond a grinder's documented range or mechanically tight zero. If no verified recommendation exists, an accurately recorded user-known setting can anchor relative trials; say that its suitability is unverified. With fixed preground coffee, choose another variable. Changing product/beans is a new baseline, not a grind-only test.

For a temperature comparison, use measured values ("room temperature" alone is not a repeatable number), the same water mass, same initial pot/plate condition, same grind, same heat-control rule, and same endpoint. Heating duration and number of heat cycles may differ as responses to the same rule. If heat settings or the response rule are also changed, mark the result confounded rather than crediting temperature alone.

For a time investigation, change one defined input: for example, lower the flow-phase heat setting while retaining the same endpoint. Report resulting flow time and yield. Do not prescribe "make it last longer" plus a finer grind, hotter water, and a larger yield. An endpoint test changes the endpoint alone; a filter test changes the filter alone. Do not automatically compensate a new filter with a coarser grind in the same trial.

Taste comparisons should use the same stirring, approximate tasting temperature, and milk/water/sugar additions. A dilution test changes serving dilution alone, not the brewing recipe. Trying a sip with water is a concentration diagnostic; distinguish it from a controlled extraction experiment. Never require drinking all of several brews to complete a comparison.

## Taste-led hypotheses

Use the strongest combination of taste, flow, and recipe evidence. Give one next test, not every possible remedy. The table is a reasoning aid, not an automatic diagnosis.

| Report | Clarify or inspect | Example single next test when supported |
| --- | --- | --- |
| Unpleasant sourness, thin cup, fast otherwise stable flow | Pleasant fruit acidity or sharp unpleasant sourness? Same serving temperature and dilution? Is grind unusually coarse? | Go one small finer step with all other inputs fixed; test for more sweetness and less sharpness. |
| Sour but concentrated and enjoyable apart from intensity | Is acidity actually the problem, or just strength? | A measured serving-dilution test; explain that this changes concentration, not extraction in the pot. |
| Bitter with a rapid, aggressive flow or harsh tail | Heat rule and endpoint; was the brew allowed to sputter for a long time? | Test a gentler flow-phase heat schedule OR an earlier endpoint, selecting one. |
| Bitter with stable flow and no harsh tail | Roast character, grind, starting temperature, desired body, old coffee/oils | Depending on evidence, test one coarser step OR a lower starting temperature. Explain uncertainty; do not assume bitterness proves excess extraction. |
| Drying/astringent, rough finish | Distinguish mouth-drying from bitter taste; inspect fine grinding, uneven prep, and late sputtering | If grind is the likely cause, test a small coarser step. If preparation varied, first repeat a stable baseline instead. |
| Sour and bitter together | Uneven flow/preparation, excessive heat, coffee character, concentration, and serving | Stabilize the clearest observed problem; do not reflexively go finer or change several inputs. |
| Weak/watery but balanced | Beverage mass, dose, serving dilution; separate weak strength from sour underextraction | If diluted, test less serving water. Otherwise select a permitted endpoint trial or another supported input; do not change dose and water together. |
| Fast flow without bad taste | Is the user satisfied? | Keep the recipe; speed alone does not require correction. |
| No flow, leaking joint, or valve venting | Potential assembly/obstruction/model issue | Stop heat, cool fully, follow manufacturer inspection instructions; no flavor experiment until resolved. |

Ask for overall enjoyment and comparison with the reference, not only bitter/sour labels. An optional 0-5 scale for attributes and 0-10 enjoyment can make trends easier to compare; do not force numeric taste scores when plain language is more useful.

## Decision and confirmation

- **Baseline:** first adequately recorded brew, with confidence limited if not repeated.
- **Candidate:** a promising improvement reported once. Retain the previously confirmed preference separately.
- **Accepted:** a candidate repeated under the same conditions with consistent preference. Compare at similar serving conditions; this is practical confirmation, not proof of a universal optimum.
- **Rejected:** worse than the reference; return to the previous preference for the next trial.
- **Inconclusive:** multiple input changes, changed beans, unclear/missing observations, or a contradictory repeat. Do not overwrite the preferred recipe. Identify the issue and repeat the candidate or reference as appropriate.

Track settings within a complete recipe, not an unqualified list of "best grind" or "best temperature." Later changes may alter earlier preferences. Revisit with another one-input trial from the current recipe. Do not erase a failure or reinterpret it as a success to make progress appear linear.

If the user accepts a recipe after only one brew or skips confirmation, respect the decision but record the recipe as preferred/unconfirmed. If the user is happy, provide the recipe and stop; do not invent another problem to optimize.

## Memory modes and journal format

Ask for the session's mode before saving or loading personal brew history. If local tracking is chosen, use the active project's `brew-journal/moka-pot/`. If a project root or filesystem access is unavailable, offer chat-only tracking with a portable summary and explain the limitation. Do not write to another workspace or claim a save succeeded when it failed.

Keep one readable Markdown profile per pot + grinder + heat-source combination, for example `brew-journal/moka-pot/moka-express-3cup-kinu-gas.md`. Choose a descriptive filename using only known facts; avoid collisions by adding a suffix, and never overwrite a different setup. Within a profile, keep separate coffee runs/baselines when beans change. Choose the relevant profile from known setup details; if several match, ask the user which one to resume.

Use these sections and fields; omit unknown values only when they are explicitly marked unknown elsewhere:

1. **Equipment and session context:** profile identifier, pot/model/material/size, measured fill constraints and manual source, grinder variant/calibration/direction and setting source, heat source/adapter, measurement tools, water source, serving preferences, current memory choice.
2. **Coffee run:** bean identity, roast/freshness/process/decaf, start date, baseline ID, and any equipment or coffee changes. Dates use the user's local date when known.
3. **Baseline and preferred recipe:** complete measured recipe, baseline ID, preferred brew ID, current candidate if any, accepted versus unconfirmed status, confidence and limits. Preserve old baselines and winners as history.
4. **Trial history:** append chronological entries with unique IDs such as B0 and T1, date, reference ID, hypothesis, exactly changed input and old/new values, full recipe or reference plus explicit difference, reported times/yield/flow/taste, other deviations, decision, and explanation. Keep enough recipe detail to reconstruct each brew.
5. **Next step:** unresolved questions, proposed one-input trial or confirmation repeat, and why it is next. A proposal is not an observed result.

Update after the user reports a brew or changes/corrects profile information; do not save invented measurements, tastings, approvals, or an unbrewed proposal as a completed trial. Read the existing profile before editing, preserve history, and correct errors explicitly. After a successful write, briefly identify the journal saved and summarize the preferred/candidate status.

At each new session, ask the memory-mode choice again unless supplied in that session. Before reusing history, confirm the current setup and coffee, then ask what changed; do not force the user through full intake again. A changed bean or major component creates a new baseline while retaining old data. If a new session selects chat-only, do not read or update prior personal journal files unless the user separately asks to load them.

Chat-only mode writes no personal brew records. At the end or on request provide a copyable summary with setup/beans, baseline, current preferred and candidate recipes, completed trials and decisions, unresolved questions, and next test. Explain that a future chat needs this summary to resume reliably. Apply the same summary format if the user wants to export a local session. No mode promises invisible cross-chat memory.
