# Tonight: environment and frontend preparation

This is your human checklist, not another document for Qoder to read. The lecturer
asked you to note plugins/environment preferences and prepare permitted materials
through Moodle. Tomorrow's instructions decide what can be installed or imported.
Use the actual brief for marks and required behavior; the announcement highlights
visual design and usability without making the exam frontend-only.

## What to write down

Latest rules: arrive by **07:45**. Session **08:00-17:00**, with **08:00-08:30
planning only (no coding)**, **7.5 programming hours** and **one hour lunch** at the
instructed time. Qoder is assured; Gemini/Google Search AI are only possible.
Prepare for the Qoder-only A0 route. Python, JavaScript, Java and well-known
frameworks, Docker and popular databases are described as available; verify the
actual stack/domains in the brief. Phones/earphones are permitted. Short breaks
must stay within the MSL courtyard boundaries stated by the lecturer.

Record names/settings you already use so you can recreate them quickly on the exam
machine. A written list is enough; installing everything listed is not a goal.

| Item | Your choice to record tonight |
| --- | --- |
| Editor | Actual Qoder/editor version and where you open the terminal |
| Appearance | Familiar theme; comfortable editor/terminal font size and zoom |
| Layout | Editor beside browser; visible terminal and Problems panel |
| Editing | Word wrap preference, indentation and one formatter per language |
| Formatting | Format on save only if tested with the chosen formatter/project |
| Terminal | Actual shell (PowerShell/bash/etc.); do not assume another machine matches |
| Runtime | Provisional language/framework/database; verify actual available versions tomorrow |
| Git | Required Gitea URL/branch when supplied, user identity, permitted authentication method |
| Qoder | Actual credit balance/model rates; no extra AI assistants or agent bundles |

Use project formatting settings if supplied. Keep credentials and tokens out of
Markdown, screenshots and Moodle uploads. No package upgrades or global environment
changes just to recreate a cosmetic preference.

## Small tool shortlist

Choose only tools you can test tonight. Availability in Qoder must be checked;
VS Code support does not establish Qoder compatibility.

| Tool | Why consider it | When to skip it |
| --- | --- | --- |
| Prettier - Code formatter | Consistent JS/TS/HTML/CSS formatting with less manual tidying | Existing formatter suffices, unsupported editor, or configuration work adds friction |
| Tailwind CSS IntelliSense | Class suggestions and Tailwind language support | You are not using Tailwind or it is unavailable in your editor |
| Existing language support | Diagnostics/navigation for your chosen stack | It is already built in; avoid duplicate language servers |
| Browser DevTools | Inspect CSS; check Console/Network; resize with Device Mode | No separate extension is needed for ordinary browser checks |
| Built-in Git UI / ordinary Git | Stage changes, inspect diffs and push checkpoints | Extra Git dashboards add little if ordinary Git is familiar |

Editor extensions, application libraries and AI plugins are different things.
Qoder's plugin marketplace can bundle agents, skills, MCP integrations and hooks;
it is not automatically a harmless editor convenience. For this credit-limited
workflow, keep extra AI assistants, agent bundles and background automations off.
Do not assume an editor profile/import from another product works in Qoder.
If using VS Code, a tested exported profile can carry selected preferences; use
only import methods available and permitted on the exam machine.

## Choose a frontend direction once

Spend roughly 10-15 minutes choosing a direction, then stop browsing. These are
options, not three designs to build:

| Direction | Palette | Layout/feel |
| --- | --- | --- |
| Clean dashboard | Navy, teal, off-white | Clear navigation, aligned data, restrained borders |
| Editorial | Charcoal, cream, orange | Strong headings, generous whitespace, structured sections |
| Architectural | Forest green, stone, white | Orderly grid, solid surfaces, precise spacing |

Your selected default: **Editorial - charcoal, cream and orange**. Use cream
background `#F7F3EA`, charcoal text `#242424`, burnt-orange accent `#B84018`, and
subtle dividers. Treat these as starting tokens, checking contrast for actual use.
Use strong headings, clear navigation, generous whitespace and aligned tables.
Keep data views practical; avoid turning every item into a decorative card.

Note one or two reference sites and the specific thing
you like (navigation, table layout, spacing), rather than asking Qoder to clone a
whole website. Use system fonts unless a required/custom font is already available.
Make accent colours readable; use text/icons as well as colour for status.

Paste only your short choice into Google A's VISUAL DIRECTION input:

```text
Visual direction: editorial; charcoal text, cream backgrounds and burnt-orange
accents. Strong headings, generous whitespace, subtle dividers and aligned data.
Use consistent spacing/type, readable contrast, clear navigation and an obvious
primary action. Match the layout to the required workflow and data. Include
loading, empty, validation, success and error states; preserve visible keyboard
focus and labels. Adapt cleanly to narrower windows. Keep one coherent style;
avoid unrelated decoration, fake data and optional redesigns.
```

This is a default preference; the brief and required branding/accessibility rules
take precedence. A component library is optional: use an existing familiar one if
it saves implementation work, without adding one just for appearance.

## Roughly hourly: you use the app

Walk through the main user task from start to finish. Check the screen at a
narrower width, read the labels, try an empty/invalid input where relevant and
confirm loading/errors are understandable. Check keyboard focus for main controls.
Look at browser Console/Network when something fails. Report concrete issues in
one batch: action, expected result, actual result and screenshot/error if useful.
Do not ask Qoder for a separate broad visual audit after each small edit.

Commit a working checkpoint and push roughly hourly. The last 45 minutes are for
required checks, delivery and blockers, not a new visual concept.

## Bring in, then rest

Prepare the README, playbook and Qoder rules through Moodle as instructed; bring
this preference list if useful. No runtime settings were changed or extensions
installed by creating these notes. Check the next announcement, take two quiet
minutes at the start tomorrow, sleep and arrive early.

## Sources checked 1 November 2026

- [VS Code settings](https://code.visualstudio.com/docs/configure/settings) and
  [profiles](https://code.visualstudio.com/docs/configure/profiles).
- [Prettier editor integration](https://prettier.io/docs/editors).
- [Tailwind editor support](https://tailwindcss.com/docs/editor-setup).
- [Qoder plugin components](https://docs.qoder.com/extensions/plugins).
- [Chrome Device Mode](https://developer.chrome.com/docs/devtools/device-mode)
  approximates mobile layouts; it does not prove behavior on a physical device.
