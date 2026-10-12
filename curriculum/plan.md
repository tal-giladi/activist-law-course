# Activist Law — course plan

A free, practical online course in law for activists ("Activist Law: A Free Practical Course"; never call it a degree). It covers about half an Israeli LL.B.: public law, human rights and international law, plus a practical stage. The goal is that a learner can act alone, without hiring a lawyer.

Written 2026-10-12. Status: plan + research done. No lessons written yet.

## 0. Binding build rules — read first

> **Course guidelines (binding):** before writing or changing anything in this course, read
> `C:\Users\TalGiladi\OneDrive\repos\tals-academy\docs\new-course-instructions.md` in full.
> It wins over this plan, except for the two deviations Tal approved in chat (§0.1).

The rules from that file that matter most here:

- Work only in this folder (`course-creator\activist-law-course`), never in the Academy repo.
- Plain markdown and YAML only.
- Repo layout, `_sidebar.md`, front-matter and file names exactly as specified there.
- Every graded question is multiple choice in a `.quiz.yaml`:
  - 4 options, 1 correct, with an explanation.
  - 3–5 questions per lesson.
  - 8–10 scenario questions per module quiz.
  - Pass mark 70%.
- Learning by doing. Every lesson ends in something the learner does. Every module ends in a larger practical piece (§8).
- Always current. Verify every legal claim, fee, deadline and URL against a primary source before writing. Record `sources` and `last_verified`.
- **At most two agents running at once, counted across the whole tree. Sub-agents never spawn sub-agents.**
- Keep `BUILD_PROGRESS.md` and `curriculum/status/module-NN.log` up to date. Commit after every module.
- Run `npm run check-course -- ../course-creator/activist-law-course` from the Academy repo after every module, until it reports `0 problems`.
- Do not create course-details again — `curriculum/course-details.md` exists (§13).

### 0.1 Deviations approved by Tal (2026-10-12)

1. **Language: mixed English/Hebrew** instead of English only. Rules are in §3.
2. **External free platforms are part of the learning path.** When a free external course, video series or guide already teaches something well, the lesson sends the learner there instead of copying it. Rules are in §4.

## 1. Purpose and honest positioning

**Purpose.** After the course, the learner can do all of the following personally, without paying a lawyer:

- Research the law.
- Write and file Freedom of Information requests, complaints, planning objections and pre-petition letters.
- Represent themselves in small claims, administrative petitions and High Court petitions.
- Take part in Knesset and local-council processes.
- Use UN human-rights mechanisms.
- Document violations.
- Organise others.

**What it is not.** It is not a law degree, does not lead to the bar exam, and does not make anyone a lawyer.

Use this standard wording in README, lesson 01.1 and the certificate:

> "This free course teaches you to act for yourself in Israeli and international legal processes. It is not a law degree, does not license you to practise law, and is not legal advice."

**The legal limit we teach early and repeat.** In Israel, people may represent *themselves*. Bar Association Law 1961, s. 20 reserves certain acts to lawyers when they are done for another person "דרך עיסוק, או בתמורה" (as an occupation, or for payment). The reserved acts are:

- representing another person,
- drafting legal documents for another person,
- legal advice.

Breaking this is an offence under s. 96, punished by a fine.

Further rules, all quoted in `research/sources-israel.md` M18:

- The 2009 Bar ethics decision on NGOs.
- The Medical Rights Centre ruling. Its case number is still unconfirmed.
- The working rule from that ruling: general legal information is allowed; individual advice is not.

Lessons 01.1 and 18.4 teach where the line is. Acting for yourself, sharing general information, and helping a group act in its own name are all fine. Every template says "for use in your own name". No lawyer review before publishing (Tal, 2026-10-12): lesson 18.4 opens with a `> [!IMPORTANT]` "not legal advice — this is our reading of the law text" notice.

**Not legal advice.** Every module that ends in a real-world action reminds the learner of this.

