# SDP Test Cheat Sheet — COMS3011A

Student: Dean Feldman  
Student Number: 2803899

## Test Basics

- Time: **14:30–17:00**
- Use the **lab computers**
- Qoder is allowed
- Other AI tools are not allowed
- Submission must be **one clonable Git repository**
- The marker must be able to run:

```bash
git clone <repo-url>
```

with **no SSH key and no HTTP PAT**
- The repo must contain a **README** with exact run instructions
- The last commit **before 17:00** is what gets marked
- Make sure everything is **committed and pushed**

---

# 1. Start-of-Test Workflow

## Read before coding

1. Read the entire brief.
2. Read the entire rubric.
3. Identify:
   - high-mark requirements
   - required core functionality
   - dependencies
   - quick marks
   - submission requirements
4. Read the rubric yourself once before giving it to Qoder.

---

# 2. First Qoder Prompt

Give Qoder the **entire brief + rubric**.

```text
Read the entire attached assessment brief and rubric carefully.

Your objective is to complete this assessment to the highest possible standard
and maximise the rubric score.

Before making changes:
1. Inspect the entire existing repository.
2. Identify every requirement in the brief.
3. Extract every rubric criterion and its marks.
4. Identify dependencies between requirements.
5. Identify anything that could prevent the application from running or being marked.
6. Create a concise implementation plan prioritised by:
   - required/core functionality
   - highest-mark rubric items
   - dependencies
   - quick marks
   - cosmetic improvements last

Then implement the complete solution.

Important:
- Follow the existing architecture and coding style.
- Prefer the simplest working solution.
- Do not unnecessarily refactor working code.
- Do not add unnecessary dependencies.
- Do not remove existing functionality unless required.
- Implement ALL rubric requirements.
- Test functionality as you implement it.
- Fix build, type, runtime and integration errors.
- Do not leave TODOs, placeholders, fake implementations or incomplete features.
- Keep track of the rubric throughout implementation.

Submission requirements:
- Everything must be contained in one Git repository.
- The repository must be clonable without requiring an SSH key or HTTP PAT.
- Include a README with exact instructions for running the submission.
- Do not put secrets, PATs or credentials in the repository.

After implementation:
1. Run the relevant build.
2. Run available tests.
3. Test the important user flows.
4. Review the solution against EVERY rubric criterion.
5. Fix anything incomplete, partial or broken.
6. Check obvious edge cases.
7. Check the README/run instructions.
8. Give me a final rubric table showing:
   - criterion
   - status
   - evidence/file implementing it
   - expected marks
9. Clearly tell me if ANYTHING remains that could prevent 100%.

Do not stop after only generating a plan. Carry out the implementation as well.
```

---

# 3. If Qoder Starts Going Wrong

## Stop unnecessary refactoring

```text
Stop.

Do not make any more unrelated changes.

The current issue is:

<PASTE ERROR OR PROBLEM>

Find the root cause and fix only this issue.
Do not refactor unrelated code.
```

## If it changes too many files

```text
Stop making changes.

Explain why this requirement required changes to so many files.
Identify which changes are actually necessary.
Keep the smallest working solution.
```

## If one requirement is still broken

```text
Implement rubric requirement X only.

Use the existing architecture.
Make the smallest working change.
Do not refactor unrelated code.

Afterwards:
1. list the files changed
2. explain what changed
3. tell me exactly how to test it
4. tell me which rubric criterion it satisfies
```

---

# 4. Git Commands You Need

## Check where you are

```bash
pwd
ls
```

## Check repository state

```bash
git status
```

## See changes

```bash
git diff
```

## See recent commits

```bash
git log --oneline -5
```

## Save work

```bash
git add .
git commit -m "Implement feature"
git push
```

## Check remote

```bash
git remote -v
```

## Undo one bad uncommitted file change

```bash
git restore path/to/file
```

Be careful: this discards uncommitted changes in that file.

---

# 5. PAT Reminder

If Git asks for credentials while pushing:

```text
Username: Dean
Password: <YOUR PAT>
```

The PAT is used as the password.

## NEVER

- put the PAT in the repo
- put the PAT in the README
- commit the PAT
- paste the PAT into source code
- put the PAT inside the clone URL

---

# 6. Public Clone Check

The marker must be able to clone without credentials.

Use:

```bash
GIT_TERMINAL_PROMPT=0 git clone <repo-url>
```

If this succeeds without asking for:

- username
- password
- PAT
- SSH key

