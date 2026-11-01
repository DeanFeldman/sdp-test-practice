# Nine-hour hackathon: Google plans, Qoder checks once and implements

For Monday, 2 November 2026: one person, 3,000 Qoder credits. You confirmed Qoder
and Google Search AI are allowed. Prepared materials must follow the exam's rules.

The rehearsal exposed errors in Google's proposed technical details. Use Google
for complete rubric coverage, priorities and a proposed architecture. Give Qoder
one bounded technical preflight, then use its effort for implementation. You run
routine commands, provide real results and submit. This workflow aims to reduce
avoidable work; actual time/credit savings and the eventual score are not guaranteed.

## Inputs and Gitea

Give both tools the original brief and full rubric PDF, including every page,
table and descriptor. Resolve unreadable source with complete text/page images;
verify extraction against the original. Google cannot inspect local code unless
you provide the relevant tree, manifest, scripts and excerpts.

Supply the actual **Gitea exam repository URL and target branch**. This prep repo
is separate. Use ordinary Git, preserve external sample/input URLs from the brief,
and add hosting/CI integrations only when required. You handle commits, pushes,
marker access and the submission action; a clean tree alone does not prove delivery.

Google chooses one suitable proposed architecture, following mandatory stack and
starter constraints. It should not ask you to choose frameworks. Qoder checks
technical correctness against reality and corrects concrete errors while preserving
scope and valid decisions. Major architectural changes go back to you/Google with
evidence and one minimal recommendation. Do not insist on implementing a known flaw.

## A. Google: plan once

```text
I am alone in a nine-hour assessment with 3,000 Qoder credits. You are the overall
planner responsible for a complete, technically consistent implementation plan.
Qoder implements it. I run routine commands and submit through my supplied Gitea
repository/branch.

Read every original brief/rubric PDF page, including tables and full-mark
qualifiers. Confirm readable coverage; flag missing source and essential unknown
facts. Preserve actual weights, formulas, constraints and submission requirements.
Do not invent existing files, benchmarks, expected results or commit hashes.

Return the complete contents of one file named exactly EXECUTION-PLAN.md, in
Markdown, inside one copyable code block. Use inline code for commands; avoid
nested code fences. No introductory/closing prose. I will save the file myself;
do not claim to have saved it on my computer. Include all of the following in
that single file, using descriptive Markdown headings and checklist tables:
1. A compact COMPLETE checklist: criterion ID/page | full-mark requirement |
   weight if supplied | implementation/check milestone. Preserve every qualifier,
   cumulative tier dependency and non-code requirement. Flag mark discrepancies.
2. One suitable proposed architecture: stack/libraries, modules, data/storage
   responsibilities, important interface behavior and relevant performance strategy.
   Follow supplied starter/stack constraints; otherwise make the choices yourself.
   No menu of alternatives. Make overall design choices; leave exact schema DDL,
   parser implementation, dependency versions and executable commands to Qoder
   using the actual project. State uncertainty instead of guessing.
3. One ordered execution plan, with milestone time targets fitting the stated
   assessment duration and a final submission buffer. Cover every criterion;
   establish a working end-to-end flow early and address risky core logic early.
4. Required behavior, shared contracts, error/empty/boundary cases and observable
   acceptance checks per milestone. Cross-check keys/scoping, filter semantics,
   examples for consistency. Leave local coding details to Qoder;
   do not generate the whole application's code here.

Before returning the file, review and correct your draft against the originals:
- Trace every full-mark qualifier to concrete behavior and an acceptance check.
  Where the brief defines formulas, preserve each formula, denominator, units,
  boundary and zero/empty case explicitly; category names alone are insufficient.
- Choose one implementation approach per decision, with no unresolved "X or Y".
  Prefer the simplest suitable design; avoid duplicate sources of truth and
  unnecessary dependencies. Check compatibility with the supplied environment.
- Walk through one normal, empty and boundary example for critical calculations
  and combined filters. Check time basis, inclusive/exclusive bounds, identities,
  aggregation and isolation where relevant. Fix inconsistent results/contracts.
- Check keys and foreign keys against repeated imports and entities shared across
  users/projects/repositories where applicable. Trace UI action -> API request ->
  stored data/computation -> response. Supply missing essential contracts.
- Check important library/CLI semantics your design relies on using official
  documentation available through search. Do not invent flags or claim execution.
  Do not generate speculative shell commands or machine-specific paths. Resolve design/semantic
  questions yourself before handoff. Only facts that
  require access to the actual local starter may be marked LOCAL FACT TO CHECK,
  with the exact file/fact needed. Flag other unresolved essentials as blockers;
  do not delegate your planning checks to the implementer or invent answers.
- Separate supplied facts from proposed scripts, benchmarks and assumptions.
  Preserve exact reference versions/hashes and expected results when provided;
  flag missing fixtures/results. No invented performance guarantees. Validate
  risky behavior during implementation, rather than only at submission time.
- Include planning, project setup, human command time, incremental checks, repairs
  and final delivery in the time budget. Specify what human checks must establish;
  Qoder supplies actual command IDs, directories and commands during implementation.
  Preserve
  required repository visibility/access and the actual submission action.
Apply corrections before output. Do not print your review process or another
audit report. Put only remaining material uncertainties in a short Open Blockers
section. A self-review is not proof that code runs or the plan is error-free.

Assign installs/scaffolding commands, servers, builds, lint/typechecks, test runs,
Git writes and browser checks to me. Qoder writes required code/tests/docs and
cues batched commands with IDs, directories and success conditions. Allow its
independent work while my checks run, with checked inputs stable. Keep reports
terse, repairs bounded and one final criterion evidence table IN CHAT ONLY.
Do not require Qoder to re-plan, create extra process documents or repeat audits.

Use Gitea delivery and ordinary Git; do not assume GitHub tooling/Actions.
Keep external sample/input URLs required by the brief. Ask only for missing
facts that materially block a correct plan; otherwise produce the plan now.

ORIGINAL BRIEF/RUBRIC: <attach/reference full originals>
PROJECT FACTS: <mandated stack, starter/no starter/unknown, tree, scripts, code>
GITEA EXAM URL / BRANCH: <actual values or unknown>
```

