# Frontend resources and Qoder handoff

For the human preparing the exam. Follow the actual brief and permitted-resource
rules. Your default is **editorial: charcoal, cream and burnt orange**. This guide
does not establish any resource as permitted by the exam and is not another whole
document to feed to Qoder. Give it only your chosen brief and relevant examples.

## Start the UI early; finish the polish later

Do not leave the entire frontend until the end. Do not spend the beginning making
a beautiful disconnected mockup either. Build in this order inside the existing
execution plan, rather than creating a separate UI project:

1. Before coding, choose a style and at most one suitable component approach.
2. Early milestone: basic page shell, navigation, type/colour/spacing tokens and
   one real end-to-end user flow connected to the backend or required data source.
3. As each feature lands, add its working controls, real results, loading, empty,
   validation and error states. Keep required tables/charts readable.
4. Roughly hourly, you use the app and send Qoder one batch of concrete issues.
   Check a narrower window and keyboard focus on main controls. Commit and push.
5. After required flows work, do one focused consistency pass: alignment, spacing,
   responsive layout, contrast, labels and selected/disabled/focus states.
6. Protect the final 45 minutes for required verification, blockers and submission.
   No new UI library, visual concept or animation framework at that point.

For a data-heavy task, prioritize readable tables, filters, useful charts and
clear feedback over landing-page effects. For a different brief, use its actual
main workflow. A styled shell is not evidence that the required application works.

## Small resource shortlist

Firewall update: these sites are candidates to browse tonight, not confirmed exam
allowlist entries. Save permitted references through Moodle. Tomorrow use supplied
domains and installed/reachable packages. Default to system fonts and local assets;
the app must not depend on a font/icon/CSS CDN or external preview loading. If a
component kit is unavailable, keep the chosen visual style using plain CSS and
existing components instead of spending time on network workarounds.

| Resource | Use it for | Integration decision |
| --- | --- | --- |
| [shadcn/ui blocks](https://ui.shadcn.com/blocks) | React UI components and reference layouts | Consider when using a compatible React stack and setup is familiar; bring only needed components, not a whole dashboard with demo dependencies/data |
| [daisyUI components](https://daisyui.com/components/) | Tailwind component classes for forms, buttons, alerts and navigation | Alternative if using Tailwind; select one UI approach rather than combining it with shadcn |
| [Lucide](https://lucide.dev/guide/) | Consistent navigation/action/status icons | Use its package for the chosen framework; import only needed icons and keep labels on important actions |
| [Google Fonts: DM Serif Display](https://fonts.google.com/specimen/DM+Serif+Display) | Optional editorial heading typeface | Pair with system sans-serif body/control text; use system fonts throughout if this saves setup or external access is uncertain |
| [Awwwards](https://www.awwwards.com/websites/) | Layout, typography and colour inspiration | Pick one relevant reference; note what you like rather than copying its entire site |

Plain CSS is sufficient when it is the simplest fit. These resources are optional,
not a shopping list of dependencies. Keep the starter's working UI stack where
suitable. Do not force a stack migration for a component library.

Use the ordinary documentation, previews and permitted source examples. Skip
embedded AI generators, "open in v0" buttons, MCP installers, agent plugins and
AI theme generators: the agreed exam tools are Qoder and Google Search AI only.
Preserve applicable licenses/notices when reusing code or assets. A public preview
is not automatically permission to reuse its code, photos or branding.

## Your default design brief

- Background: cream `#F7F3EA`; primary text: charcoal `#242424`.
- Accent: burnt orange `#B84018`, used consistently for primary actions/highlights.
- Large editorial headings; practical sans-serif controls, body and tables.
- Generous spacing, aligned columns, subtle borders and a clear page hierarchy.
- Visible focus, labelled inputs, readable contrast and useful feedback states.
- Use actual application data; no dummy dashboard sections just for decoration.

Colours are starting tokens, not a claim that every possible combination passes
contrast checks. Adjust for readability and any branding/accessibility requirements.
Avoid adding a font dependency solely to achieve this direction: a system serif
heading and system sans-serif body can express it too.

## How to integrate without wasting Qoder credits

**Tonight, you:** spend 10-15 minutes choosing one reference and familiar resources.
Record one URL and 2-3 specific details (for example heading treatment, sidebar
structure and table spacing). Save a permitted screenshot/snippet if useful.
Do not download an entire template collection or install several competing kits.

**Google A:** fill in its stack/visual inputs with your choice. Add this:

```text
UI reference: <one URL or supplied screenshot; details I like>.
Chosen resources: <compatible UI approach and icons, or plain CSS/system fonts>.
Use the editorial charcoal/cream/orange direction. Establish the style and one
real connected user flow early, then complete UI behavior alongside each feature.
Include a focused final consistency pass before the submission buffer.
Resources are optional; preserve the starter and avoid unnecessary dependencies.
Do not add demo sections, fake data or integrations merely for appearance.
```

**Qoder C1/C2:** keep the existing sequence and same chat. Do not add a separate
paid design-planning turn. The execution plan should carry the short visual brief.
If it does not, append this to C2:

```text
UI: editorial charcoal/cream/burnt orange; strong headings, clear navigation,
aligned data and generous spacing. Use <chosen compatible resources or plain CSS>.
Reference detail: <specific detail; attach only the relevant screenshot/snippet>.
Build a connected flow early and UI states alongside features; finish with one
focused consistency pass. Reuse working components/tokens; no optional redesign.
I run setup and browser checks; cue the needed commands. Preserve rubric behavior.
```

Do not paste a whole component website, screenshot gallery or template repository
into chat. A link alone does not guarantee Qoder can read it: supply the relevant
example if needed, or let it implement from your short description. If adopting
a component, account for its dependencies/imports; a pasted fragment may not run
alone. Qoder cues the actual setup command for your project, and you run it.

## How to ask for a late visual fix

Batch concrete observations in the same Qoder chat:

```text
UI fixes only; preserve working behavior and architecture:
1. <screen/action>: <actual issue> -> <required result>.
2. <screen/action>: <actual issue> -> <required result>.
Change only affected components/styles. Reuse current tokens and dependencies.
Request affected checks only; update changed audit rows if relevant. No redesign,
new UI library or duplicate report. Human browser checks: <actual results>.
```

Prefer "the table overflows at this width" or "the error is hidden below the form"
to "make it cooler", which can trigger broad redesigns and extra credit use.

Resources checked 1 November 2026. The application brief still determines what
must be built, what may be reused and how it is assessed.
