# Hackathon: your steps

## Latest rules for Monday, 2 November

- Arrive by **07:45**. Session: **08:00-17:00**.
- **08:00-08:30: planning only; no coding.** Then 7.5 hours programming and a
  one-hour lunch at the instructed time. Lunch is not extra coding time.
- **Qoder is the only assured AI.** Gemini/Google Search AI may work; Antigravity
  is not allowed. Do not make the workflow depend on Google being reachable.
- Check the exam's domain allowlist and actual tools. Be ready to adapt the stack.
  Phones/earphones are permitted; breaks must stay within the stated courtyard bounds.

## Your exam sequence

1. **Planning period:** take two quiet minutes, read the complete brief/rubric and
   allowlist, then choose the route below. No code, scaffolding or implementation.
2. **If Google works:** use **A** with the original PDFs, actual project facts,
   preferred stack, domain list and Gitea details. Save its complete Markdown output
   as **`EXECUTION-PLAN.md`**. No 2.5-hour rehearsal override.
3. **If Google fails:** use **A0 in Qoder**, with the rules and same originals/facts.
   It returns one compact plan including the local blocker check. Save the plan
   yourself; **skip separate C1**. Do not spend the planning period fixing Google.
4. **From 08:30, when coding is permitted:** on the Google route give Qoder the
   rules, originals and plan, then **C1**. READY/READY WITH CORRECTIONS -> **C2 in
   the same chat**. On the A0 route, paste **C2 in that same Qoder chat**, without
   repeating the plan/rubric extraction. For a major blocker use B only if Google
   is available; otherwise ask Qoder for one focused recommendation/diagnostic.
5. **Set up Git and make the initial push early in the coding period.** You run
   installs, servers, checks and Git commands when Qoder cues them; report compact
   results. Roughly hourly, use the app end to end, commit and push.
6. **Monitor credits:** protect 600 for late required fixes. After two failed repairs
   of one problem, stop that loop and use a focused diagnostic with Qoder or Google
   if available. Model rates/eligibility must be checked in the actual selector.
7. **Final coverage:** around 5.5 active hours (excluding lunch), Qoder reconciles
   the originals and returns one rubric evidence table **in chat only**. E is only
   a fallback if this is missing; update changed rows after fixes. Google F is optional.
8. **Final 45 minutes:** required checks, README/run instructions, fixes and delivery.
   Verify the actual submission, Gitea commit and marker access before **17:00**.

## Model to use for each prompt

Select the model yourself before sending; prompts cannot switch it. Check your
actual displayed rate and balance. These are starting choices, not quality or
credit guarantees. Use Efficient at 0.0x only if your account actually offers it.

| Prompt / work | Where | Starting model |
| --- | --- | --- |
| A: original plan | Google, if available | Available permitted Google AI; no Qoder credits |
| A0: Qoder-only planning fallback | Qoder | **Auto once**, then switch to Efficient for C2; skip C1 |
| B: material plan correction | Google, if available | Google; if unavailable, **Auto** for one focused Qoder correction |
| C1: quick local blocker check | Qoder | **Efficient** |
| C2: continuous implementation | Qoder | **Efficient** for clear tasks; **Auto** for difficult core logic |
| D: persistent blocker diagnosis | Google if available, otherwise Qoder | Google; **Auto** for a focused Qoder diagnosis/complex repair |
| E: final evidence table, only if missing | Qoder | **Efficient**; Auto only for a specific complex unresolved gap |
| F: optional final gap review | Google, if available | Google; skip if unavailable, since Qoder already checks coverage |
| Frontend handoff / targeted UI fixes | Existing Qoder C2 chat | **Efficient** |

Use the same chat when switching. Escalate for repeated wrong behavior, unmet
requirements or a difficult logic problem; do not rerun the whole plan/audit.
After two failed repairs of one issue, stop that loop and diagnose. A thinking
pause alone is not evidence the model is failing. No automatic Ultimate, Fast,
specific-model or multi-agent escalation; Fast is an optional turnaround choice
only if the actual rate and remaining time make sense. Keep Experts/sub-agents off.