Check coverage yourself. Copy the entire Markdown block (including the rubric
checklist) into a new text file in the **exam project's root folder**, named
exactly `EXECUTION-PLAN.md`. Save as UTF-8 plain text, without the surrounding
code fences; check it is not named `EXECUTION-PLAN.md.txt`. Google supplies the
contents; you save it. No Qoder request or Google Docs/PDF conversion is needed.
For the old Test 1 rehearsal, explicitly override nine hours with its stated
2.5 hours; tomorrow's actual brief remains authoritative.

## B. Google: focused plan correction only if needed

```text
Resolve these concrete gaps/preflight findings using the original rubric and
actual facts. Return only changed sections of EXECUTION-PLAN.md and affected
criterion IDs in one copyable Markdown code block, retaining their headings. Preserve
valid architecture, coverage and my Gitea remote/branch. Choose one minimal
correction where a design change is necessary; do not offer framework menus or
repeat the whole plan. Ask only for essential missing facts. Keep Qoder's coding
work and my routine command work separate. Before responding, check each repair
against the original requirements and affected schema, API, examples, commands
and checks; update those affected sections together. Resolve technical decisions
yourself. List only essential unresolved factual blockers, with a precise question.
FINDINGS / NEW FACTS: <exact issues and relevant current code/results>
```

Use the same Google chat. Replace the affected sections in `EXECUTION-PLAN.md`
yourself, then transfer only relevant corrections back to Qoder.

## C1. Qoder: quick local blocker check

Google owns detailed plan validation. C1 is one narrow read-only pass, targeting
roughly 1-2 minutes, not a guaranteed time or credit cap. Use the implementation
model (Efficient if available at 0.0x); no automatic Auto escalation for C1.
Provide the plan, short rules and starter context. Keep originals available for
implementation; C1 does not re-extract the rubric or redo Google's analysis.

```text
Read QODER-HACKATHON-RULES.md once. Run only its quick C1 check on
EXECUTION-PLAN.md and relevant starter facts. No implementation or full audit.
Return the prescribed status and only actionable blockers/corrections.
```

For READY or READY WITH CORRECTIONS, continue to C2 in the same chat; Qoder applies
its concrete local corrections without asking you to choose technical details.
For RETURN TO GOOGLE, paste its findings into Google B, update the affected plan
sections and give the response to Qoder. It checks those affected issues only
before dependent implementation; no repeated full preflight or extra paperwork.

## C2. Qoder: implement continuously

Use the **same Qoder chat**. Try Efficient if its actual rate is 0.0x for
well-specified work; use Auto for difficult core logic or repeated failures.
You select the model. The prompt cannot switch tiers or enforce a credit cap.

```text
C2: continue under the rules already loaded. Implement EXECUTION-PLAN.md with
the C1 corrections, using the original brief/rubric as authority. Read originals
once if not already read. Reuse context; work continuously through milestones.
Cue my command batches when needed. Finish with the rules' single chat evidence
table. No repeat planning, C1 or extra process documents.
```

You run commands in your terminal. Reply in one batch, e.g. `H1 PASS (exit 0);
H2 FAIL: <useful error/stack frames>`. Preserve full logs locally. An empty log
or server startup alone does not prove required behavior. Qoder labels your
results human-run, and pending/outdated checks unverified.

Install again only when dependency inputs change or installation failed. Do not
pay for repeated polling, lengthy successful logs or commands you already know.
While an isolated backend check runs, Qoder can work on unrelated UI files; full
project checks need all relevant inputs stable. If no independent work remains,
it pauses for your result. Wait for scaffolding before editing generated files.
You can explicitly delegate a command when that is more practical.

## D. Google: persistent blocker

After two unsuccessful Qoder repairs of the same failure, stop the loop. Supply
current code and actual errors; Google does not have a live repository view.