then the repo is clonable correctly.

---

# 7. Build / Run Checks

Use whichever commands match the project.

Common Node project commands:

```bash
npm install
npm run dev
npm run build
npm test
```

Do not assume Qoder saying "complete" means the project works.

Actually run it.

---

# 8. Error Handling Workflow

When something fails:

```text
RUN
↓
READ FIRST USEFUL ERROR
↓
PASTE ERROR INTO QODER
↓
LET QODER FIX
↓
RUN AGAIN
```

Look for:

- filename
- line number
- first useful error message
- HTTP status
- failing command

Do not paste hundreds of irrelevant stack-trace lines if one clear error is enough.

---

# 9. Check the App Yourself

Actually click through the important functionality.

Examples:

```text
[ ] Create
[ ] Edit
[ ] Delete
[ ] Search
[ ] Filter
[ ] Validation
[ ] Navigation
[ ] Refresh
[ ] Persistence
[ ] Error states
```

If the rubric mentions it, test it yourself.

---

# 10. README Requirement

The repo needs clear run instructions.

Example:

```md
# Running the Project

Install dependencies:

npm install

Start the app:

npm run dev
```

If frontend and backend are separate:

```md
# Backend

cd backend
npm install
npm run dev

# Frontend

cd frontend
npm install
npm run dev
```

The commands must work from a **fresh clone**.

---

# 11. Final Rubric Audit Prompt

Use this before submission:

```text
Review the current repository against the COMPLETE rubric.

Do not modify anything yet.

For every rubric criterion classify it as:
- Complete
- Partially complete
- Missing
- Broken

For each criterion:
- show the evidence/file
- explain what is still missing
- estimate the marks currently achieved

Then rank remaining work by:
1. marks gained
2. time required
3. risk of breaking working functionality
```

Then fix the highest-value remaining items.

---

# 12. Final 20-Minute Submission Routine

Do not start a risky major feature near the end.

## Check state

```bash
git status
git diff
```

## Build

```bash
npm run build
```

## Tests, if available

```bash
npm test
```

## Commit and push

```bash
git add .
git commit -m "Final submission"
git push
```

## Verify

```bash
git status
git log --oneline -5
```

You want:

```text
nothing to commit, working tree clean
```

---

# 13. Marker Test

Pretend you are the marker.

```bash
cd ~
rm -rf marker-test

GIT_TERMINAL_PROMPT=0 git clone <repo-url> marker-test
cd marker-test
```

Now follow **only the README**.

If the README says:

```bash
npm install
npm run dev
```

run exactly that.

Check:

```text
[ ] Public repo
[ ] Clone works without auth
[ ] README exists
[ ] README commands work
[ ] Dependencies install
[ ] Build works
[ ] App starts
[ ] Core functionality works
[ ] Latest commit is pushed
[ ] Final commit is before 17:00
```

---

# 14. Time Plan

## 14:30–14:45
- Read brief
- Read rubric
- Understand marks
- Give full brief + rubric to Qoder

## 14:45–15:00
- Get repo/project running
- Confirm Git remote
- Understand structure
- Make first safe commit if needed

## 15:00–16:10
- Implement highest-value requirements
- Test after each meaningful feature
- Commit working milestones

## 16:10–16:35
- Rubric audit
- Fix missing/partial high-value items
- Avoid unnecessary rewrites

## 16:35–16:45
- Build
- Test
- README
- Commit
- Push

## 16:45–16:55
- Fresh clone
- Follow README
- Confirm marker can run it

## Before 17:00
- Final push completed

---

# 15. Most Important Rules

```text
READ THE RUBRIC YOURSELF
↓
GIVE EVERYTHING TO QODER
↓
LET QODER IMPLEMENT
↓
RUN IT YOURSELF
↓
FIX REAL ERRORS
↓
AUDIT AGAINST RUBRIC
↓
COMMIT
↓
PUSH
↓
FRESH CLONE
↓
FOLLOW README
↓
SUBMIT
```

## Remember

**Committed is not submitted.**

You need:

```bash
git commit
git push
```

**Qoder saying it works is not proof.**

You need to run and test it.

**A working local repo is not enough.**

The marker must be able to clone and run the remote repo without authentication.

---

# Emergency Commands

```bash
pwd
ls
git status
git diff
git log --oneline -5
git remote -v

git add .
git commit -m "Save working progress"
git push

npm install
npm run dev
npm run build
npm test
```

Keep it simple. Get the marks. Keep the product working.
