# Eight-hour hackathon: Google plans, Qoder checks once and implements

For Monday, 2 November 2026: one person, 3,000 Qoder credits. Prepared materials
must follow the exam's rules; Google access is optional, not assured.
Latest lecturer rules: arrive by 07:45 on Monday 2 November. Session 08:00-17:00:
30 minutes planning (08:00-08:30, no coding), 7.5 hours programming and one hour
lunch. Lunch placement follows the invigilator's instructions; it is not coding
time. Qoder is the only assured AI. Gemini/Google Search AI may fail behind the
firewall; Antigravity is not allowed. Check the supplied domain list and adapt.

The rehearsal exposed errors in Google's proposed technical details. Use Google
for complete rubric coverage, priorities and a proposed architecture. Give Qoder
one bounded technical preflight, then use its effort for implementation. You run
routine commands, provide real results and submit. This workflow aims to reduce
avoidable work; actual time/credit savings and the eventual score are not guaranteed.

## Inputs and Gitea

Before the exam, use [EXAM-PREP.md](EXAM-PREP.md) to record editor/terminal
preferences and select a visual direction. Do not feed that human checklist to
Qoder. Supply just the chosen stack/style below; avoid spending coding time on
new plugins or a new design system.

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

Prepared default: React + TypeScript + Vite, plain CSS/system fonts; Python +
FastAPI when a backend is needed; SQLite via sqlite3 when persistence is needed.
Preserve a suitable starter. No mandatory component kit, ORM, Docker or extra
services. If React tooling is blocked, prefer plain HTML/CSS/JavaScript where
suitable; required stack changes must follow the actual brief and available tools.

## A. Google: plan once

Use A only if Google Search AI or Gemini actually works and is permitted. If it
fails, switch promptly to A0 below; do not burn planning time troubleshooting it.

```text
I am alone with 3,000 Qoder credits. The session is 08:00-17:00: 30 minutes
planning with NO CODING, 7.5 hours programming and one hour lunch at the instructed
time. Plan within those limits; lunch is not coding time. This turn is planning
only: no application code, executable scaffolding or implementation. You are the overall
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
   Follow supplied starter/stack constraints; otherwise use my provisional familiar
   stack where suitable, making remaining choices yourself. Preserve my visual
   direction and define a coherent layout, typography and colour system; avoid
   generic decorative effects unrelated to that direction.
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
AI ATTRIBUTION REQUIREMENTS: supplied ai_policy.pdf (attach it), plus any later
Moodle/exam clarifications. Include its required attribution/declaration in the submitted
application's README, using required wording/fields and only genuine AI usage.
Include code-commit Assisted-by trailers and written-document declarations in
deliverable checks. Flag unresolved source/usage details; do not fabricate compliance.
PROJECT FACTS: <mandated stack, starter/no starter/unknown, tree, scripts, code>
AVAILABLE DOMAINS / ENVIRONMENT: <supplied allowlist and actual installed tools>
GITEA EXAM URL / BRANCH: <actual values or unknown>
PREFERRED STACK: React + TypeScript + Vite; plain CSS and system fonts. Python +
FastAPI backend if needed; SQLite via Python sqlite3 if persistence is needed.
Preserve a suitable supplied starter. Avoid unnecessary ORM/services/component
kits. Check actual runtime/package availability. If React tooling is unavailable,
prefer plain HTML/CSS/JavaScript where suitable; otherwise choose one minimal
permitted alternative. No repeated blocked installs or mandatory external CDNs.
VISUAL DIRECTION: Editorial: charcoal text, cream backgrounds, burnt-orange accents.
Strong headings, generous whitespace, subtle dividers and aligned data. Use clear
navigation, labelled controls and visible keyboard focus. Include loading/empty/
error/success states and adapt to narrower windows. Follow required branding and
accessibility rules; keep this coherent style without optional redesigns.
Do not require external fonts, images, CDNs or design sites to load at runtime.
Use available local assets/system fonts and only compatible, reachable packages.
```

Check coverage yourself. Copy the entire Markdown block (including the rubric
checklist) into a new text file in the **exam project's root folder**, named
exactly `EXECUTION-PLAN.md`. Save as UTF-8 plain text, without the surrounding
code fences; check it is not named `EXECUTION-PLAN.md.txt`. Google supplies the
contents; you save it. No Qoder request or Google Docs/PDF conversion is needed.
For the old Test 1 rehearsal, explicitly override the exam timetable with its
stated 2.5 hours; tomorrow's actual brief remains authoritative.

## A0. Qoder-only planning fallback (08:00-08:30; no coding)

**Model: Auto for this one planning turn.** Select it manually; switch to Efficient
before C2 for well-specified work. No extra planning turn just to change models.

Give Qoder the originals, short rules, actual starter facts, available domains
and your stack preference. Use one concise planning request. This replaces Google
A and separate C1: do not pay for another planning/preflight turn afterward.
Use the same chat for C2 from 08:30, reusing this context. Save the plan yourself
as `EXECUTION-PLAN.md`; do not ask Qoder to write a second process document.

