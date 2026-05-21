# Outcome Logging Skill

## Purpose
This skill defines a reusable workflow for capturing the outcome of an interaction, attaching a timestamp, and saving it as a text file in a project-specific folder.

## When to use
Use this skill when you want to log the result of a task, decision, or generated output so it can be referenced later.

## Workflow
1. Receive the outcome summary or suggested result from the user or agent.
2. Create a timestamp in a standard format such as `YYYY-MM-DD HH:mm:ss`.
3. Determine the project-specific log folder (for example, `./claude/memory` or another folder inside the current workspace).
4. Write a text file named with the timestamp and a short slug, for example: `2026-05-19_13-45-00_outcome.txt`.
5. Save the content with a header containing the timestamp and the outcome detail.

## Output format
The generated text file should include:
- `Timestamp: YYYY-MM-DD HH:mm:ss`
- `Outcome: <brief description>`
- `Details: <expanded summary or suggested result>`

Example file content:
```
Timestamp: 2026-05-19 13:45:00
Outcome: Created a thought-leader prompt template.
Details: Added a reusable prompt that turns thought starters into concise Justin Welch-style posts with icons and sources.
```

## Notes
- The skill is project-scoped and should save logs in a workspace-specific folder.
- If the folder does not exist, create it before saving.
- Use a consistent timestamp-based filename pattern to avoid collisions.
- Keep the logged outcome concise and actionable.
