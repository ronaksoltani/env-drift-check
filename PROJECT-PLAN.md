# Project plan: Env Drift Check

## Brief

**Type:** Local-first developer tool

**Audience:** Developers maintaining local and deployment environments.

**Problem:** Compare an example env file with a local environment snapshot. See missing, extra and duplicate key names while keeping every value out of the report.

## Experience flow

1. Read the scope and privacy boundary before entering data.
2. Load the fictional sample or paste authorized input.
3. Run the local analysis and inspect each rule or calculation.
4. Copy or download a draft only when the user chooses.

## Core capabilities

- Compare .env.example and current key sets
- Find missing, unexpected and duplicate names
- Copy blank placeholders for missing keys
- Never display or persist environment values

## Key design decision

Keep the application self-contained and explain what is heuristic, human-reviewed or user-configured. Never imply that a demo replaces a production control.

## Boundaries

Paste only data you are authorized to inspect. The app parses key names and discards values from its report; it does not edit files or validate whether a value is correct.

## Learning goals

- Keep input handling, analysis and rendering in clear small functions.
- Make empty, invalid and successful states visible and accessible.
- Use semantic HTML, labelled fields, keyboard focus and responsive CSS.
- Document assumptions, local data handling and limitations.

## Next iteration

Add user research and domain-specific validation rules, then document those rules with examples before expanding scope.
