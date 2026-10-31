# Nine-hour hackathon: Google plans, Qoder executes

Prepared for Monday, 2 November 2026: one person, 3,000 Qoder credits, and the
brief supplied on the day. You confirmed Qoder and Google Search AI are allowed.
Use prepared materials only if the assessment permits them.

The aim is to move requirements analysis, architecture, task breakdown and
rubric review to Google Search AI. Give Qoder the overall plan once and let it
implement related steps continuously, using local reasoning where needed.

## The workflow

1. Read the original brief and rubric yourself. Supply both originals, including
   the complete rubric PDF, to both tools.
2. Give Google Search AI the brief, rubric PDF and actual project facts using A.
3. Google produces the rubric checklist, design/contracts and ordered execution
   plan using B. You check it against the brief.
4. Save B's execution plan as `EXECUTION-PLAN.md` in the assessment project.
   Give Qoder the short rules and complete agreed plan using C. It can execute
   several related steps without a new user message for each one.
5. Run terminal checks and manual user flows yourself. Record real results.
6. At useful milestones, update the checklist from actual results. Consult Google
   when the plan needs revision, rather than after every file edit.
7. Qoder fixes straightforward local errors. Use Google and D for repeated
   failures, major uncertainty or decisions that would change the design.
8. Use Qoder E for one final criterion-by-criterion audit against the original
   PDF, then Google F for review using that evidence. Resolve the identified gaps.

Do not ask Qoder to re-plan, repeat full audits after every edit, estimate marks
or redesign Google's approach. It must still read the original rubric and check
full coverage before finishing. Avoid an unbounded "keep going until 100%" loop.

## Supply the rubric PDF to both tools

Attach the original PDF using the permitted interface if supported. If either
tool cannot read it, provide complete extracted text and readable images of any
tables, diagrams or scanned pages it cannot parse. Keep page references and
compare the extraction with the original yourself. Do not substitute a summary
that drops full-mark qualifiers. Stop planning until unreadable criteria are
resolved; do not silently treat them as satisfied.

Both tools should identify the rubric's page count, criteria, marks, full-mark
descriptors and submission constraints. Compare the extracted mark total with
any stated total and flag discrepancies. Preserve original IDs; assign stable
IDs only if the rubric has none. Aim to meet every full-mark descriptor, with
evidence. Neither tool can guarantee the lecturer's eventual grading.

## Give Google enough facts

Google Search AI cannot see your local repository. Supply the file tree,
manifest/dependency versions, run scripts, relevant starter files and exact
errors yourself. Start with small relevant excerpts, then provide complete
files when an exact replacement requires them. Do not send dependencies,
generated output or the whole repository by default.

If there is no starter, tell Google that explicitly. It can choose the simplest
stack allowed by the brief and specify the scaffold as the first Qoder task.
If a stack is mandated, do not spend time comparing alternatives.

Keep one Google conversation for planning. Before a new conversation, preserve
the current decisions, contracts, rubric checklist, latest files and blockers.
Search AI output can be wrong: compare requirements with the original text and
confirm implementation with executed checks. A claimed score is not evidence.

## A. Google Search AI: establish the plan

```text
I am working alone in a nine-hour software assessment. Only Qoder and Google
Search AI are allowed. Qoder has 3,000 credits. You handle requirements analysis,
architecture, task breakdown, diagnosis and rubric review. Qoder executes your
precise implementation plans with minimal additional planning.

Read the original brief and every page of the attached rubric PDF, including
tables and full-mark descriptors. Confirm page count and flag unreadable pages
or text; ask for missing source before claiming full coverage. Preserve explicit
requirements, marks, constraints and submission instructions. Do not invent facts.

Return:
1. A complete rubric checklist: ID, PDF page, exact requirement and full-mark
   descriptor, marks if supplied, and observable acceptance check. Compare the
   mark total with any stated total and flag discrepancies. Distinguish supporting
   tasks from marked items. Target every full-mark descriptor, not just a pass.
2. One simple implementation design compatible with the required stack/starter.
   Decide shared data shapes, interfaces and persistence behavior where needed.
3. Dependency-ordered batches covering every criterion, prioritizing required
   prerequisites and marks per effort. Include an early working end-to-end flow.
4. Only the essential missing project facts needed to specify the plan accurately.

Do not compare multiple architectures or write a long essay. Do not invent
existing filenames, dependency versions, commands or APIs. Clearly label any
new files/contracts you propose creating. Once essential facts are supplied,
prepare to turn the whole plan into the execution format I give you next.

ORIGINAL BRIEF AND RUBRIC PDF:
<attach/reference originals; paste complete text/page images if unreadable>

ACTUAL PROJECT FACTS:
<required stack, starter/no starter, file tree, manifest, scripts, relevant code>
```

