# Project-based source learning skills

Two small, complementary Codex/agent skills for learning programming through an existing codebase.

- [`source-code-author`](source-code-author/SKILL.md) drafts a learning plan or lesson from the learner's project and observed answers.
- [`source-code-tutor`](source-code-tutor/SKILL.md) helps the learner read one current code passage and checks understanding without turning every reply into a long lecture.

The skill instructions are written in English and tell the agent to use the learner's requested language. They do not require a particular programming language, framework, editor, note-taking app, or project directory layout. Copy either skill folder into the skills directory used by your agent. They can be installed separately. In a project-specific setup, put personal learning preferences and exclusions in that project's own instructions or handoff; keep them out of the reusable skills.

Example requests:

```text
Use $source-code-author to make the first lesson from this repository. I know basic Python but have not read this project's JavaScript. Start with one observable behavior and give me an exercise before marking anything learned.

Use $source-code-tutor to help me read the selected function. First find out what I think it does; when I ask about a term, explain that term directly.
```

The author works without an existing plan or handoff: it makes a provisional baseline from available evidence and revises it after the learner answers. The tutor can start from a selected snippet without loading an entire repository. Neither skill treats having read a lesson as proof of mastery. If records are requested, keep observed answers distinct from tentative inferences.

## Maturity and evidence

Experimental. These rules were developed while one learner studied one JavaScript project. They address observed problems such as losing track of a long data flow, mistaking teaching substitutions for successive code execution, and confusing paths with file contents. They have **not** been validated across multiple projects, languages, learners, or smaller assistant models. A syntactically valid `SKILL.md` is not evidence of teaching quality. Please test with a different repository and learner before relying on it broadly; feedback and counterexamples are welcome.

No user project files, learning history, or example source code are included in this package.

## License

MIT. See [LICENSE](LICENSE).