## 2. Target learner

An Israeli resident, any age 16+, with no legal background. They care about a cause, from any political direction. They are comfortable with Hebrew bureaucracy, and they read English well enough for online courses.

They have a computer, an Israeli ID, and access to government online identification (הזדהות לאומית).

## 3. Language policy (mixed EN/HE)

The principle is that each piece of content goes in the language the learner will actually use it in.

| Content | Language |
|---|---|
| Lesson prose, explanations, worked examples | English |
| Israeli statute text, quoted rulings, official forms, form fields | Hebrew, quoted exactly, never translated. A one-line English gist follows each quote. |
| Templates the learner files in Israel (letters, FOI requests, objections, petitions, affidavits) | Hebrew (that is what gets filed), with English instructions around them |
| International material (UN, ICJ, ICRC, MOOCs) | English |
| Legal terms | `Key terms` table: Hebrew \| transliteration \| English meaning |
| Quizzes | English. Hebrew terms or short quotes may appear inside questions. |
| External resources | Their original language. Never translated. |

- Hebrew paragraphs go in blockquotes (`> …`) so the right-to-left text sits on its own lines.
- Never mix Hebrew and English inside one sentence, except for single terms.
- YAML: UTF-8. Use `>-` scalars for anything with Hebrew punctuation (`"`, `׳`, `:`).

## 4. External resources policy

**When to send learners out.** The lesson sends learners out when a free external resource teaches the topic at least as well as we would. The lesson then does three things:

1. Frames it: why, and what to watch for.
2. Assigns an exact unit: a deep link, the chapter or episode, and the minutes.
3. Turns it into practice and a quiz on our side.

We never copy external material.

**Allowed tags.** Every external resource is listed once in `references/external-resources.md` with one of these tags:

- **FREE-FULL** — everything free, no expiry. Preferred.
- **FREE-AUDIT** — content free with limits, e.g. an edX audit that expires. Allowed only if the assigned unit is free and the limit is stated in the lesson ("audit is free for N weeks; enrol only when you start module X").
- **PAID / UNAVAILABLE** — never assigned. Kept in a separate list so nobody re-adds it.

**Required fields** for every entry: URL, tag, signup needed (y/n), language, length, the lessons that use it, and `last_checked`.

**Fallback.** Every assigned external unit has a fallback: a second free source, or a short summary in our lesson. A dead link must never block a learner.

**Re-checking.** Before each module is written, the writer re-opens every external link it uses (WebFetch) and updates `last_checked`. A link that has not been opened is not assigned.

## 5. Neutrality

The course teaches tools, not positions.

- Examples, worked cases and NGO lists cover causes across the political spectrum: civil rights, religious freedom, property rights, environment, disability, good governance, settlers' and Palestinians' petitions, and protests from left and right.
- Contested matters (judicial reform, the territories, ICJ/ICC proceedings) are presented with official Israeli government positions next to UN, court and NGO positions. Each claim is attributed.
- Quizzes test the law and the procedure, never an opinion.

## 6. Architecture — 20 modules, about 105 lessons

Stage lines are plain text in `_sidebar.md`. Lesson ids are `NN.M`. Each module ends with a module quiz and a project, `projects/mNN-<slug>.md`.

`(ext)` marks a lesson expected to assign an external free unit. The candidates are in the research files (§11).

### Stage 1 — Foundations

**Module 1 — How Israeli Law Works** — project `m01-issue-map`: map a real issue to its laws, authorities and forum.