Keep the checklist and decisions in a local `HACKATHON-STATUS.md` for yourself.
Google can format it; update it from actual results. Do not spend Qoder credits
regenerating it after every task. Include these fields:

```text
Deadline:
Credits remaining (measured by me):
Stack, run/check commands and agreed contracts:
Criterion ID/page | marks | full-mark requirement | milestone | evidence | check/result | gap
Current blocker and attempted fixes:
Submission requirements and delivery status:
```

Use actual criterion IDs and marks; leave unsupplied marks unknown. Distinguish
implemented behavior from verified behavior and checks not yet run.

## B. Google Search AI: produce the Qoder execution plan

Use this after the initial plan. Supply relevant current code when needed;
Google has no live repository view. Revisit only when the plan needs revision.

```text
Prepare one ordered Qoder execution plan from our agreed design and supplied
project facts. Settle major design decisions here. Group work into coherent
testable milestones and allow continuous execution between them. Do not require
a new user prompt after every file, feature or check.

The prompt must specify:
- Objective and every rubric ID/page, full-mark requirement and acceptance check.
  Map each criterion to at least one implementation/verification milestone.
  Include a final comparison with the original PDF and a complete evidence table.
- Existing files to read and files to create/change, grounded in supplied facts.
  If an existing path is unknown and not essential to the design, name its role
  and relevant symbol so Qoder can locate it with a targeted search.
- Required behavior and contracts; exact edits only where useful and supported
  by supplied code. Leave routine local implementation details to Qoder.
  Keep any replacement contents consistent with the latest code; preserve existing
  behavior. Do not reproduce large unchanged files unnecessarily.
- Final signatures, imports, data shapes, API payloads, validation, persistence
  and error behavior needed for each milestone. Omit irrelevant fields.
- Dependencies/commands only when supported by the brief and actual project.
- Observable acceptance checks, including relevant failure cases.
- Explicit exclusions, relevant checks, milestone reporting and the overall
  endpoint. Stop for essential blockers, design changes or repeated failures.

If an essential fact is missing, ask for that fact instead of making Qoder
investigate broadly. Do not invent existing code or leave important contracts
for Qoder to design. Do not make Qoder re-audit the plan or expand its scope.

CURRENT STATE:
<starter facts or latest milestone result, relevant code, check results, time>
```

Use milestones that you can review and check meaningfully. Group related edits
instead of paying for a request per file. Preserve every required
criterion across the batches; do not turn "minimal" into incomplete behavior.
Save the execution plan as `EXECUTION-PLAN.md`; keep the rubric checklist and
decisions in `HACKATHON-STATUS.md`. Save the original brief/rubric separately.

## C. Qoder: implement the supplied plan

Use `QODER-HACKATHON-RULES.md` as a short project rule or attach it to the chat.
Do not load this whole playbook as an always-applied rule. Preserve any supplied
assessment instructions rather than overwriting them.
Attach/reference the original brief and rubric PDF alongside the plan. Qoder
must read the originals once at the start and compare final coverage against
them. Assessment requirements take precedence over an incorrect plan.

