# COMP2850 HCI Assessment: Evaluation & Redesign Portfolio

> **📥 Download this template**: [COMP2850-submission-template.md](/downloads/COMP2850-submission-template.md)
> Right-click the link above and select "Save link as..." to download the template file.

**Student**: [Curtis Lau] [id: 201825792]

**Submission date**: [26/01/2026]
**Academic Year**: 2025-26

---

## Privacy & Ethics Statement

- [Y] I confirm all participant data is anonymous (session IDs use P1_xxxx format, not real names)
- [Y] I confirm all screenshots are cropped/blurred to remove PII (no names, emails, student IDs visible)
- [Y] I confirm all participants gave informed consent
- [Y] I confirm this work is my own (AI tools used for code assistance are cited below)

**AI tools used** (if any): N/A

---

## 1. Protocol & Tasks

### Link to Needs-Finding (LO2)

**Story S1: Keyboard Accessibility**

Situation: When interacting with the UI

Motivation: i want all features to work efficiently with just keyboard

Outcome: so no mouse required i can work using my laptop

Underlying need: Because when i am travelling and working i only carry laptop

Inclusion risk: Motor impairment, RSI, temporary disability, keyboard-only preference

WCAG: 2.1.1 Keyboard A, 2.1.3 Keyboard (No Exception, AAA)

Task Link: All tasks must be sucessfully completed keyboard only variant to show all functions work


**Story S2: Dynamic and Persistent UI**

Situation: When I submit a form (add/edit/delete task)

Motivation: I want immediate, explicit confirmation that the action succeeded

Outcome: So I can trust the interface without refreshing to verify

Underlying need: Because uncertainty about save status causes anxiety and inefficient workarounds

Inclusion risk: Cognitive, Screen reader, Low digital literacy

WCAG: 4.1.3 Status Messages (AA)

Task Link: Actions for T1, T2, T3, T4 are all confirmed at top of site when executed

**Story S3: Text to Speach**
Situation: When I am interacting with UI(buttons, text boxes)

Motivation: I want them all to be labelled correctly

Outcome: So it is compatible with a screen reader

Underlying need: As having audio confirmation gives me comfort

Inclusion risk: Screen reader, Cognitive

Type: Job story

WCAG: 2.4.6 Headings and Labels (AA), 2.4.2 Page Titled (A)

Task Link: All tasks must be sucessfully completed screen reader variant to show all functions can be completed using a screen reader


**Story S4: Task List**

Situation: When I have added a task

Motivation: I want to be able to see a list of all the tasks in order of time added

Outcome: So I can keep track of which ones have priority

Underlying need: Because sometimes i cant keep mental track and forget some tasks

Inclusion risk: Cognitive, ADHD

Task Link: T0 ensures tasks are all displayed correctly seperated into pages, T3 ensures ordered by recent

**Story S5: Error Messages (No-JS)**

Situation: When JavaScript is disabled (corporate firewall, data-saving mode) and I submit invalid data

Motivation: I want an error message to show on screen

Outcome: So I can understand what went wrong and correct it

Underlying need: Because errors can cause stress and anxiety

Inclusion risk: Cognitive

WCAG: 3.3.1 Error Identification (A), 3.3.3 Error Suggestion (AA)

Task Link: T3 displays an error message when adding a task with name less than 3 chars long

---

### Evaluation Tasks (4-5 tasks)

#### Task 0 (T0): [Paginated task list]

- **Scenario**: 
  - "You have been asked to see all current tasks including the older ones on other pages"
- **Setup**
  - Prepopulate task list of over 10 tasks (10 fit on a single page)
- **Action**: 
  - Scroll through all pages until you have seen all the tasks
- **Success**:
  - Participant used the "next" button to go to next page
  - Participant correctly identifies when all pages have been displayed
- **Target time**: 
  - Less than 6 seconds
- **Linked to**: [Week 6 Job Story 4]

#### Task 1 (T1): [Filter Tasks]

- **Scenario**: 
  - "You have been asked to filter all current tasks by "worksheet""
- **Setup**
  - Prepopulate task list with 8 tasks, some of the same type including 3 worksheet tasks
  - Example: Maths Worksheet 1, Programming Project, Hardware Worksheet 1, Maths Worksheet 2,  ....
- **Action**: 
  - Type "worksheet" into filter and resulting list of tasks
- **Success**:
  - Participant types "worksheet" into filter box
  - Participant correctly identifies 3 worksheet tasks
- **Target time**: 
  - Less than 5 seconds
- **Linked to**: [Week 6 Job Story 2]

#### Task 2 (T2): [Edit Task]

- **Scenario**:
  - "You realised you spelt made a spelling mistake in "Ecomomics esay" task and need to correct it"
