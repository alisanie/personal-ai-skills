---
name: laravel-issue-writer
description: Write focused Laravel issues in Persian from user requests, code review reports, or repository findings. Use when turning Laravel work or findings into actionable issues.
---

# Laravel Issue Writer

Turn a user's description, an HTML/Markdown Code Review report, or findings from direct repository inspection into clear, actionable Laravel issues.

Apply the same issue standard regardless of the source. Give the developer enough context to understand and solve the problem without dictating the implementation.

## Before writing

- Identify the actual problem, where it occurs, and the relevant scenario.
- Distinguish verified behavior from assumptions, symptoms, and possible root causes.
- If essential facts are missing or ambiguous, ask only the minimum questions needed to avoid a misleading issue. Decide minor details reasonably without unnecessary follow-up questions.
- Check whether findings overlap. Group duplicate or closely related findings when one issue gives the developer a coherent task.
- Avoid creating tiny issues for low-value details that do not justify a separate task.
- For findings from code or reports, include useful context such as file path, Class, Method, or location when available and verified.
- Never invent or present an unverified file, Class, Method, behavior, or root cause as fact.

## Write the issue

- Give the issue a short, specific title that clearly describes the problem or required change.
- Write primarily in Persian.
- Keep technical terms in English where natural, including Session, Cache, Queue, Job, Middleware, Controller, Action, API, Feature Test, Request, Response, Validation, Authentication, Authorization, Migration, Model, Service, Event, Listener, and similar terms.
- Do not create Persian equivalents for technical terms when the English term is the normal terminology.

Use an adaptive structure. Include only sections that help explain the specific issue.

Possible sections include:

- **Problem**
- **User Story**
- **Location / Scenario**
- **Proposed Solution**
- **Suggested Code**
- **Tests**
- **Definition of Done**

Do not force every section into every issue. For example, a maintenance task such as a Laravel upgrade usually does not need a User Story.

### Problem

Clearly explain:

- What is wrong or needs to change.
- Where the problem appears.
- Under what conditions or scenario it occurs.
- Why it matters when that context is useful.

Describe observed symptoms separately from suspected root causes when the root cause has not been verified.

### User Story

Add a User Story only when it improves understanding of the expected behavior.

When useful, prefer a simple form such as:

> به عنوان [user/role] می‌خواهم [behavior] تا [goal].

Do not add a User Story to maintenance, infrastructure, refactoring, upgrade, or other tasks where it would be artificial.

### Location / Scenario

When the issue comes from Code Review, repository inspection, or a technical report, reference relevant context when verified, such as:

- file path
- Class
- Method
- Route
- relevant flow or scenario

Provide enough context for the developer to locate the problem quickly without turning the issue into a step-by-step implementation guide.

### Proposed Solution

Keep the proposed solution correct and directional.

Describe:

- the desired behavior,
- important constraints,
- relevant Laravel conventions or architectural considerations when useful.

Do not dictate a line-by-line implementation.

The developer should still evaluate the codebase and choose a sound implementation.

### Suggested Code

Add Suggested Code only when a short snippet materially clarifies the intent.

Suggested Code must be:

- short,
- illustrative,
- directly related to the issue.

Do not provide a complete copy/paste implementation.

### Tests

Tests are an important part of the issue.

Specify a small set of simple, directly relevant tests covering the essential behavior.

Prefer tests that verify:

- the main expected behavior,
- the important failure or edge case when relevant,
- security or authorization behavior when directly related to the issue.

Avoid creating a large or unnecessarily complex test suite.

The required tests must pass before the issue is considered complete.

### Definition of Done

End with a short and practical checklist, usually 2–5 items.

Include only conditions that are genuinely required to consider the issue complete.

Example:

- [ ] رفتار موردنظر پیاده‌سازی شده است.
- [ ] scenario اصلی مشکل دیگر قابل بازتولید نیست.
- [ ] Tests مرتبط اضافه یا به‌روزرسانی شده‌اند.
- [ ] تمام Tests مرتبط pass می‌شوند.

## Guiding principle

An issue should explain **what is wrong, where it happens, what behavior is expected, and how completion will be verified**.

It should guide the developer without replacing the developer's technical judgment.