```text
Apply the attached QODER-HACKATHON-RULES.md. Read the original brief, every page
of the rubric PDF and EXECUTION-PLAN.md. Flag unreadable source. Target every
full-mark descriptor and implement the plan in order. Continue through related
steps without asking after every task.
Use existing patterns for local details; do not redesign or expand scope.
Read relevant code only. Run agreed checks at milestones; fix straightforward
errors. Stop for missing essential facts, required design changes or two failed
repairs of the same issue. Keep prose terse. Report at milestones without
waiting for a reply. Before finishing, compare every original rubric criterion
with implementation/check evidence and report gaps; do not claim a guaranteed
score or treat unverified behavior as complete.
```

Inspect the diff and manually check required behavior at useful milestones.
Run routine terminal checks yourself where practical. Qoder can also run agreed
checks and repair straightforward failures; avoid unlimited repair loops.

## D. Google Search AI: diagnose and write the fix

```text
Diagnose this failure using the actual evidence. Do not send the diagnosis back
to Qoder as an open-ended investigation. If the cause is clear, produce an exact
minimal Qoder fix prompt using our execution format. If not, ask for the smallest
additional file excerpt or give me a specific diagnostic command to run first.
Do not guess, repeat a failed fix or change architecture without evidence.

TASK / RUBRIC REQUIREMENT: <ID and required behavior>
EXPECTED: <behavior>
ACTUAL: <behavior>
COMMAND / REPRODUCTION: <exact command or steps>
ERROR: <first useful error and relevant stack frames>
CURRENT RELEVANT CODE: <files/excerpts>
ATTEMPTED FIXES AND RESULTS: <facts>
```

Run the diagnostic commands yourself. Send the resulting narrow fix to Qoder,
then rerun the failed check yourself. Preserve full logs locally; send more
context if the initial excerpt does not establish the cause.

## E. Qoder: final audit against the original rubric PDF

Use once near the end if Qoder has not already produced this audit. Reuse valid
checks already run; rerun only when relevant changes or unresolved concerns
justify it. This is the final coverage check, not a request to redesign the app.

```text
Apply QODER-HACKATHON-RULES.md. Compare the current repository with the original
brief and EVERY page/criterion/full-mark descriptor in the rubric PDF. Do not
treat EXECUTION-PLAN.md or previous completion claims as proof. Flag unreadable
source. For every criterion return:
ID/page | full-mark requirement | marks if supplied | implementation path |
implemented/verified/partial/missing/blocked/unverified | actual check/result | gap.

Account for every criterion, including non-code deliverables and submission
constraints. Run agreed outstanding checks. Fix scoped omissions within the
existing design, rerun affected checks and update the table; stop for required
design changes or two failed repairs. Label checks needing human input, access
or observations unverified until I supply real results. Report remaining gaps
explicitly. Do not invent results, estimate awarded marks or guarantee 100%.
```

Keep the resulting table in `HACKATHON-STATUS.md`. Supply it to Google with
prompt F, plus current relevant code and real check results when needed.

## F. Google Search AI: review rubric evidence

```text
Read every page of the original rubric PDF and the original brief again.
Compare every full-mark descriptor with the current evidence below, including
Qoder's audit table. Flag unreadable source. For every criterion give:
ID/page | full-mark requirement | implemented/verified/partial/missing/unknown |
actual supporting evidence | remaining gap. Distinguish code claims from checks
actually run. You cannot inspect my local app; mark unsupported claims unknown
and tell me exactly what to inspect, run or supply. Do not invent a score.

Check submission requirements as well as application behavior. Prioritize gaps
by dependencies, marks, remaining time and regression risk. Produce the next
precise Qoder fix prompt only when current code/evidence supports it. Otherwise
give me the smallest fact-gathering step. Keep every criterion accounted for.

ORIGINAL BRIEF/RUBRIC PDF: <original attachments or complete readable extraction>
CURRENT EVIDENCE: <checklist, relevant code, commands/results, manual observations>
TIME REMAINING: <time>
```

## Token reduction: concise instructions and controlled context

- Give the complete agreed plan once. Do not confuse one user message with one
  model call: an agent can invoke the model repeatedly while executing it.
- Use short headings and precise requirements. Remove pleasantries, repeated
  explanations and duplicate rules. Preserve negations, exact identifiers,
  constraints and acceptance checks. Shorter prompts must remain unambiguous.
