# Nine-hour hackathon: full rubric coverage with less wasted work

Monday, 2 November 2026: one person, 3,000 Qoder credits. You confirmed Qoder and
Google Search AI are allowed. Prepared materials must follow the exam's rules.

Google handles overall planning. Qoder writes code using the actual repository.
You run routine commands, verify behavior, watch time/credits and submit. Target
every full-mark requirement with evidence; no prompt guarantees the lecturer's score.

## What to give each tool

- **Google:** original brief/rubric PDF, actual starter facts and relevant code.
- **Qoder:** original brief/rubric PDF, `EXECUTION-PLAN.md` and the short rules.
- **You:** this playbook. Do not attach the whole playbook as Qoder's standing rules.

Both tools need readable access to every PDF page, including tables, diagrams
and full-mark descriptors. If the permitted interface cannot read an attachment,
provide complete extracted text and readable images of affected sections. Check
against the original. Resolve unreadable requirements before claiming coverage.
Google cannot inspect local files unless you supply them. Distinguish proposed
new files/contracts from actual existing code; avoid speculative replacements.

## Human runs commands; Qoder keeps coding

Default ownership reduces routine agent orchestration; it does not remove the
required checks. You can explicitly delegate a command if that becomes faster.

| Work | Owner |
| --- | --- |
| Plan, interpret rubric, investigate difficult blockers | Google and you |
| Inspect relevant code, implement features, write required tests/docs, fix code | Qoder |
| Install dependencies, run scaffold/setup commands, start services | You |
| Run builds, lint/typechecks, focused tests and required full checks | You |
| Browser flows, configuration entry, Git commit/push and submission | You |

Qoder should batch commands at milestones, not ask after every edit. For each
command provide an ID, exact working directory, command and success condition.
Reuse commands already in Google's plan; Qoder only needs to cue their IDs unless
the command changes. Do not spend a new Qoder request on a command you already know.
Use scripts, dependencies and lockfiles actually present. Install once as needed;
repeat only if dependency inputs change or installation failed. Do not ask Qoder
to watch long logs or repeatedly poll a running command.

You run commands in your terminal and return one compact result message, for
example `H1 PASS; H2 FAIL: <first useful error and relevant stack frames>`.
Keep complete logs locally. Success should include the completed command's exit
status or requested behavioral observation, not just a server startup message.
Do not rerun checks already valid for unchanged code.

Qoder can continue independent work while a command runs. It must leave the
files/configuration being checked stable and avoid assuming a pending result.
Examples: while you check a completed backend flow, it can work on an unrelated
UI section; while dependencies install, it must leave the manifest/lockfile alone.
If shared inputs change, treat the result as outdated and rerun affected checks.
If no independent work remains, Qoder pauses for your result rather than spinning.
Wait for scaffolding to finish before editing generated files. Full-project
builds/test suites need stable relevant source/configuration; independent work
must genuinely fall outside those inputs.

Before submitting, you still run every required final check and important user
flow. Qoder must label evidence as human-run and keep pending/outdated checks
unverified. Writing required tests remains Qoder's job; running them is yours.

Local commands do not themselves spend Qoder credits. Model calls around tool
execution, log interpretation and repeated agent turns can consume tokens.
This division may reduce that overhead; the exact savings are not measured.

## A. Google: plan once

Give Google this prompt with the originals and project facts. It should produce
both the coverage checklist and executable plan in one response when possible.

```text
I am alone in a nine-hour assessment. Qoder has 3,000 credits. You handle overall
planning; Qoder implements against the actual repository. Optimize for correct
completion within time and credits, covering every full-mark rubric descriptor.

Read the original brief and every rubric PDF page, including tables. Confirm
page count and flag unreadable source or essential missing facts. Do not invent
requirements, marks or existing project details.

Return:
1. A compact COMPLETE coverage checklist: criterion ID/page | full-mark requirement
   (preserve every qualifier) | marks if supplied | implementation/check milestone.
   Preserve original IDs; assign stable IDs if absent. Compare the extracted
   marks with any stated total and flag discrepancies.
2. One ordered Qoder execution plan. Choose the simplest compatible approach;
   settle major design decisions and shared contracts. Include an early working
   end-to-end flow and meaningful verification milestones. Cover every criterion,
   required technology, non-code deliverable and submission constraint.
3. For each milestone specify required behavior, relevant files/roles, necessary
   data/API contracts, validation/error cases and observable acceptance checks.
   Use actual commands where known; distinguish proposed new scripts/dependencies
   from existing ones. Leave routine local coding details to Qoder. Do not write
   the whole application here or compare multiple architectures.

Allow continuous execution without user approval after every task. Assign routine
setup/install, scaffolding commands, servers, builds, lint/typechecks, tests and
Git writes to me. Read-only code inspection/search/diffs are allowed. Qoder writes
code/tests and batches exact human commands
with working directories and success conditions at milestones. It continues
independent work while I run them, keeping checked inputs stable. Pause only for
essential dependencies/blockers; do not assume results. Require focused checks,
bounded repairs and ONE final complete rubric evidence table
IN CHAT ONLY. No separate audit/status/planning files generated by Qoder.
Include documentation/tests explicitly required by the rubric or necessary to
run and verify the work. Stop for essential blockers, required design changes
or two unsuccessful repairs of the same failure.

If missing facts prevent a correct plan, ask only for those facts. Otherwise
produce the complete plan now. Label unknowns; do not invent certainty or scores.

ORIGINAL BRIEF/RUBRIC PDF: <attach/reference originals>
PROJECT FACTS: <required stack, starter/no starter, tree, manifest, scripts, code>
```

