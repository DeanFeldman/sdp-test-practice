# Qoder: implement efficiently and verify full rubric coverage

The original brief and rubric PDF take precedence over the generated plan.
Target every full-mark requirement; do not claim a guaranteed score.

- Read the original brief and every rubric page once at the start, including
  tables/descriptors. Flag unreadable or missing source. Reuse this understanding
  in the same conversation; revisit relevant criteria rather than repeatedly
  extracting the entire PDF.
- Execute the supplied plan continuously. Group related changes. Do not ask for
  permission after every task, redesign the approach, add optional features or
  repeat planning. Resolve routine local details using existing project patterns.
- Read relevant files/callers/contracts only. Search before broad file reads.
  Preserve working behavior, validation and tests. Avoid unnecessary dependencies
  and refactoring. Keep tool output focused without losing diagnostic evidence.
- I run routine setup/install, scaffold commands, servers, builds, lint/typechecks,
  tests, browser checks and Git writes unless I explicitly delegate a command.
  You may inspect/search code and read diffs. Write required code/tests/docs.
- Batch human commands at meaningful milestones: ID, working directory, exact
  command and expected success. Derive commands from actual scripts/lockfiles;
  do not guess. Reuse known command IDs instead of reprinting unchanged commands.
  Mark results pending until I report them. No repeated polling.
- Continue independent work while my commands run. Do not edit files/configs
  being checked or rely on pending results. If relevant files change, mark the
  result outdated and request only affected checks again. Pause when progress
  depends on my result rather than looping or inventing success.
- Use my actual failures to fix straightforward errors, then ask me to rerun
  affected checks. Reuse valid results; do not repeat passing checks unnecessarily.
- Stop for missing essential facts, a required design change or two unsuccessful
  repairs of the same failure. Give the exact blocker and attempts made.
- No sub-agents, repo wiki, external AI calls or narrated edits. Use terse,
  technically precise prose. Preserve requirements, identifiers and negations.
  Give brief milestone updates without awaiting a reply.
- Before finishing, check every original rubric criterion once. Fix scoped gaps
  within the agreed design and request outstanding human checks. Report one compact
  complete table IN CHAT ONLY: criterion ID/page | implementation evidence |
  actual check/result | remaining gap. Attribute my results as human-run; mark
  pending, outdated, blocked or unverified items explicitly;
  never invent results or award yourself marks. Do not repeat the table elsewhere.
- Do not create or maintain audit reports, status files, planning documents or
  duplicate summaries. Produce any documentation/tests/deliverables explicitly
  required by the assessment, plus what is necessary to run and verify the work.
  If later fixes affect a few criteria, report changed rows only; do not regenerate
  the whole audit unless explicitly requested or a broad change invalidates it.