- 01.1 What this course can and cannot make you (self-representation, limits, safety)
- 01.2 Where Israeli law comes from (Mandate and Ottoman layers, Foundations of Law Act, Knesset, case law)
- 01.3 The hierarchy: Basic Laws, laws, regulations, directives and procedures (נהלים, הנחיות היועמ"ש)
- 01.4 The map of courts and tribunals
- 01.5 Reading a statute: structure, definitions, legal Hebrew
- 01.6 Reading a ruling: anatomy of a פסק דין

**Module 2 — Legal Research and Writing** — project `m02-research-memo`.

- 02.1 Finding the current text of a law, free (Wikisource, Knesset legislation database)
- 02.2 Finding rulings, free (court search, Versa)
- 02.3 Secondary sources: Kol Zchut, Knesset Research Center, free law journals (ext)
- 02.4 Building an argument (issue, rule, application, conclusion)
- 02.5 Writing a formal letter to an authority (פנייה / דרישה)
- 02.6 Affidavits (תצהיר): structure, who certifies, cost

**Module 3 — Constitutional Law and Basic Laws** — project `m03-proportionality`: proportionality analysis of a real measure.

- 03.1 A constitution built from Basic Laws
- 03.2 Basic Law: Human Dignity and Liberty and the limitation clause
- 03.3 Proportionality step by step
- 03.4 Rights the courts derived: equality, expression, religion, protest
- 03.5 Judicial review and the 2023–2026 constitutional dispute, with all sides presented

### Stage 2 — Public Law Toolbox (the core)

**Module 4 — Administrative Law Principles** — project `m04-decision-audit`: audit a real government decision.

- 04.1 Authority and the principle of legality
- 04.2 Discretion: relevant and extraneous considerations
- 04.3 Reasonableness and proportionality in administrative decisions
- 04.4 Fair procedure: hearing, reasons, conflict of interest
- 04.5 Standing, justiciability, exhausting remedies

**Module 5 — Acting Against the Authorities** — project `m05-foi-to-petition`: an FOI request taken all the way to a petition-ready file.

- 05.1 Choosing the right tool (decision tree)
- 05.2 Freedom of Information request
- 05.3 When FOI fails: reminders, FOI Unit complaint, appeal path
- 05.4 Public Complaints Commissioner and State Comptroller
- 05.5 The pre-petition letter (מיצוי הליכים)
- 05.6 Administrative petition, self-represented
- 05.7 High Court petition (בג"ץ), self-represented

**Module 6 — Protest, Expression and Police** — project `m06-protest-plan`: a legal plan for a real or realistic protest.

- 06.1 Freedom of expression and assembly in Israeli law
- 06.2 Permits: when you need one (Police Ordinance ss. 83–85)
- 06.3 At the protest: police powers, dispersal, filming police
- 06.4 Complaints about police conduct
- 06.5 Social media, signs and incitement limits

**Module 7 — Criminal Law and Procedure for Activists** — project `m07-arrest-kit`.

- 07.1 Offences activists are most often charged with
- 07.2 Detention, arrest and your rights
- 07.3 Interrogation: silence, lawyer, Public Defender
- 07.4 Remand hearings and release conditions
- 07.5 After the case: closed files, criminal and police records

**Module 8 — Defamation, Privacy and Online Speech** — project `m08-publication-check`.

- 08.1 Defamation basics
- 08.2 Defences: truth plus public interest, good faith
- 08.3 Threat letters and SLAPP suits: what to do
- 08.4 Privacy law for activists (photos, data, Amendment 13)
- 08.5 Platforms, takedowns and online harassment

**Module 9 — Equality and Anti-Discrimination** — project `m09-discrimination-file`.

- 09.1 Map of anti-discrimination laws
- 09.2 Discrimination in services and entry: suing without proof of damage
- 09.3 Employment discrimination and the Commission
- 09.4 Disability rights and accessibility complaints
- 09.5 Collecting evidence lawfully (testers, records)

**Module 10 — Planning, Land and Environment** — project `m10-objection`.

- 10.1 The planning system map
- 10.2 Reading a plan on Mavat
- 10.3 Writing an objection
- 10.4 The hearing and the appeal
- 10.5 Environmental laws and complaints

**Module 11 — Civil Litigation on Your Own** — project `m11-small-claim`.

- 11.1 Should you go to court? Cost, risk, alternatives
- 11.2 Small claims court step by step
- 11.3 Net HaMishpat for unrepresented parties
- 11.4 Civil Procedure Regulations 2018: what self-represented people must know
- 11.5 Evidence and the day of the hearing
- 11.6 Fee exemptions and Legal Aid

**Module 12 — The Knesset and Local Government** — project `m12-position-paper`.

- 12.1 How a law is made
- 12.2 Committees and how the public takes part
- 12.3 Writing a position paper (נייר עמדה)
- 12.4 MKs, parliamentary questions and lobbying rules
- 12.5 Your local authority: council meetings, municipal petitions, local FOI

### Stage 3 — International Law and Human Rights

**Module 13 — International Law Foundations** — project `m13-intl-in-israeli-court`.

- 13.1 What international law is (ext)
- 13.2 Treaties (ext)
- 13.3 Customary law (ext)
- 13.4 The International Court of Justice (ext)
- 13.5 International law inside Israeli courts

**Module 14 — The UN Human Rights System** — project `m14-un-communication`.

- 14.1 The core treaties Israel ratified
- 14.2 Treaty bodies and shadow reports
- 14.3 The Universal Periodic Review
- 14.4 Special Procedures: sending a communication
- 14.5 Human Rights Council and commissions of inquiry (ext)

**Module 15 — Law of Armed Conflict and Occupation** — project `m15-incident-analysis`.

- 15.1 IHL basics (ext)
- 15.2 The law of occupation (ext)
- 15.3 The Israeli High Court on the territories
- 15.4 ICJ advisory opinions and Israel's positions
- 15.5 Analysing an incident under IHL, neutrally

**Module 16 — International Criminal Law and Accountability** — project `m16-accountability-map`.

- 16.1 International crimes (ext)
- 16.2 The ICC and Israel
- 16.3 Complementarity and Israeli investigation mechanisms
- 16.4 Universal jurisdiction
- 16.5 Sending information to international bodies

**Module 17 — Documenting Human Rights Violations** — project `m17-documentation-kit`.

- 17.1 Documentation principles
- 17.2 Interviews and informed consent
- 17.3 Open-source and digital evidence: the Berkeley Protocol (ext)
- 17.4 Preserving and archiving evidence
- 17.5 Digital security for activists (ext)

### Stage 4 — Practical Stage (replaces the internship)

**Module 18 — Organising and Working Within the Law** — project `m18-org-plan`.

- 18.1 Acting as a group: informal group vs amuta
- 18.2 Registering an amuta yourself
- 18.3 Running an amuta: proper management, donations, reporting
- 18.4 What non-lawyers may and may not do for others
- 18.5 Using lawyers smartly: clinics, pro bono, Legal Aid

**Module 19 — Practicum** — project `m19-portfolio`: a real-world portfolio of everything filed.

- 19.1 Court observation: 10 hearings
- 19.2 Real FOI campaign
- 19.3 Real complaint to an oversight body
- 19.4 Knesset or local council participation
- 19.5 Clinic or NGO placement (3+ months)
- 19.6 A real international submission

**Module 20 — Capstone Campaign** — project `m20-capstone`.

- 20.1 Choosing a cause and a theory of change
- 20.2 The legal strategy map
- 20.3 Execution log
- 20.4 Media and public communication within the law
- 20.5 Retrospective and handing over

### Paths

| Path | Modules | Estimate |
|---|---|---|
| **Fast activist path** | 1, 2, 4, 5, 6, 7, then 19 (19.2–19.4) | ~3–4 months part-time |
| **Full nano degree** | all 20 | ~18–24 months at 6–8 h/week, including the practicum |

## 7. Lesson format (exact, every lesson)

```markdown
---
id: "05.2"
module: 5
minutes: 12
practice_minutes: 60
prerequisites: ["05.1"]
objectives:
  - "Write and file a Freedom of Information request to the right officer."
  - "Calculate the fee and identify when you are exempt."
volatility: implementation
sources:
  - title: "חוק חופש המידע, התשנ״ח-1998"
    url: https://…
last_verified: "2026-10-.."
---

# 05.2 · Freedom of Information request

One plain intro paragraph: what the learner will do by the end.

## Why it matters
## Key terms
## The law
## How it works in practice
## Worked example
## Do it yourself
## Learn more
## What goes wrong
## Review
```

- **Exactly these 9 `##` sections**, in this order. Use `###` inside them.
- **Key terms**: a table `| עברית | Transliteration | English |`, 3–10 terms.
- **The law**: the exact Hebrew sections quoted in blockquotes, each followed by a one-line English gist and a link to the free full text. For international lessons, quote the treaty article in English.
- **How it works in practice**: who, where, which form, how long it takes, what it costs. Current numbers are *not* written here; link `../../references/current-numbers.md` instead (§9).
- **Worked example**: a realistic case, solved step by step. Rotate causes across the spectrum (§5).
- **Do it yourself** has these subsections:
  - `### You need`
  - `### Steps` (numbered)
  - `### Template` (link to `templates/`)
  - `### How you know it worked`
  - `### Self-check` (a task list)

  Levels: *practice* (a fictional or own-name dry run) by default. *Real* (actually filing) only in Stage 2 projects and the practicum. Every real action opens with `> [!IMPORTANT]` saying "own name only, not legal advice, check current rules".
- **Learn more**: the assigned external unit(s) per §4, with tag, minutes, deep link and fallback. "None" is allowed.
- **What goes wrong**: a table `| Mistake | Consequence | How to fix | How to avoid |`. Rejections for missed deadlines, wrong forum, missing affidavit, unpaid fee and so on.
- **Review**: 3–5 bullets.
- Set `volatility: implementation` for anything with fees, deadlines, forms, procedures, current cases or the status of legislation. Otherwise `concept`.

## 8. Practical design

- **Every lesson** ends in a task: find a law, read a ruling and summarise it, fill a template, draft a letter, plan a protest, or analyse a scenario.
- **Every module** ends in a project in `projects/` with a self-assessment rubric. The Academy cannot grade documents, so the learner compares their work against the rubric and a model answer in `<details>`.
- **Practicum (Module 19)** consists of real actions in the learner's own name. Each lesson gives:
  - eligibility,
  - exact steps,
  - expected timeline,
  - what to record in the portfolio,
  - how to stay safe and lawful.
- **Safety**: arrest, police, digital security and documentation lessons open with `> [!WARNING]`. Real documentation work in conflict zones is explicitly out of scope; we teach remote and open-source work.

## 9. Shared reference pages (main session only)

These are linked from the top of `_sidebar.md`:

- `references/current-numbers.md` — every fee, ceiling and deadline (FOI fees, small-claims ceiling, court fees, objection periods, petition deadlines), each with source and date checked. Lessons link here instead of repeating numbers. **One place to update each October.**
- `references/external-resources.md` — the catalog from §4.
- `references/where-to-get-help.md` — clinics, Legal Aid, the Public Defender, NGOs across the spectrum.
- `references/laws-index.md` — every law and ruling the course cites, with free full-text links.
- `glossary.md` — Hebrew, transliteration and English for every term.
- `templates/` — Hebrew filing templates:
  - FOI request
  - FOI Unit complaint
  - Ombudsman complaint
  - pre-petition letter
  - administrative petition skeleton
  - HCJ petition skeleton
  - small-claims statement
  - planning objection
  - affidavit
  - Knesset position paper
  - police complaint
  - discrimination demand letter
  - English templates for the UN Special Procedures communication and the shadow report outline

## 10. Quizzes

Follow the guidelines §5 exactly. Questions are realistic decisions, for example:

- "Your FOI request got no answer after 45 days — what now?"
- "Which forum hears a petition against a municipality's planning decision?"

Wrong options are real mistakes people make, such as the wrong court, a missed deadline, or no exhaustion of remedies.

## 11. Research (pre-built source lists)

All in `curriculum/research/` (not imported):

| File | Content | Status |
|---|---|---|
| `activist-law.md` | first overview of options | done |
| `activist-law-practical.md` | practical procedures (FOI, ombudsman, objections, UN) | done |
| `activist-law-curriculum.md` | first LL.B.-style curriculum draft | done, superseded by §6 |
| `sources-israel.md` | verified sources for Israeli modules M01–M12, M18–M19, Hebrew video; 2026 numbers table | done 2026-10-12 |
| `sources-international.md` | verified sources for M13–M17 + free course catalog (Coursera dropped free audit in 2025: Leiden / Case Western excluded; UN AVL, ICRC, OpenLearn FREE-FULL; edX FREE-AUDIT) | done 2026-10-12 |

Writers take sources from these files first. Anything new must be opened (WebFetch) before it is cited. Items marked ⚠️ must be verified before use.

## 12. Build process (for spawned agents)

**Phase A — foundations (main session):**

- `README.md`, `_sidebar.md`, `glossary.md`
- `references/*` (§9), `templates/*`
- `curriculum/architecture.md` (the §6 inventory with competencies and the practice for each lesson)
- `curriculum/build-spec.md` (this plan's §3, §4, §7 and §8 condensed for module writers)
- `.gitignore`
- the first commit and push

**Phase B — modules**, two agents at a time, one module each, in this order:

1. 01, 02
2. 04, 05
3. 03, 06
4. 07, 08
5. 09, 10
6. 11, 12
7. 13, 14
8. 15, 16
9. 17, 18
10. 19, 20

Module 19 is written last, because it references everything else.

**Each module agent:**

1. Reads, in order:
   - the guidelines
   - this plan
   - `build-spec.md`
   - `architecture.md`
   - its module's sections in the research files
   - one finished module, if one exists
2. Writes for every lesson: the lesson `.md` and its `.quiz.yaml`.
3. Writes the module quiz, the `.md` and the `.quiz.yaml`.
4. Writes the project brief.
5. Writes `curriculum/glossary-inbox/module-NN.md`.
6. Writes `curriculum/inbox/module-NN-numbers.md`, with new fees and deadlines for `current-numbers.md`.
7. Writes `curriculum/inbox/module-NN-external.md`, with new external resources for the catalog.
8. Appends `lesson-MM done` to `curriculum/status/module-NN.log` after each lesson, then `module done`.
9. Never edits shared files and never commits.
10. Never spawns sub-agents.

**Main session, after each module:**

- merges the inboxes
- updates `_sidebar.md`
- runs `check-course`
- commits and pushes
- updates `BUILD_PROGRESS.md`

**Phase C — QA:**

- re-open every external link
- check every number against `current-numbers.md`
- run the neutrality review (§5)
- run `check-course` until it reports `0 problems`
- write `TODO_FOR_TAL.md`: ready to import, repo and commit

## 13. Course details

See `curriculum/course-details.md`:

- slug `activist-law`
- repo `tal-giladi/activist-law-course`
- free
- risk notice about legal risk (arrest, defamation suits, costs orders) and "not legal advice"

## 14. Open questions for Tal

1. Repo: public (Tal, 2026-10-12).
2. Title: "Activist Law: A Free Practical Course" (Tal, 2026-10-12). Never "degree" or "nano degree".
3. Certificate wording: approved as in course-details.md (Tal, 2026-10-12).
4. Lesson 18.4 published without lawyer review, with a not-legal-advice notice (Tal, 2026-10-12).
5. **Hebrew-only Academy translation later.** Prose is English. If Hebrew translation is switched on, the Hebrew quotes stay as they are.