```text
Apply QODER-HACKATHON-RULES.md. A0: planning only; NO CODING or file changes.
Session 08:00-17:00: planning until 08:30, 7.5 hours programming, one hour lunch
at the instructed time. Read the complete original brief/rubric once, including
tables; flag unreadable source. Inspect only essential supplied starter facts.
Return one compact Markdown plan for EXECUTION-PLAN.md: all criterion IDs/pages,
exact full-mark requirements/weights; one feasible architecture using my familiar
stack where suitable (React/TypeScript/Vite + plain CSS; FastAPI and SQLite only
when needed); critical formulas/boundaries/contracts; ordered milestones
and observable checks; final 45-minute delivery buffer. No application code,
speculative commands, alternative surveys or separate audit. Preserve every
required criterion, Gitea delivery and editorial charcoal/cream/orange styling.
Use the supplied domain allowlist/actual environment; avoid CDN/runtime asset
dependencies. This includes the quick local blocker check; do not repeat C1.
Ask only for essential missing facts. Wait for my C2 after coding is permitted.
INPUTS: <originals, starter facts, preferred stack, allowlist, Gitea URL/branch>
AI ATTRIBUTION: follow the supplied Moodle document/template or instructions in
chat for the submitted application's README. Include it as a deliverable/check;
request missing source/details instead of inventing wording or usage.
```

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
If Google stops working, keep the Qoder chat and request one focused correction
or missing diagnostic from its findings. Do not restart with A0 or another full plan.

## C2. Qoder: implement continuously

Use the **same Qoder chat**. Try Efficient if its actual rate is 0.0x for
well-specified work; use Auto for difficult core logic or repeated failures.
You select the model. The prompt cannot switch tiers or enforce a credit cap.

```text
C2: coding is now permitted. Continue under the rules already loaded.
Implement EXECUTION-PLAN.md with
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
If Google is unavailable, use the same focused diagnostic request with Qoder in
the existing chat; do not call external AI. Request one missing diagnostic or
one evidence-based fix; pause dependent work if an essential blocker remains.

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

**Model: Efficient.** Use Auto only for a concrete complex gap, not to repeat an
already complete table or re-audit solely because you changed models.

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

| Prompt / work | Starting choice |
| --- | --- |
| A: original plan | Available permitted Google AI, if working; no Qoder tier |
| A0: Qoder-only planning | Auto once; then Efficient for clear C2 work; skip C1 |
| B: plan correction | Google; if unavailable, Auto for one focused Qoder correction |
| C1: quick local blocker check | Efficient if available at the displayed rate |
| C2: implementation | Efficient for clear work; Auto for difficult core logic |
| D: blocker diagnosis | Google if working; otherwise Auto for focused Qoder diagnosis/complex repair |
| E: final audit only if missing | Efficient; Auto for a specific complex gap only |
| F: optional final review | Google if working; otherwise skip duplicate review |
| Frontend guide's C2 add-on / UI fix prompt | Efficient in the existing chat |

You select tiers manually; prompts cannot switch them. See the same table in the
README while working. A model change is not a reason to restart the chat, re-plan
or repeat checks. Stop after two unsuccessful repairs of the same failure; diagnose
with evidence rather than buying another blind attempt. A thinking pause alone
does not show failure. Fast may help turnaround when its actual rate/time tradeoff
makes sense, but is not a default step. Ultimate and specific models are not needed
by default; keep Experts/multi-agent mode off to avoid extra context and calls.

Choose according to observed progress. Efficient's free offer has eligibility
conditions and may be slow/rate-limited. Check your actual selector on the day;
sub-agent/specific-model calls can be billed separately, so keep sub-agents off.
Do not let a cheap model burn time in repeated failures. Avoid scattering work
across many chats or switching models after every small edit.

| Spending envelope, not an automatic cap | Credits |
| --- | ---: |
| Planning/preflight allowance; use for A0 if Google unavailable | 200 |
| Required implementation | 1,800 |
| Focused corrections | 400 |
| Protected reserve for late gaps/blockers | 600 |
| Total | 3,000 |

These allocations are suggestions, not price predictions or enforced limits.
A 100-word reply can still involve substantial billed input/internal activity.
Limit C1's scope and reads, not just its output. Check actual usage;
stop at a safe milestone and reassess if the burn rate is too high. At 1,200
remaining, review gaps and stop optional polish. Protect the last 600 for required
gaps and delivery. Never drop explicit rubric items merely to save tokens.

## Exam timetable and active-work targets

| Elapsed time | Target |
| --- | --- |
| Before 08:00 | Arrive by 07:45 and follow setup instructions |
| 00:00-00:30 (08:00-08:30) | Two quiet minutes; read originals/allowlist; Google A or Qoder A0; no coding |
| 00:30-00:45 (from 08:30) | C1 only for Google route; C2; human Git setup/initial push; start baseline |
| 00:45-05:30 | Continuous implementation; roughly hourly human workflow checks, commits and pushes |
| 05:30-06:30 | One final rubric reconciliation and scoped fixes; Google review only if available/useful |
| 06:30-07:15 | Required final checks, user flows, README and fresh-copy rehearsal |
| 07:15-08:00 | Submit, verify Gitea commit/access and actual submission; buffer |

Elapsed targets count eight active hours: 30 minutes planning plus 7.5 programming.
Pause this active-work clock for the instructed one-hour lunch. Do not invent a
lunch slot or code during planning. Deadline is 17:00 per the latest announcement;
follow any authoritative clarification. Git push alone may not complete submission.

Credit accounting and Efficient offer rechecked 1 November 2026:
[credit accounting](https://docs.qoder.com/Credits),
[Efficient eligibility/limits](https://docs.qoder.com/events/efficientunlimited).
Other references checked 31 October:
[model controls](https://docs.qoder.com/user-guide/chat/model-tier-selector),
[Performance became Fast](https://docs.qoder.com/product-overview/fast-mode-announcement),
[Caveman limitations](https://raw.githubusercontent.com/JuliusBrussee/caveman/main/docs/HONEST-NUMBERS.md).