- **Setup**
  - Task list has one task "Ecomomics esay"
- **Action**: 
  - Use edit button on "Ecomomics esay" to change name to "Economics essay"
- **Success**:
  - Finds and uses edit button on correct task
  - Correctly renames task
- **Target time**:
  - Less than 10 seconds
- **Linked to**: [Week 6 Job Story 2]

#### Task 3 (T3): [Add Task]

- **Scenario**: 
  - "A new task called "t1" has been assigned and you must add this task to your list"
- **Action**: 
  - Try click add task button to add tasked named "t1"
  - Click add task button and type "task1"
- **Success**: 
  - Adding task t1 should produce error message at the top of site
  - New task appears at the end of list with no errors
- **Target time**:
  - Less than 15 seconds
- **Linked to**: [Week 6 Job Story 5] [Week 6 Job Story 2]

#### Task 4 (T4): [Delete Task]

- **Scenario**: 
  - A task in the list needs removing
- **Setup**
  - Task list has one task "Essay 1"
- **Action**:
  - Use the delete button to remove Essay 1
- **Success**:
  - List doesnt show Essay 1 and no errors
- **Target time**:
  - Less than 5 seconds
- **Linked to**: [Week 6 Job Story 2]



---

### Consent Script (They Read Verbatim)

**Introduction**:
"Thank you for participating in my HCI evaluation. This will take about 15 minutes. I'm testing my task management interface, not you. There are no right or wrong answers."

**Rights**:
- [ ] "Your participation is voluntary. You can stop at any time without giving a reason."
- [ ] "Your data will be anonymous. I'll use a code (like P1) instead of your name."
- [ ] "I may take screenshots and notes. I'll remove any identifying information."
- [ ] "Do you consent to participate?" [Wait for verbal yes]

**Recorded consent timestamp**: [P1 consented 14/01/2026 13:56] [P2 consented 16/01/2026 12:30] [P3 consented 19/01/2026 15:01]

---

## 2. Findings Table

**Instructions**: Fill in this table with 3-5 findings from your pilots. Link each finding to data sources.

| Finding | Data Source | Observation (Quote/Timestamp) | WCAG | Impact (1-5) | Inclusion (1-5) | Effort (1-5) | Priority |
|---------|-------------|------------------------------|------|--------------|-----------------|--------------|----------|
| SR button names not announced | metrics.csv L48-50 + P2 notes T4 | P3: "I didn't hear the delete button even though im hovering over it" | 4.1.2 Level A | 5 | 5 | 2 | 8 |
| Hard to navigate without mouse | P2 notes general observation | P2: "I cant really see where i am at the outline is almost same colour as the button" | 2.4.7 Level AA | 4 | 5 | 3 | 6 |
| Cant mark tasks as complete |P1 notes general observation| "So when i finish a task do i just delete it"| -| 5| 1| 5| 1|
|  | | | | | | | |


**Priority formula**: (Impact + Inclusion) - Effort

