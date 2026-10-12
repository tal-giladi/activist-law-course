---
id: "17.1"
module: 17
minutes: 20
practice_minutes: 45
prerequisites: ["09.5", "08.4", "15.5"]
objectives:
  - "Decide what a documentation effort is for (advocacy, a complaint, litigation, the historical record) and what standard of care each purpose needs."
  - "Record an incident in an incident log that separates what was seen, by whom, when and where, from analysis and opinion."
  - "Apply the Berkeley Protocol's professional, methodological and ethical principles, including do no harm and data minimisation, to a documentation plan."
  - "Spot the Israeli privacy limits that apply to collecting and publishing information about victims, witnesses and suspects."
volatility: concept
sources:
  - title: "Berkeley Protocol on Digital Open Source Investigations (OHCHR and UC Berkeley Human Rights Center, HR/PUB/20/2, 2022), ch. II Principles (PDF)"
    url: https://www.ohchr.org/sites/default/files/2024-01/OHCHR_BerkeleyProtocol.pdf
  - title: "UC Berkeley Human Rights Center — Berkeley Protocol project page"
    url: https://humanrights.berkeley.edu/programs-projects/tech-human-rights-program/berkeley-protocol-digital-open-source-investigations
  - title: "חוק הגנת הפרטיות, התשמ״א–1981 — ss. 2, 2א, 18 (Hebrew Wikisource)"
    url: https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות
  - title: "The Civil Commission on October 7th Crimes by Hamas against Women and Children — About"
    url: https://www.civilc.org/about
  - title: "NBC News — report by the Dinah Project, 'A Quest for Justice' (8 July 2025, corrected 22 July 2025)"
    url: https://www.nbcnews.com/world/israel/hamas-israel-sexual-violence-rape-war-oct-7-rcna217401
  - title: "Yesh Din — Data sheet: law enforcement on Israeli civilians in the West Bank (settler violence) 2005–2025"
    url: https://www.yesh-din.org/en/data-sheet-law-enforcement-on-israeli-civilians-in-the-west-bank-settler-violence-2005-2025/
last_verified: "2026-10-13"
---

# 17.1 · Documentation Principles

Documentation turns what happened to people into a record that others can check, rely on and act on: a complaint, a petition, a UN submission, a news story or a history. In this lesson you learn the principles that make a record trustworthy and safe — a clear purpose, first-hand detail, accuracy, separation of fact from opinion, do no harm and data minimisation — and you open an incident log for three incidents from different parts of the political map.

> [!WARNING]
> This module teaches remote and open-source documentation, and interviews with people who are safe and willing to talk. It does **not** teach fieldwork in conflict zones, at checkpoints, inside closed military zones or during violent events. Never put yourself or anyone else at risk to get a picture or a testimony, never pressure a victim to talk, and never collect information by hacking, deception or secret recording of conversations you are not part of (lesson [09.5](../module-09/lesson-05.md)). Documentation about real people can expose you to privacy and defamation claims (lessons [08.1](../module-08/lesson-01.md) and [08.4](../module-08/lesson-04.md)). This lesson is not legal advice.

## Why it matters

Every legal tool in this course runs on facts. A police complaint (06.4), a demand letter (09.2), a petition (05.7), a Special Procedures communication (14.4) and a submission to an international body (16.5) all ask the same questions: what happened, to whom, when, where, who did it, and how do you know. Documentation done well answers them in a way a sceptical reader — a judge, a ministry lawyer, a UN officer, a journalist from the other side — can test. Documentation done badly is worse than none: an exaggerated number, a misdated video or a testimony given under pressure lets the other side dismiss everything else you say, and can hurt the very people you meant to help.

The same discipline serves every cause. Israeli civil groups documented the atrocities of 7 October 2023 for prosecutors and historians; Israeli and Palestinian groups document settler violence and law-enforcement follow-up in the West Bank; protesters from opposite camps have documented police violence at their demonstrations; disability and anti-discrimination groups document refusals and barriers. The methods below do not change with the cause.

## Key terms

| עברית | Transliteration | English |
|---|---|---|
| תיעוד | ti'ud | Documentation: creating a reliable record of events |
| יומן אירועים | yoman eru'im | Incident log |
| עדות | edut | Testimony |
| עד ראייה | ed re'iya | Eyewitness |
| עדות שמיעה | edut shmi'a | Hearsay: what someone heard from another person |
| אימות | imut | Verification |
| מקור ראשוני | makor rishoni | Primary (first-hand) source |
| מזעור מידע | mizur meida | Data minimisation: collecting only what you need |
| לא להזיק | lo lehazik | Do no harm |
| הסכמה מדעת | haskama mida'at | Informed consent |