## What to bring and give each tool

The **submitted application's README** must include the required **AI attribution /
declaration** from the Moodle document/template or instructions supplied in chat.
Bring that source with the brief and give it to the planner and Qoder. Preserve
its required wording/fields and actual tool usage; missing requirements must be
flagged, not invented. Qoder's final checks must cover this required deliverable.
The supplied [AI policy](ai_policy.pdf) also requires attribution in AI-generated
code commits and declarations in written documents. See
[AI-ATTRIBUTION-GUIDE.md](AI-ATTRIBUTION-GUIDE.md) for exact templates, fresh-session
and transcript guidance. Record actual models; Auto/Efficient tier names may not
identify the underlying model, so disclose unavailable details and seek clarification.

Bring these permitted Markdown materials through Moodle as instructed:

- [EXAM-WORKFLOW.md](EXAM-WORKFLOW.md): the readable step-by-step workflow from chat.
- [HACKATHON-PLAYBOOK.md](HACKATHON-PLAYBOOK.md): A/A0, C1/C2 and fallback prompts.
- [QODER-HACKATHON-RULES.md](QODER-HACKATHON-RULES.md): shared Qoder instructions.
- This README: your steps.
- [EXAM-PREP.md](EXAM-PREP.md): optional human editor/plugin checklist.
- [FRONTEND-GUIDE.md](FRONTEND-GUIDE.md): optional human resource/handoff guide.
- [AI-ATTRIBUTION-GUIDE.md](AI-ATTRIBUTION-GUIDE.md) and [ai_policy.pdf](ai_policy.pdf): attribution requirements and templates.

Give Qoder only the rules, execution plan if already created, original brief/rubric
and relevant project facts/examples. Do not ask it to read the whole playbook,
human prep sheets, old plans or Google history. Keep the same chat and reuse context.
The exam plan is created tomorrow, not copied from the Test 1 rehearsal.

## Tonight and frontend direction

**Preferred stack, unless the brief/starter or actual environment requires otherwise:**

| Part | Default |
| --- | --- |
| Frontend | React + TypeScript + Vite |
| Styling | Plain CSS with shared colour/spacing/type tokens; system fonts |
| Backend, when needed | Python + FastAPI |
| Database, when persistence is needed | SQLite, using Python's sqlite3 initially |
| UI extras | Only needed, reachable packages; no mandatory component kit/CDN |

This follows the main technologies used in your Test 1 solution, without requiring
its exact architecture or every dependency. A/B/A0 should use this default rather
than ask you to choose frameworks. Preserve a suitable provided starter. Do not
add a backend/database if the actual task does not need one, or add Docker, Redis,
authentication, an ORM or deployment services merely because they are available.

Check actual Node/Python compatibility and allowed package access before setup;
do not assume latest versions work on the exam machine. If React tooling is
unavailable, use plain HTML/CSS/JavaScript with FastAPI where suitable. If a required
part of the stack is blocked, the planner chooses one minimal permitted alternative
and explains why, rather than repeatedly attempting blocked installations.

Note editor extensions/settings you already use rather than depending on new
installations. Check compatibility tonight.

Your chosen visual style is **editorial: charcoal, cream and burnt orange**, with
strong headings, whitespace, subtle dividers and aligned data. A/A0 carry that
preference. Build a connected UI flow early, complete UI alongside features, then
polish once. Follow any required branding/accessibility rules.

Design sites are inspiration to browse tonight, not confirmed exam domains.
Save permitted references through Moodle. Prefer **system fonts and local assets**;
no required runtime CDNs. Keep the style with plain CSS if a component kit is
unavailable. No extra AI generators, agent plugins or AI integrations.

Get sleep and arrive early. Follow authoritative exam updates. Target every rubric
criterion with real evidence; no prompt guarantees a score, time or credit usage.
`this_is_a_test.md` is an old guide and is not tomorrow's instructions.
