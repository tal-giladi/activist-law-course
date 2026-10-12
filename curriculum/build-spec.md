# Build spec for module writers

You write ONE module of "Activist Law: A Free Practical Course".

## Before you write: read, in this order

1. `C:\Users\TalGiladi\OneDrive\repos\tals-academy\docs\new-course-instructions.md`. It is binding.
2. `curriculum/plan.md`. The parts that matter most:
   - §0.1 (approved deviations)
   - §1 (positioning and the s.20 limit)
   - §3 (language)
   - §4 (external resources)
   - §5 (neutrality)
   - §6 (your module's lesson list)
   - §7 (lesson format)
   - §8 (practical design)
3. This file.
4. Your module's section in `curriculum/research/sources-israel.md` or `curriculum/research/sources-international.md`, and the numbers table at the top of `sources-israel.md`.
5. `references/current-numbers.md`.
6. One finished module, if one exists, to match its tone.

## Hard limits for agents

- **Do not spawn sub-agents. Work sequentially.** Tal's rule is that no more than 2 agents run in total.
- **Shared files are off-limits.** Never edit:
  - `_sidebar.md`, `README.md`, `glossary.md`
  - `references/`, `templates/`
  - `BUILD_PROGRESS.md`, `curriculum/plan.md`
  - another module's files
- **Never commit or push.** The main session does that.

## What you produce for module NN

**Lessons.** For every lesson listed in plan §6 (exact count and ids; you may polish the titles):

- `lessons/module-NN/lesson-MM.md`
- `lessons/module-NN/lesson-MM.quiz.yaml` (3–5 questions)

**Module quiz:**

- `assessments/module-NN-quiz.md`. A short intro, a "Revisit by topic" list that links each lesson, and a link to the project. No questions and no answers.
- `assessments/module-NN-quiz.quiz.yaml`. 10 scenario questions.

**Project.** `projects/mNN-<slug>.md`, using the slug in plan §6. It must contain:

- the brief and the steps;
- a self-assessment rubric (a table);
- a model answer in `<details><summary>Model answer</summary>…</details>`.

**Question bank.** `curriculum/question-bank/module-NN.yaml` holds **at least 60, ideally 80–100** extra practice questions for Tal's daily practice tool (§ Question bank below).

**Inboxes.** The main session merges these into the shared files:

- `curriculum/glossary-inbox/module-NN.md`, one term per line: `- **מונח** (transliteration) — English meaning.`
- `curriculum/inbox/module-NN-numbers.md`: any fee, deadline or ceiling you used, with its source URL and the date you checked it, that is not already in `references/current-numbers.md`.
- `curriculum/inbox/module-NN-external.md`: every external resource you assigned. One line each: URL, tag, signup (y/n), language, length, the lessons that use it, `last_checked`.
- `curriculum/inbox/module-NN-laws.md`: every law and ruling you cited, with its free full-text URL.
- `curriculum/inbox/templates/<name>.md`: complete drafts of any template your lessons need. A lesson links to the future path `../../templates/<name>.md`; the main session moves the draft there before the check runs.

**Progress.** Append `lesson-MM done` to `curriculum/status/module-NN.log` after each lesson (md + quiz). Append `module done` at the end.

**Check.** Run `node curriculum/tools/check-module.mjs NN` from the course root until it reports `0 problems`. Template links count as broken until the main session moves the drafts; ignore only those warnings, and list them in your final report.

## Lesson format

Use the exact front-matter and the 9 `##` sections in plan §7, in that order. Use `###` inside them.

**Objectives.** 2–4 per lesson, each quoted and measurable ("Find…", "Write…", "Decide…").

**Sources.** Every legal claim cites a primary source in `sources`. You may cite only URLs you opened with WebFetch, or that `sources-*.md` marks ✅.

- gov.il and kolzchut.org.il block bots. If one of their URLs is in the research file, you may use it and note `(⚠️ manual check)` in your inbox file.
- **Never cite Nevo case-law pages.** They are paid.

**Key terms.** A table: `| עברית | Transliteration | English |`.

**The law.**

- Quote the Hebrew text exactly, in a blockquote.
- Follow each quote with `*Gist:*` and one English sentence.
- Then a link to the free full text.
- Keep quotes short: only the sections the lesson needs.

**Numbers.** Never write a fee, ceiling or deadline as a bare fact. Link `../../references/current-numbers.md`. You may say "a fee of about ₪24 (see current numbers)".

**Do it yourself.** Use the subsections from plan §7.

- The default level is a dry run on a real issue the learner chooses.
- Every real-world filing step opens with `> [!IMPORTANT]` and the text: "Act in your own name only. This is not legal advice — check current rules before filing."

**Learn more.** Assign external units per plan §4:

- the exact deep link;
- the tag (FREE-FULL or FREE-AUDIT, never PAID);
- the minutes;
- a fallback.

Write "None." if there are none.

**Worked example.** A realistic Israeli case. Rotate causes across the political spectrum (plan §5). Use invented names for private persons; real public bodies are fine.

**Safety.** Police, arrest and documentation content opens with `> [!WARNING]`.

**Language.** English prose and Hebrew legal text, as plan §3 sets out. Do not translate statutes. Give English gists only.

## Quizzes (lesson and module)

Follow guidelines §5.

- Exactly 4 options, `correct` 0–3, spread across positions, with an `explanation`.
- No "all/none of the above".
- The correct option is not the longest.
- Questions are realistic decisions, for example:
  - "A ministry ignored your FOI request for 40 days — what now?"
  - "Which source wins: a regulation or a Basic Law?"
- Use `>-` scalars for every text field. Hebrew is allowed inside the text.

## Question bank (Tal's daily practice — tool not built yet)

The file is `curriculum/question-bank/module-NN.yaml`. It is not imported. Later it will feed a daily practice tool that draws questions only from modules the learner has finished.

Format: the quiz format plus four fields.

```yaml
- id: m01-001                  # m<NN>-<3 digits>, unique, never reused
  module: 1
  lesson: "01.3"               # the lesson the question practises
  subject: hierarchy-of-norms  # kebab-case topic; reuse the same subject names across the module
  difficulty: 2                # 1 recall-plus, 2 apply, 3 tricky real-world decision
  question: >-
    …
  options:
    - >-
      …
    - …
  correct: 2
  explanation: >-
    …
```

- At least 60 questions per module, and about 10 per lesson. Mix the difficulties: roughly 30% level 1, 45% level 2, 25% level 3.
- Questions must be **different** from the lesson and module quiz questions: new scenarios, not rewordings.
- Cover every lesson and every key term. Include "spot the mistake in this letter or request" questions and "which forum or tool" questions.
- The same quality rules as quizzes: 4 options, one correct, plausible distractors, spread `correct`, and the correct option not the longest.
- Parse the file after writing. The checker validates it.

## Final report (under 200 words)

Include the module total time estimate (plan §16): lessons minutes + practice_minutes + project time + 30 min quizzes, rounded to hours.

Your final report must cover:

- the files you wrote;
- the question count;
- the checker result;
- template links waiting to be moved;
- any ⚠️ facts you could not verify;
- anything Tal must decide.
