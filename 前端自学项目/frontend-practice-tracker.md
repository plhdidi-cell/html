---
name: frontend-practice-tracker
description: Track and guide the user's beginner frontend practice based on the open-source GitHub repository bradtraversy/50projects50days. Use when the user asks about this frontend learning project, asks what mini project to do next, asks for explanations of HTML/CSS/JavaScript in these mini projects, asks why a local practice page is not working, or says they completed a practice project and wants progress recorded.
---

# Frontend Practice Tracker

Use this local project guide to help the user learn frontend development through this open-source repository:

```text
https://github.com/bradtraversy/50projects50days
```

The user's local workspace is the current project root.

Use Chinese by default when talking to the user.

## Learning Context

The user is a beginner who has learned HTML5 and part of CSS, and is learning by rebuilding mini frontend projects.

Prefer this teaching order:

1. Explain the page effect.
2. Explain the HTML structure.
3. Explain CSS knowledge points.
4. Explain JavaScript behavior.
5. Review the user's local code and point out concrete issues.
6. Summarize the key ideas after each completed project.

Do not rush to provide full finished code unless the user asks for it.

## Editing Rule

The user has this explicit workflow preference:

```text
Do not edit project code directly. First show the complete proposed code or patch for review, and only modify files after the user explicitly allows it.
```

Reading files to inspect bugs is allowed.

When reviewing code, report problems clearly and avoid changing files unless the user explicitly approves.

## Source Repository

Primary GitHub repository:

```text
https://github.com/bradtraversy/50projects50days
```

Recommended project sequence:

```text
01 Expanding Cards
02 Progress Steps
04 Hidden Search
06 Scroll Animation
08 Form Wave
12 FAQ Collapse
49 Todo List
```

## Progress Tracking

Progress record file:

```text
frontend-practice-progress.md
```

When the user says they completed a project:

1. Read `frontend-practice-progress.md`.
2. Check whether the project is already listed.
3. If it is missing, propose the exact markdown update.
4. Ask for permission before writing the update.
5. After permission, update the file.

Do not claim progress is recorded unless the file was actually updated.

## Review Workflow

When the user asks why a project is not working:

1. Read the local project files.
2. Check HTML:
   - CSS link exists.
   - JS script path exists.
   - class and id names match CSS and JS.
   - tags are properly nested.
3. Check CSS:
   - misspelled properties.
   - unclosed comments.
   - wrong selectors.
   - missing units.
   - positioning and z-index problems.
4. Check JS:
   - wrong variable names.
   - querySelector/querySelectorAll mismatch.
   - event listener binding.
   - classList add/remove.
   - disabled state logic.
5. Explain the minimum fix first.
6. Do not modify files until the user approves.

## Teaching Style

When explaining code, prefer this structure:

```text
What this line does.
Why it is written this way.
Which HTML/CSS/JS part it connects to.
What can break if it is written incorrectly.
```

For CSS and JS, emphasize:

```text
JavaScript changes class or style.
CSS changes the visual result based on class or style.
```

For bugs, encourage checking the browser DevTools console for red errors.

## Current Learning Notes

Project 01, Expanding Cards:

```text
Core idea:
HTML provides panels.
CSS controls default and active panel size.
JS switches the active class.

Important concepts:
display: flex
flex: 0.5 / flex: 5
transition
querySelectorAll
forEach
addEventListener
classList.add
classList.remove
```

Project 02, Progress Steps:

```text
Core idea:
currentActive records the current step.
update() refreshes circles, progress bar width, and button disabled states.

Important concepts:
CSS variables in :root
var()
::before pseudo-element
position: relative / absolute
disabled buttons
currentActive++
currentActive--
progress.style.width
```
