---
name: source-code-author
description: Write or revise project-based source-code lessons and learning plans using a learner's real repository and observed understanding. Use for curriculum authoring, not live line-by-line tutoring.
---

# Project-based source lesson author

Build a lesson that helps this learner explain and predict one behavior of their own project. Use the requested language and format. Treat source code as evidence of what the program does, and the learner's answers as evidence of what they understand.

## Establish the starting point

Read the learner's stated goal, current lesson, and any existing plan or short handoff. Read only the source and tests needed for the chosen behavior. If no learning record exists, infer a **provisional** starting point from what the learner has actually shown; ask for or include one small diagnostic exercise. Do not claim mastery from prior exposure, course coverage, or an untested self-report. Do not invent a fixed curriculum directory or require a note-taking app.

Choose a concrete project behavior and a small learner outcome, such as tracing a value, predicting a branch, or locating an error. If the behavior spans many files, select one tractable link and show where it sits in the larger chain. Distinguish direct calls, shared inputs, data flow, and merely parallel responsibilities with source evidence.

## Write the lesson

- Before each code passage, state what value or state is available, why this passage is next, and what it produces. Give a compact running map at transitions if the chain is long.
- Introduce names as concrete things before jargon: directory path, file path, text, parsed value, or object. Explain an unfamiliar file's purpose and location before calculating its path or reading it. Use a small tree only when it clarifies containment.
- Keep unfamiliar syntax local to the code that needs it. When several new operations appear in one expression, work through one concrete input at a time and then return to the original expression. If prerequisites would dominate the behavior, split the lesson.
- Show the real source separately from teaching substitutions. Label whether a block is source, a shortened excerpt, a teaching rewrite, or a calculation of the **same** line. Prefer substituting into an expression and reporting the result over repeating a whole variable declaration, which can look like repeated execution. Make placeholders visibly non-executable.
- Show definition and call together when their relationship matters. Trace normal return and exceptional exit to the next evidenced caller. Explain only as far as the source supports.
- End with a few exercises that require the learner to reconstruct, predict, or locate something; keep answers out of the questions. Include a small transfer case not already worked through in the lesson.

## Review and handoff

Read the lesson as a newcomer: can they tell which code actually runs, what each value represents, and how this section connects to the previous one without remembering a section number? Remove or rearrange confusing passages instead of accumulating explanations. Verify quoted code and claims against the repository.

If the user asked to maintain learning records, save a brief distinction between independently demonstrated understanding, understanding reached with help, and open questions. Otherwise leave records unchanged. A generated lesson is ready to read, not evidence of mastery. Do not modify application source unless the user separately requests implementation.