## The law

There is no Israeli "documentation law". The limits come from privacy, wiretap and computer law (lessons 09.5, 17.3 and 17.5), defamation (08.1) and criminal law. The international standard of practice is set by the Berkeley Protocol.

> Relevant methodological principles include, at a minimum, accuracy, data minimization, data preservation and security by design.

*Gist:* every documentation effort must be accurate, collect only what it needs, preserve what it collects and build security in from the start. ([Berkeley Protocol, ch. II, summary](https://www.ohchr.org/sites/default/files/2024-01/OHCHR_BerkeleyProtocol.pdf))

> These include, at a minimum, protecting the dignity of all individuals who participate in or are implicated in an investigation, as well ensuring humility, inclusivity, independence and transparency.

*Gist:* the ethical principles protect the dignity of everyone involved — victims, witnesses and suspects — and require humility about your limits, inclusivity, independence and openness about methods. (Berkeley Protocol, ch. II)

> (1) בילוש או התחקות אחרי אדם, העלולים להטרידו, או הטרדה אחרת;
> (9) שימוש בידיעה על עניניו הפרטיים של אדם או מסירתה לאחר, שלא למטרה שלשמה נמסרה;

*Gist:* following or tracking a person in a way that may harass them is an invasion of privacy, and so is using or passing on a person's private information for a purpose other than the one it was given for — so a testimony given "for the police complaint" may not be posted online without new consent. ([Protection of Privacy Law, s. 2](https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות#סעיף_2))

> (4א) פרסום תצלומו של נפגע ברבים שצולם בזמן הפגיעה או סמוך לאחריה באופן שניתן לזהותו ובנסיבות שבהן עלול הפרסום להביאו במבוכה ...

*Gist:* publishing an identifiable photo of an injured person taken during or just after the injury, in circumstances that may embarrass them, is an invasion of privacy; s. 2א adds a separate rule against publishing an identifiable photo of a body without the family's consent. ([s. 2(4א)](https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות#סעיף_2), [s. 2א](https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות#סעיף_2א))

> (3) בפגיעה היה ענין ציבורי המצדיק אותה בנסיבות הענין, ובלבד שאם היתה הפגיעה בדרך של פרסום – הפרסום לא היה כוזב.

*Gist:* a public-interest defence exists, but only if what you published is true — another reason accuracy is a legal duty, not only good practice. ([s. 18(3)](https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות#סעיף_18))

## How it works in practice

### Start with the purpose

Decide first what the record is for. The purpose sets how careful you must be and who may see the material.

| Purpose | Who will test it | What it needs |
|---|---|---|
| Public advocacy (a post, a report) | Journalists, opponents, platforms | Accurate facts, consent to publish, no identifying details you do not need |
| A complaint (police, Police Investigation Department, ombudsman, a ministry) | An official investigator | Dates, places, names of officers or bodies, witnesses' contact details, originals kept |
| Litigation (a claim, a petition, an affidavit) | A judge and the other side's lawyer | Originals, chain of custody (17.4), witnesses willing to testify, affidavits (02.6) |
| An international body (UN, ICC) | A UN or court officer | Sourced facts, consent to disclosure (14.4), security (17.5) |
| The historical record (an archive) | Historians, future prosecutors | Complete, preserved, well-described material; strict access control |

One record can serve several purposes, but write down which ones at the start: it decides what consent you ask for (17.2).

### The five questions of every entry

Each incident in your log answers, as precisely as the evidence allows:

1. **What** happened — acts, not labels. "An officer struck a seated protester twice on the back with a baton", not "police brutality".
2. **Who** — victims, people who acted, witnesses; with roles, units or vehicle numbers if known.
3. **When** — date and time, and how you know it (a phone timestamp, a news alert, a witness's estimate).
4. **Where** — address or coordinates, and how you know it.
5. **How do we know** — the source of each fact: first-hand witness, video, document, official data, hearsay.

### Fact, source, analysis — in separate columns

The most common mistake is mixing what was seen with what it means. Keep three layers apart:

- **Fact:** what a source says or shows. "Witness A says she saw two men in civilian clothes set fire to a car at 23:10."
- **Source assessment:** how reliable it is. "First-hand; she knows the area; account given the next morning; consistent with a video uploaded at 23:40."
- **Analysis:** what it may mean in law. "If confirmed, arson (Penal Law); a complaint to the police; the question of law-enforcement follow-up."

Analysis belongs to a later stage (15.5 for IHL, 16.1 for international crimes). In the log, the facts come first and must stand on their own.

### Accuracy and humility

- Prefer first-hand sources. Record hearsay as hearsay.
- Corroborate: two independent sources are better than one source repeated by many.
- Use ranges and say what you do not know. "Between 30 and 50 people", "time not confirmed".
- Correct errors openly. The Berkeley Protocol asks investigators to take responsibility for errors and issue corrections.
- Never add to a testimony, never "tidy up" a video, never round numbers up.

### Do no harm and data minimisation

- Before you collect anything, ask: could this record put someone at risk if it leaks, is seized or is published? Victims, witnesses, the documenter, and even suspects (who keep their rights and their presumption of innocence).
- Collect only what the purpose needs. If a home address adds nothing, do not record it. If a face is not needed, do not keep the close-up.
- Use codes instead of names in working files ("Witness W-03"); keep the key separately and securely (17.4, 17.5).
- Material about health, sexual violence, children or political views is especially sensitive (08.4).
- Do not ask victims to tell their story again and again; coordinate with others who have already documented it (17.2).

### Neutrality and independence

- Describe acts in neutral language. Avoid words that decide the legal question ("massacre", "pogrom", "terrorist", "lynch", "war crime") in the fact columns; if a source uses them, quote the source.
- Record the other side's account, and official responses, when you have them.
- Say who funds and runs the documentation effort. Independence is easier to show when methods and funding are open.

### Know who already documents

You rarely need to start from zero. Examples of documentation work by Israeli civil groups, described here as each group describes itself:

- **The Civil Commission on October 7th Crimes by Hamas against Women and Children** gathers testimonies and keeps an archive for the victims' memory and for future research and prosecution, under its own code of ethics. The **Dinah Project** (Ruth Halperin-Kaddari, Nava Ben-Or, Sharon Zagagi-Pinhas) published "A Quest for Justice" in July 2025, based on hostages' and witnesses' accounts, first responders, forensic and visual material. Its finding that sexual violence was systematic is disputed by the UN Special Rapporteur on violence against women; note both positions when you cite it.
- **Yesh Din** collects testimonies from Palestinians about violence by Israeli civilians in the West Bank and tracks what happens to the investigation files; its data sheet reports conviction and complaint rates.
- Protesters from different camps — opponents of the judicial overhaul, Haredi anti-draft demonstrators, settlers evacuated from outposts — have filmed and logged police conduct for complaints to the Police Investigation Department (06.4).

If a group already works on your issue, ask whether to send material to them instead of building a parallel file. Duplicate interviews hurt victims.

## Worked example

**Situation.** Shira Ben-Ami, a volunteer in a Jerusalem residents' group, receives three things in one evening: a WhatsApp message from a friend saying "the police beat protesters at the Chords Bridge"; a 40-second video forwarded many times; and a voice note from a protester, Avi, who says he was hit and hurt his arm.

1. **Purpose.** The group wants to support Avi's complaint to the Police Investigation Department and, later, a short public report. Two purposes: a complaint (high care) and advocacy (consent to publish).
2. **Log entry 1 — Avi's account.** Fact: "Avi (W-01) says an officer pushed him to the ground at about 21:15 near the bridge and struck his arm with a baton." Source: first-hand, voice note received 22:02. Doubts: time estimated; officer not identified.
3. **Log entry 2 — the video.** Fact: "Video shows an officer with a baton striking a person lying on the ground; no time visible." Source: forwarded, original uploader unknown. Doubts: date and place not verified — it may be from another protest. Next step: find the original upload and verify it (17.3).
4. **Log entry 3 — the WhatsApp message.** Recorded as hearsay. Not used as evidence on its own.
5. **Minimisation.** Shira does not record Avi's home address or medical details beyond "arm injury, treated at a clinic, medical document exists". The full name goes in the separate key, not in the shared log.
6. **Next steps.** Ask Avi for a short interview with consent (17.2); preserve the voice note and the video with hashes (17.4); help Avi file the complaint himself (06.4).

**Mirror test.** The same log fits a Haredi demonstrator hit at a draft protest on Route 4, an Arab citizen hurt at a protest in Umm al-Fahm, or a settler youth injured during an outpost evacuation. The five questions and the separation of fact from analysis do not change.

## Do it yourself

### You need

- The template [incident-log.md](../../templates/incident-log.md).
- Three public news reports or official statements about three different incidents from the last year, chosen from different parts of the political map (for example: an attack on Israeli civilians, an incident of settler violence, police conduct at a protest, a discrimination case).
- 45 minutes.

### Steps

1. Write the purpose of your (practice) log in one sentence, and who would use it.
2. For each incident, fill one row of the incident log: what, who (by role, not name, unless the person is a public official acting in role), when, where, and the source of each fact.
3. Mark each fact as first-hand, documentary (video, document) or hearsay.
4. Move every evaluative word ("brutal", "terror", "pogrom", "provocation") out of the fact column; if it matters, put it in quotation marks with the source.
5. In the "doubts" column, write at least one thing you could not confirm for each incident.
6. In the "harm check" column, write what you deliberately did *not* record and why.
7. Re-read the three rows and check that a reader from the other side of each incident would accept the fact column as fair, even if they reject your analysis.

### Template

- [incident-log.md](../../templates/incident-log.md) — bilingual incident log (Hebrew field names with English instructions), with fact, source, doubts and harm-check columns.

### How you know it worked

- Every fact in your log has a source next to it.
- No evaluative or legal label appears in the fact column.
- Each row says what is still unconfirmed.
- You can say, for each row, what you chose not to record.

### Self-check

- [ ] I wrote the purpose of the record before collecting anything.
- [ ] I can tell first-hand evidence from hearsay.
- [ ] I keep facts, source assessment and analysis in separate columns.
- [ ] I collect only what the purpose needs and use codes instead of names.
- [ ] I know a testimony given for one purpose cannot be published for another without consent (Privacy Law s. 2(9)).

## Learn more

- **Berkeley Protocol, chapter II "Principles" (pp. 9–15)** — FREE-FULL, English, no signup, about 30 minutes: <https://www.ohchr.org/sites/default/files/2024-01/OHCHR_BerkeleyProtocol.pdf>. Read the professional, methodological and ethical principles; notice how often "dignity" and "data minimization" come back. *Fallback:* the [UC Berkeley Human Rights Center project page](https://humanrights.berkeley.edu/programs-projects/tech-human-rights-program/berkeley-protocol-digital-open-source-investigations) (5 minutes) and the summary in this lesson.
- **WITNESS — Video as Evidence Field Guide, "All About Evidence"** — FREE-FULL, English (also Arabic, Russian, Ukrainian), no signup, about 30 minutes: <https://library.witness.org/product/video-as-evidence-all-about-evidence/>. Watch for: what makes material evidence rather than advocacy. *Fallback:* the field guide's landing page <https://vae.witness.org/video-as-evidence-field-guide/>.

## What goes wrong

| Mistake | Consequence | How to fix | How to avoid |
|---|---|---|---|
| Starting to collect with no stated purpose | Wrong consent; material cannot be used where needed | Go back to sources and ask for the missing consent | Write the purpose first |
| Labels in the fact column ("massacre", "pogrom") | The record looks partisan and is dismissed | Rewrite as acts; quote labels with their source | Describe acts, not conclusions |
| Treating a viral video as first-hand evidence | Misdated or relocated footage discredits the file | Verify before use (17.3); mark it unverified | Log the source and doubts for every item |
| Rounding numbers up or filling gaps | One error undermines everything else | Publish a correction | Use ranges; write "unknown" |
| Recording addresses, health details and names in a shared sheet | Leak endangers people; privacy breach | Remove them; move names to a separate key | Data minimisation and codes from day one |
| Interviewing a victim already interviewed by others | Re-traumatisation; inconsistent accounts | Stop; coordinate with the first group | Ask who has already documented the case |

## Review

- Decide the purpose first: advocacy, complaint, litigation, international body or archive; each needs a different standard of care and consent.
- Every entry answers what, who, when, where and how we know; facts, source assessment and analysis stay in separate columns.
- Accuracy, humility, corroboration and open corrections are what make a record believable to the other side.
- Do no harm and data minimisation: collect only what you need, use codes, protect sensitive material; information given for one purpose may not be used for another without consent (Privacy Law s. 2(9)).
- Describe acts in neutral language and check who already documents the issue before you start.