Check the response against the original yourself. Save only the execution plan
as `EXECUTION-PLAN.md` in the assessment project, ready for Qoder. Keep Google's
checklist and decisions in the same Google chat or your own notes. A human-held
`HACKATHON-STATUS.md` is optional; Qoder must not maintain it for you.

## B. Google: repair the plan only if needed

Skip this when A produced a complete usable plan. Do not pay the time cost of
re-planning a correct approach or generating an unnecessary second full version.

```text
Resolve these specific gaps in our existing plan using the original rubric and
new facts below. Return only the changed sections and affected criterion IDs.
Preserve valid decisions and coverage. Do not redesign or repeat unchanged text.
If an essential fact remains missing, ask for it rather than guessing.
GAPS / NEW FACTS: <exact issues and current relevant code/project facts>
```

Update your saved execution plan yourself before starting Qoder. If changing a
plan during implementation, give Qoder only the relevant revision and context.

## C. Qoder: implement continuously

Attach/reference the original brief, full rubric PDF, saved execution plan and
`QODER-HACKATHON-RULES.md`. Preserve any supplied assessment instructions.

```text
Apply QODER-HACKATHON-RULES.md. Read the original brief, full rubric PDF and
EXECUTION-PLAN.md. Target every full-mark descriptor and implement the plan
continuously. Use relevant code and existing patterns; do not re-plan or expand
scope. I run routine setup/install, servers, builds, tests and Git writes.
Batch exact commands with IDs/working directories/success conditions at milestones;
continue independent coding while my checks run, leaving checked inputs stable.
Wait for actual results before claiming verification; request affected reruns
after fixes and mark stale results outdated. Fix straightforward failures. Stop
for essential blockers, a required design change or two unsuccessful repairs
of the same failure. Keep prose terse; do not await replies after progress reports.
Before finishing, check every rubric criterion and fix scoped omissions. Return
ONE complete evidence table IN CHAT ONLY. Do not create audit/status documents
or repeat the table in a summary. Produce required assessment deliverables.
```

Try the important behavior and inspect changes at useful milestones. Run routine
terminal commands yourself by default and batch results back to Qoder. Save
working Git checkpoints. Keep real results; distinguish human-run checks from
Qoder's code inspection and pending checks from verified behavior.

## D. Google: diagnose persistent blockers

Use when Qoder is stuck or the agreed design needs reconsideration. Google needs
current code and actual errors; it does not have a live repository view.

```text
Diagnose this failure from evidence. If the cause is clear, give one narrow
Qoder fix prompt specifying the change and acceptance check. If unclear, ask
for the smallest additional excerpt or give me a diagnostic command to run.
Do not guess, repeat a failed fix or redesign without evidence. Return only
what is needed to unblock implementation.
CRITERION / EXPECTED BEHAVIOR: <ID and required behavior>
REPRODUCTION / COMMAND: <exact steps or command>
ACTUAL / ERROR: <first useful error and relevant stack frames>
CURRENT CODE: <relevant files/excerpts>
ATTEMPTS AND RESULTS: <facts>
```

Let Qoder apply the focused code fix; you run the affected checks. Preserve full
logs locally so you can supply more diagnostic context when needed. Do not send
irrelevant log dumps by default.

## E. Qoder: final audit only if not already done

C already requests the audit. **Skip E if that final audit exists.** Reuse valid
human results; Qoder requests outstanding checks for you to run. Do not redo the
complete audit after each localized fix. Use affected-row updates instead.

```text
Apply QODER-HACKATHON-RULES.md. Check the repository against every original
brief/rubric criterion and full-mark descriptor. Flag unreadable source. Reuse
valid human-run results, batch outstanding commands for me and fix scoped
omissions within the existing design. Stop for required design changes or two
failed repairs.
Return ONE complete compact table IN CHAT ONLY:
criterion ID/page | implementation evidence | actual check/result | remaining gap.
Include every criterion and non-code/submission requirement. Attribute human-run
checks; mark pending/outdated/blocked/unverified items, including results I have
not supplied. Do not invent results, award marks, create audit/status files or
duplicate the table elsewhere.
```

