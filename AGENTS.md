# AGENTS.md

Claude and Codex collaborate in this repo. Claude (in chat) writes task
specs and reviews results. Codex implements.

## Rules for Codex
- Do one task at a time, exactly as written in the task text you are given.
- Change only the files listed under "Files in scope". Do not touch anything
  under "Out of scope".
- If the spec is unclear or seems wrong, ask instead of guessing.
- Run the verification command before finishing, and fix any failures.
- Work on a branch named task/NNN-name. Do not push directly to main.
- Never commit secrets, keys, or .env files.
- Finish with a report in the report format below.

## Task format (written by Claude)
- Goal
- Files in scope
- Out of scope
- Acceptance criteria (checkable by a command)
- Verification command

## Report format (written by Codex)
- Summary of what was done
- Files changed
- Verification command run and its result
- Deviations from the spec, and why
- Open questions

## Commands
- Install: TODO
- Test: TODO
- Lint: TODO
