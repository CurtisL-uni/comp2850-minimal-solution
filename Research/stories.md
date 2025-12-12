## Story S1: keyboard accessibility
**Situation**: When interacting with the UI
**Motivation**: i want all features to work efficiently with just keyboard
**Outcome**: so no mouse required i can work using my laptop
**Underlying need**: Because when i am travelling and working i only carry laptop

**Inclusion risk**: Motor impairment, RSI, temporary disability, keyboard-only preference
**Type**: Job story
**WCAG**: 2.1.1 Keyboard A, 2.1.3 Keyboard (No Exception, AAA)


## Story S2: dynamic and persistent UI
**Situation**: When I submit a form (add/edit/delete task)
**Motivation**: I want immediate, explicit confirmation that the action succeeded
**Outcome**: So I can trust the interface without refreshing to verify
**Underlying need**: Because uncertainty about save status causes anxiety and inefficient workarounds

**Inclusion risk**: Cognitive, Screen reader, Low digital literacy
**Type**: Job story
**WCAG**: 4.1.3 Status Messages (AA)

## Story S3: text to speach 
**Situation**: When I am interacting with UI(buttons, text boxes)
**Motivation**: I want them all to be labelled correctly
**Outcome**: So it is compatible with a screen reader
**Underlying need**: As having audio confirmation gives me comfort  

**Inclusion risk**: Screen reader, Cognitive
**Type**: Job story
**WCAG**: 2.4.6 Headings and Labels (AA), 2.4.2 Page Titled (A)


## Story S4: task list 
**Situation**: When I have added a task
**Motivation**: I want to be able to see a list of all the tasks in order of time added
**Outcome**: So I can keep track of which ones have priority
**Underlying need**: Because sometimes i cant keep mental track and forget some tasks

**Inclusion risk**: Cognitive, ADHD
**Type**: Job story

## Story S5: Persistent Error Messages (No-JS)
**Situation**: When JavaScript is disabled (corporate firewall, data-saving mode) and I submit invalid data
**Motivation**: I want error messages to persist after page reload
**Outcome**: So I can understand what went wrong and correct it
**Underlying need**: Because ephemeral error messages (lost on redirect) require perfect memory or multiple submission attempts

**Evidence**: Inferred from Lab 1 no-JS testing; no explicit interview mention (add if time)
**Inclusion risk**: Cognitive, screen reader (needs page-level error summary)
**Type**: Pain point (internally identified)
**WCAG**: 3.3.1 Error Identification (A), 3.3.3 Error Suggestion (AA)