Copy the response to Google for F. Save it yourself if useful; do not ask Qoder
to write the same report into the repository. Required assessment documentation
is still required: this restriction concerns extra process/audit paperwork.

## F. Google: review coverage, return gaps only

Google reviews the whole rubric against Qoder's final evidence. It should report
only actionable gaps or confirm no gaps identified in supplied evidence, rather
than print a second complete table. Supply current code/results if requested.

```text
Compare EVERY original brief/rubric full-mark descriptor with the evidence below.
Flag unreadable source. Check all criteria, including submission and non-code
work. Do not accept unsupported completion claims or invent a score.
Return ONLY gaps, contradictions or missing verification: criterion ID/page,
what is missing, smallest next check/fix, priority. If no gaps are identified in
supplied evidence, say so without claiming a guaranteed score. Do not duplicate
Qoder's complete table. For a supported fix, give a focused Qoder prompt; for
uncertainty, request the smallest missing fact/code/result first.
ORIGINAL BRIEF/RUBRIC: <original attachments or complete readable extraction>
EVIDENCE: <Qoder final chat table, actual results, relevant code as needed>
TIME / CREDITS REMAINING: <actual values>
```

After a fix, update affected criteria only. Repeat broader checks/review when
cross-cutting changes or unresolved concerns invalidate earlier results.

## Credit and time controls

- One user prompt can trigger many model calls. Compare actual credit usage and
  correct completed work, rather than prompt count or reply length alone.
- Give the complete plan once. Keep related work in the same conversation.
  At a genuine new task/context boundary, provide a concise current-state handoff.
- Use terse precise instructions and reports. Preserve qualifiers, negations,
  identifiers and test evidence. Do not install elaborate compression machinery
  during the exam; shorter prose alone does not reduce all agent/token costs.
- Keep file reads and tool output relevant. Avoid repeated repository scans,
  sub-agents, repo wikis, duplicate reports and unlimited repair loops.
- Run routine commands yourself and return batched results. Let Qoder use its
  model calls for code and necessary diagnosis, with stable inputs for human checks.
- A prompt cannot enforce credit caps or turn off internal reasoning. Watch the
  actual account balance and use available model/effort controls.

Your selector showed these rates on 31 October; recheck on the day:

| Tier | Shown rate | Suggested use |
| --- | ---: | --- |
| Efficient | 0.0x | Start with a well-specified task; verify quality and speed |
| Auto | 0.5x | More involved implementation or when Efficient struggles |
| Fast | 0.8x | Faster turnaround; successor to Performance |
| Ultimate | 2.0x | A specific difficult blocker when cheaper attempts fail |

The free Efficient offer has eligibility/availability conditions. Do not rely on
it remaining available or on free use eliminating the nine-hour time constraint.

| Spending envelope | Credits |
| --- | ---: |
| Required scaffold and implementation | 2,000 |
| Focused corrections | 400 |
| Protected reserve for late gaps/blockers | 600 |
| Total | 3,000 |

These are envelopes, not forecasts or automatic limits. At 1,200 remaining,
review outstanding requirements and stop optional polish. Preserve the last 600
for required gaps and submission blockers. Never drop an explicit rubric item
merely to save tokens; remove unnecessary process work first.

| Elapsed time | Target |
| --- | --- |
| 00:00-00:30 | Read originals; Google produces coverage and plan |
| 00:30-01:00 | Resolve essential facts; start runnable baseline and submission setup |
| 01:00-06:00 | Qoder codes; you run batched commands/checks and save milestones |
| 06:00-07:30 | One final Qoder audit; Google gap review; scoped fixes |
| 07:30-08:15 | Final checks, manual flows, required README and fresh-copy rehearsal |
| 08:15-09:00 | Submit and verify delivery; retain buffer for blockers |

Use the actual deadline and submission rules supplied on the day, rather than
the older practice sheet's 17:00 cutoff. Follow the app's required run instructions
in a fresh copy. If Git delivery is required, commit, push, verify the remote
commit/access and complete the submission action before the deadline.

Credit accounting rechecked 1 November 2026; other sources checked 31 October:
[credit accounting](https://docs.qoder.com/Credits),
[model controls/offers](https://docs.qoder.com/user-guide/chat/model-tier-selector),
[Performance became Fast](https://docs.qoder.com/product-overview/fast-mode-announcement),
[Caveman limitations](https://raw.githubusercontent.com/JuliusBrussee/caveman/main/docs/HONEST-NUMBERS.md).
The current account selector, actual usage and exam requirements govern.
