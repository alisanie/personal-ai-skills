---
name: laravel-issue-writer
description: Write focused Laravel issues in Persian from user requests, code review reports, or repository findings. Use when turning Laravel work or findings into actionable issues.
---

# Laravel Issue Writer

Turn a user's description, an HTML/Markdown Code Review report, or findings from direct repository inspection into clear, actionable Laravel issues. Apply the same issue standard regardless of the source.

## Before writing

- Identify the actual problem, where it occurs, and the relevant scenario. If essential facts are missing or ambiguous, ask only the minimum questions needed to avoid a misleading issue; decide minor details reasonably.
- Check whether findings overlap. Group duplicate or closely related findings when one issue gives the developer a coherent task. Avoid creating tiny issues for low-value details.
- For findings from code or reports, include useful context such as file path, Class, Method, or location when available and reasonably verified. Do not invent locations.

## Write the issue

- Write primarily in Persian. Keep technical terms in English where natural, including Session, Cache, Queue, Job, Middleware, Controller, Action, API, and Feature Test. Do not coin Persian equivalents for them.
- Use an adaptive structure. Include only sections that help with this issue: **Problem**, **User Story**, location/scenario, **Proposed Solution**, **Suggested Code**, **Tests**, and **Definition of Done**. A maintenance task such as a Laravel upgrade does not need a forced User Story.
- Make **Problem** and the location/scenario concrete enough that the developer understands what fails, where, and under what conditions.
- Keep **Proposed Solution** correct and directional. State the desired behavior and relevant constraints without dictating a line-by-line implementation.
- Add **Suggested Code** only when a short, illustrative snippet clarifies intent. Do not provide a complete copy/paste implementation.
- Specify a small set of simple, directly relevant **Tests** covering essential scenarios, and state that these tests must pass. Avoid a large or complex test suite.
- End with a short, practical **Definition of Done**, usually 2–5 checkboxes.

The issue should give the developer enough context to act while leaving room to choose a sound implementation.