**Top 3 priorities for redesign**:
1. [Finding #1 - Priority score 8]
2. [Finding #2 - Priority score 6]
3. [Finding #3 - Priority score 1]

---

## 3. Pilot Metrics (metrics.csv)

**Instructions**: Paste your raw CSV data here OR attach metrics.csv file

```csv
ts_iso,session_id,request_id,task_code,step,outcome,ms,http_status,js_mode

[see metrics.csv attached in evidence folder]
```

**Participant summary**:
- **P1**: [Variant Standard mouse + HTMX"]
- **P2**: [Variant Keyboard-only, HTMX-on"]
- **P3** (if applicable): [Variant Screen reader, HTMX-on]

**Total participants**: [n=3]

---

## 4. Implementation Diffs

**Instructions**: Show before/after code for 1-3 fixes. Link each to findings table.

### Fix 1: [No mouse navigation]

**Addresses finding**: [Finding #2 from table above]

**Before** (src/main/resources/templates/base.peb):
```kotlin
// ❌ Problem code
[// no css file linked in base]
```

**After** (src/main.resources/static/css/custom.css: line 49 - 65):
```kotlin
// ✅ Fixed code added css file with:
*:focus {
  outline: 3px solid #f32222;
  outline-offset: 2px;
}

button:focus,
a:focus,
input:focus,
textarea:focus,
select:focus {
  outline: 3px solid #f32222;
  outline-offset: 2px;
}

// In flask html base
  <link rel="stylesheet" href="/static/css/custom.css"> 
```

**What changed**: Added a bolder outline to all buttons when using tab

**Why**: This fixes WCAG 2.4.7 as no mouse users were unable to clearly see which point they were at but this has now been highlighted in a contrasting colour

**Impact**: This improves the navigation for no mouse keyboard only users

---

### Fix 2: [Making buttons same size as text]

**Addresses finding**: [Finding #1]

**Before** (src/main/resources/templates/base.peb):
```kotlin
[ /* Override Pico.css button color for WCAG 1.4.3 AA compliance */
    button[type="submit"],
    button {
      color: white !important; /* White text on blue background for better contrast */
    }
  </style>]
```

**After** (src/main.resources/static/css/custom.css: line 276 - 279):
```kotlin
button {
  width: auto !important;
  display: inline-block !important;
}
```

**What changed**: Now the buttons are same size as text no empty space

**Why**: NVDA doesnt play audio over empty space but expected if over a button

**Impact**: Now when users hover over a button using NVDA it will always read the text

---



---

## 5. Verification Results

### Part A: Regression Checklist (20 checks)

**Instructions**: Test all 20 criteria. Mark pass/fail/n/a + add notes.

| Check | Criterion | Level | Result | Notes |
|-------|-----------|-------|--------|-------|
| **Keyboard (5)** | | | | |
| K1 | 2.1.1 All actions keyboard accessible | A | [pass] | Tested Tab on all buttons |
| K2 | 2.4.7 Focus visible | AA | [pass] | 2px RED outline on all interactive elements (FIXED in fix#1)|
| K3 | No keyboard traps | A | [pass] | Can Tab through filter, edit, delete without traps |
| K4 | Logical tab order | A | [pass] | Starts top to bottom, left to right |
| K5 | Skip links present | AA | [pass] | Skip to main content works |
| **Forms (3)** | | | | |
| F1 | 3.3.2 Labels present | A | [pass] | All inputs have labels |
| F2 | 3.3.1 Errors identified | A | [pass] | Errors have role=alert |
| F3 | 4.1.2 Name/role/value | A | [pass] | All form controls have accessible names (FIXED in fix#2)|
| **Dynamic (3)** | | | | |
| D1 | 4.1.3 Status messages | AA | [pass] | Status messages display at top of screen |
| D2 | Live regions work | AA | [pass] | Tested with error, announces 'Alert' |
| D3 | Focus management | A | [pass] | Prompt to fill in field |
| **No-JS (3)** | | | | |
| N1 | Full feature parity | — | [pass] | All CRUD ops work without JS |
| N2 | POST-Redirect-GET | — | [fail] | double-submit on refresh |
| N3 | Errors visible | A | [pass] | Error summary shown in no-JS mode |
| **Visual (3)** | | | | |
| V1 | 1.4.3 Contrast minimum | AA | [pass] | All text 7.1:1 (AAA) via CCA |
| V2 | 1.4.4 Resize text | AA | [pass] | Text size 200% increased |
| V3 | 1.4.11 Non-text contrast | AA | [pass] | Focus indicator 4.5:1 |
| **Semantic (3)** | | | | |
| S1 | 1.3.1 Headings hierarchy | A | [pass] | "h1 → h2 → h3, no skips |
| S2 | 2.4.1 Bypass blocks | A | [pass] | Skip to main content |
| S3 | 1.1.1 Alt text | A | [pass] | No images in interface OR all have alt |

**Summary**:  19/20 pass, 1/20 fail
**Critical failures** n/a

---

### Part B: Before/After Comparison

**Instructions**: Compare Week 9 baseline (pre-fix) to Week 10 (post-fix). Show improvement.

| Metric | Before (Week 9, n=X) | After (Week 10, n=Y) | Change | Target Met? |
|--------|----------------------|----------------------|--------|-------------|
| SR error detection | 0/1 (0%) | [e.g., 1/1 (100%)] | [+100%] | [✅] |

| WCAG 2.4.7 | fail | pass | [— ] | [✅] |

**Re-pilot details**:
- **P3** (post-fix): repilot already familiar with system, date: 22/01


**Limitations / Honest reporting**:
Very limited results as only tested NVDA with 1 pilot and this pilot is also an expert pilot

---

## 6. Evidence Folder Contents

**Instructions**: List all files in your evidence/ folder. Provide context.

### Screenshots

| Filename | What it shows | Context/Link to finding |
|----------|---------------|-------------------------|
| before-sr.png | Button size bigger than text | Finding #1 - SR button name not announced when hovering blue non text area of button|
| after-sr.png | Button size same as text | Fix #2 verification |
| beforeOutline.png | outline colour similar to button colour | Finding #2 not clear visibilty outline|
| afterOutline.png | Red clear contrast to highlight position | Fix #1 verification|

**PII check**:
- [Y] All screenshots cropped to show only relevant UI
- [Y] Browser bookmarks/tabs not visible
- [Y] Participant names/emails blurred or not visible

---

### Pilot Notes

**Pilot 1 (standard js on)**

P1 consented 14/01/2026 13:56

T0 - 6.57 seconds
pilot had no problems very confident

T1 - 9.49 seconds
noticed took longer than expected as after they filtered they also pressed the "apply filter" button which was unnecessary as the filter updates in real time

T2 - 9.75 seconds
pilot very confident with task

T3 -22.01 seconds
took them 2 attempts of t1 to find error message displayed at top of screen
quote "why cant i add this task" recording timestamp 12.30

T4 - 6.36 seconds
participant said they liked the pop up to verify deletion

Key observation and quote : After testing participant asked about completing task "So when i finish a task do i just delete it" recording timestamp 17.23

**Pilot 2 (no mouse variant)**

P2 consented 16/01/2026 12:30

T0 - 12.19 seconds
observed participant used tab to navigate without a mouse going through each button

T1 - 32.41 seconds
participant tabbed past the filter button and had to cycle though every button in order to go back

T2 - 10 seconds
very confident

T3 - 12 seconds
liked the status message displayed at the top showing errors or sucessful actions

T4 - 9.87 seconds

Key observation and quote: outline colour same as button colour hard to navigate "I cant really see where i am at the outline is almost same colour as the button" recording timestamp 43.12


**Pilot 3 (screen reader variant)**

P3 consented 19/01/2026 15:01

T0 - 10.55 seconds
very confident

T1 - 10.12 seconds
liked the sound queue when using a text box and buttons

T2 - 13.17 seconds
very confident

T3 - 17.49 seconds
NVDA screen reader automatically read out errors and updates without hovering over
Says "alert" when error occurs which gave participant more direct answer

T4 - 14.80 seconds
Participant noticed clicking the button doesnt necessarily lead to an audio output if not hovering over text "I didn't hear the delete button even though im hovering over it" recording timestamp 13.56

**Pilot 3 expert**

T4 - 5.40 seconds
quote "great looks like it can read the button now" recording timestamp 00.03

**Flagged anomalies**

js mode starts as off when reloading the page 

## Evidence Chain Example (Full Trace)

**Instructions**: Pick ONE finding and show complete evidence trail from data → fix → verification.

**Finding selected**: Finding #1 - SR not announced for button

**Evidence trail**:
1. **Data**: metrics.csv lines 48-50 show P3 (SR user) took around 16 seconds to complete task which is over target time of 5 seconds
2. **Observation**: P2 pilot notes - Quote: "I didn't hear the delete button even though im hovering over it"
3. **Screenshot**: before-sr.png shows there is large button space without text and unable to be read
4. **WCAG**: 4.1.2 name/role/value (Level A) violation 
5. **Prioritisation**: findings-table.csv row 1 - Priority score 8 (Impact 5 + Inclusion 5 - Effort 2)
6. **Fix**: implementation-diffs.md Fix #2 - decreased button size to match text
7. **Verification**: verification.csv Part A row F3 - 4.2.1 now PASS (tested with NVDA)
8. **Before/after**: verification.csv Part B - SR detection improved from 0% to 100%
9. **Re-pilot**: P3 (SR user) pilot notes - "great looks like it can read the button now"

**Complete chain**: Data → Observation → Interpretation → Fix → Verification ✅

---

## Submission Checklist

Before submitting, verify:

**Files**:
- [Y] This completed template (submission-template.md)
- [Y] metrics.csv (evidence folder)
- [Y] Pilot notes (summarised in Section 6)
- [Y] Screenshots folder (all images referenced above)
- [Y] Privacy statement signed (top of document)

**Evidence chains**:
- [Y] findings-table.csv links to metrics.csv lines AND/OR pilot notes timestamps
- [Y] implementation-diffs.md references findings from table
- [Y] verification.csv Part B shows before/after for fixes

**Quality**:
- [Y] No PII in screenshots (checked twice!)
- [Y] Session IDs anonymous (P1_xxxx format, not real names)
- [Y] Honest reporting (limitations acknowledged if metrics didn't improve)
- [Y] WCAG criteria cited specifically (e.g., "3.3.1" not just "accessibility")

**Pass criteria met**:
- [Y] n=2+ participants (metrics.csv has 2+ session IDs)
- [Y] 3+ findings with evidence (findings-table.csv complete)
- [Y] 1-3 fixes implemented (implementation-diffs.md shows code)
- [Y] Regression complete (verification.csv has 20 checks)
- [Y] Before/after shown (verification.csv Part B has data)

---

**Ready to submit?** Upload this file + evidence folder to Gradescope by end of Week 10.

**Estimated completion time**: 12-15 hours across Weeks 9-10

**Good luck!** 🎯