```text
Diagnose from evidence. If clear, return one narrow Qoder fix prompt with the
minimal change and acceptance check. If unclear, request the smallest missing
excerpt or give me a diagnostic command to run. Preserve valid architecture,
requirements and my Gitea delivery target; propose a major change only with
evidence. No repeated failed fixes, full re-planning or duplicate reports.
CRITERION / EXPECTED: <required behavior>
COMMAND / STEPS: <exact reproduction>
ACTUAL / ERROR: <useful error and relevant stack frames>
CURRENT CODE / ATTEMPTS: <relevant excerpts and actual results>
```

Qoder applies the fix; you run affected checks and report results. Use Auto
for a focused difficult repair if Efficient was unable to implement a clear fix.

## E. Qoder: final audit only if missing

C2 already requests this. **Skip E if the complete final audit exists.** Reuse
valid human results and update affected rows after localized fixes.

```text
If the rules' final rubric reconciliation/table already exists, report only
changed gaps/results; do not repeat it. Otherwise perform it once now, reusing
originals, current code and valid results. Fix scoped gaps and cue missing human
checks. Table IN CHAT ONLY; no extra documents or invented results/marks.
```

## F. Google: review evidence, return gaps only

```text
Compare EVERY original full-mark requirement with the evidence below. Report
ONLY actionable gaps, contradictions or missing verification: ID/page, gap,
smallest next check/fix, priority. Verify coverage of non-code and Gitea delivery
requirements too. If no gaps are found in supplied evidence, say so without a
score guarantee. Do not repeat Qoder's table or trust unsupported completion
claims. Return a focused fix prompt only when current evidence supports it;
otherwise request the smallest missing fact/code/result.
ORIGINALS: <original brief/rubric>
EVIDENCE: <Qoder final chat table, human results and relevant code>
TIME / CREDITS REMAINING: <actual values>
```

Save chat reports yourself if useful. A human-held status file is optional.
Repeat broad review only when relevant cross-cutting changes or unresolved
concerns invalidate previous evidence. Produce every deliverable the rubric
requires; skip extra process paperwork.

## Credit controls and model choice

One prompt can trigger many model calls. Credits depend on model/token activity,
not local command execution time alone. Measure balance before C1 and after
working milestones. Do not infer savings from terse prose or fewer user messages.

| Use | Starting choice |
| --- | --- |
| Quick local C1 check | Same model as implementation; Efficient if it shows 0.0x |
| Well-specified implementation and repetitive edits | Efficient if it shows 0.0x |
| Difficult core logic, or a clear fix Efficient cannot execute | Auto for that work |
| Time-sensitive turnaround | Fast, successor to Performance |
| Exceptional unresolved blocker | Consider Ultimate narrowly, after diagnosis |

Choose according to observed progress. Efficient's free offer has eligibility
conditions and may be slow/rate-limited. Check your actual selector on the day;
sub-agent/specific-model calls can be billed separately, so keep sub-agents off.
Do not let a cheap model burn time in repeated failures. Avoid scattering work
across many chats or switching models after every small edit.

| Spending envelope, not an automatic cap | Credits |
| --- | ---: |
| Quick local C1 allowance; unused credits stay with implementation | 50 |
| Required implementation | 1,950 |
| Focused corrections | 400 |
| Protected reserve for late gaps/blockers | 600 |
| Total | 3,000 |

These allocations are suggestions, not price predictions or enforced limits.
A 100-word reply can still involve substantial billed input/internal activity.
Limit C1's scope and reads, not just its output. Check actual usage;
stop at a safe milestone and reassess if the burn rate is too high. At 1,200
remaining, review gaps and stop optional polish. Protect the last 600 for required
gaps and delivery. Never drop explicit rubric items merely to save tokens.

## Nine-hour targets

| Elapsed time | Target |
| --- | --- |
| 00:00-00:30 | Read originals; Google coverage and proposed plan |
| 00:30-01:00 | One Qoder preflight, essential corrections, runnable baseline |
| 01:00-06:00 | Continuous implementation; human checks and working checkpoints |
| 06:00-07:30 | One final audit, Google gap review and scoped fixes |
| 07:30-08:15 | Required final checks, user flows, README and fresh-copy rehearsal |
| 08:15-09:00 | Submit, verify Gitea commit/access and actual submission; buffer |

Use the actual start, deadline, stack and submission rules from tomorrow's brief.
The older practice sheet's 17:00 cutoff is not assumed. Git push alone may not
complete the required submission action.

Credit accounting and Efficient offer rechecked 1 November 2026:
[credit accounting](https://docs.qoder.com/Credits),
[Efficient eligibility/limits](https://docs.qoder.com/events/efficientunlimited).
Other references checked 31 October:
[model controls](https://docs.qoder.com/user-guide/chat/model-tier-selector),
[Performance became Fast](https://docs.qoder.com/product-overview/fast-mode-announcement),
[Caveman limitations](https://raw.githubusercontent.com/JuliusBrussee/caveman/main/docs/HONEST-NUMBERS.md).