- Ask for terse reports rather than narrated edits or repeated full-file output.
  Caveman-style prose compression does not itself reduce code-reading or hidden
  reasoning tokens; added style rules can also consume input tokens.
- Keep file reads/searches relevant and command output bounded. Preserve complete
  errors locally so important diagnostic evidence can be retrieved when needed.
- Choose a cheaper capable model for small, well-specified edits. Use stronger
  reasoning when task difficulty or repeated failures justify its cost.
- Compare real credit consumption and correct completed behavior. Fewer words
  or fewer prompts alone do not prove a cheaper successful implementation.

References: [Qoder credit accounting](https://docs.qoder.com/Credits),
[Caveman author's limitations](https://raw.githubusercontent.com/JuliusBrussee/caveman/main/docs/HONEST-NUMBERS.md).

## Qoder settings and spending

A prompt cannot turn off internal reasoning or enforce a credit cap. Use the
available model/effort controls in your installed client: choose the cheapest
capable model and low reasoning effort, or disable thinking if supported, for
precise edits. Increase capability only when a concrete task requires it. Check
actual usage rather than assuming a short response means little computation.

Avoid sub-agents, premium orchestration, repo wikis and broad autonomous tasks.
Keep related edits together; use a new chat at a genuine task boundary with
only the short rules, execution prompt and necessary context. Do not repeatedly
restart a continuing fix and pay for rediscovery.

Current Qoder documentation lists a temporary free Efficient tier for eligible
paid users. Verify your event account's actual selector/rate and eligibility;
do not base the plan on receiving this offer or an unlimited free fallback.

Your selector showed these rates on 31 October. Recheck them on the day:

| Tier | Shown rate | Suggested use |
| --- | ---: | --- |
| Efficient | 0.0x | Start with a clear implementation task and verify the result |
| Auto | 0.5x | More involved work or when Efficient struggles |
| Fast | 0.8x | Faster turnaround; replaces the former Performance tier |
| Ultimate | 2.0x | A specific difficult blocker when cheaper attempts fail |

This is a suggested escalation order, not a guarantee of task quality or cost.
Source: [Performance became Fast](https://docs.qoder.com/product-overview/fast-mode-announcement).

| Qoder work | Credit envelope |
| --- | ---: |
| Scaffold and required implementation | 2,000 |
| Precise corrections from external diagnosis | 400 |
| Protected reserve for late required gaps/blockers | 600 |
| Total | 3,000 |

These are spending envelopes, not usage predictions or automatic limits. Check
balance before/after each batch and adjust using actual cost. With 600 credits
left, reserve them for required gaps and submission blockers.

Sources checked 31 October 2026:
[credit accounting](https://docs.qoder.com/Credits),
[model/effort controls and offers](https://docs.qoder.com/user-guide/chat/model-tier-selector),
[project rules](https://docs.qoder.com/user-guide/rules).
The installed client's available controls and displayed rates govern.

## Nine-hour schedule and submission

| Elapsed time | Work |
| --- | --- |
| 00:00-00:30 | Read brief; Google extracts rubric and specifies the design |
| 00:30-01:00 | Supply project facts; execute scaffold/baseline task; run it |
| 01:00-06:00 | Qoder executes the agreed plan; you check/save milestones |
| 06:00-07:30 | Google reviews evidence; execute specific gap fixes; verify integration |
| 07:30-08:15 | Required build/tests, manual flows, README and fresh-copy rehearsal |
| 08:15-09:00 | Complete and verify submission; use buffer for blockers |

- Track every original requirement, including documentation and non-code work.
- Run the required final checks and important user flows. Follow only the README
  in a fresh working copy to expose hidden setup assumptions.
- Use the new brief's deadline and submission/access rules; do not reuse the
  older practice sheet's 17:00 deadline automatically.
- If Git delivery is required, commit, push and verify the remote commit and
  required marker access before the deadline. Confirm the submission itself.
- Retain honest results: implemented is different from verified. Full marks
  depend on satisfying the actual rubric; no prompt can guarantee the score.
