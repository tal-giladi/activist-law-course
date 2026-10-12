---
id: "09.5"
module: 9
minutes: 20
practice_minutes: 45
prerequisites: ["09.2", "08.4", "06.3"]
objectives:
  - "Decide whether a planned recording is lawful under the Wiretap Law: your own conversation, yes; a conversation you are not part of, no."
  - "Design a tester check that produces the comparison the s. 6 presumptions need, without deception that harms the case."
  - "Keep an evidence log that records what, when, who and how each item was collected and stored."
  - "Spot evidence that a court may exclude under the Protection of Privacy Law s. 32 or the Wiretap Law s. 13."
volatility: concept
sources:
  - title: "חוק האזנת סתר, התשל״ט–1979 — ss. 1, 2, 13 (Hebrew Wikisource)"
    url: https://he.wikisource.org/wiki/חוק_האזנת_סתר
  - title: "חוק הגנת הפרטיות, התשמ״א–1981 — ss. 2, 32 (Hebrew Wikisource)"
    url: https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות
  - title: "חוק איסור הפליה במוצרים, בשירותים ובכניסה למקומות בידור ולמקומות ציבוריים, התשס״א–2000 — s. 6 (Hebrew Wikisource)"
    url: https://he.wikisource.org/wiki/חוק_איסור_הפליה_במוצרים,_בשירותים_ובכניסה_למקומות_בידור_ולמקומות_ציבוריים
  - title: "Kol Zchut — ruling summary, Nazareth Magistrates' Court, תא 30239-04-17 (12.6.2018): friends returned to the door to check"
    url: https://www.kolzchut.org.il/he/פיצוי_בסך_71,000_ש%22ח_לבליינים_שכניסתם_למועדון_נמנעה_בשל_היותם_ערבים
  - title: "Kol Zchut — ruling summary, Tel Aviv Magistrates' Court, 2320-04-19 (29.10.2020): passenger recorded her own conversation with the driver (updated 19.8.2026)"
    url: https://www.kolzchut.org.il/he/פיצוי_בסך_120,000_ש%22ח_על_סירוב_להעלות_נוסעת_לאוטובוס_בגלל_לבושה
last_verified: "2026-10-13"
---

# 09.5 · Collecting Evidence Lawfully

Discrimination cases are won on evidence collected in the first hours: a recording of your own conversation, a friend who was let in a minute later, a screenshot of an advertisement, a note written that night. In this lesson you learn what you may record and photograph, how testers work, which evidence a court may throw out, and how to keep an evidence log — and you plan a lawful tester check.

> [!WARNING]
> Secretly recording a conversation you are not part of is a criminal offence (Wiretap Law s. 2, up to five years' imprisonment), and the recording is usually inadmissible. Never leave a phone recording in a room you have left, never plant a device, and never use someone else's account to read messages. Publishing what you collected can also expose you to defamation or privacy claims (lessons [08.1](../module-08/lesson-01.md) and [08.4](../module-08/lesson-04.md)). This lesson is not legal advice.

## Why it matters

The presumptions in the services law (s. 6) and the burden shift in the employment law (s. 9) are powerful, but they still need facts: that others were served, that you were asked about your origin, that a condition applied only to you. Those facts disappear quickly. Security footage is overwritten within days, witnesses forget times, messages are deleted. On the other hand, evidence collected unlawfully can be excluded and can turn the claimant into a defendant. Knowing the line lets you collect more, not less.

## Key terms

| עברית | Transliteration | English |
|---|---|---|
| האזנת סתר | ha'azanat seter | Wiretapping: listening to or recording a conversation without the consent of any party |
| בעל שיחה | ba'al sicha | A party to the conversation (s. 1) |
| בודק / בודקת | bodek / bodeket | Tester: a person sent to check whether a business treats groups differently |
| קבוצת השוואה | kvutzat hashva'a | Comparison group |
| ראיה פסולה | re'aya psula | Inadmissible evidence |
| יומן ראיות | yoman re'ayot | Evidence log |
| רשות היחיד | reshut hayachid | Private domain (photographing a person there is a privacy infringement, s. 2(3)) |
| צילום מסך | tzilum masach | Screenshot |

## The law

> ”האזנת סתר“ – האזנה ללא הסכמה של אף אחד מבעלי השיחה;

*Gist:* wiretapping means listening without the consent of *any* party; if you are a party to the conversation, your own consent is enough, so recording your own conversation is not wiretapping. ([Wiretap Law, s. 1](https://he.wikisource.org/wiki/חוק_האזנת_סתר#סעיף_1))

> המאזין האזנת סתר שלא על פי היתר כדין, דינו – מאסר חמש שנים.

*Gist:* wiretapping without a lawful permit carries up to five years; using or disclosing its content is a separate offence (s. 2(ב)). ([s. 2(א)](https://he.wikisource.org/wiki/חוק_האזנת_סתר#סעיף_2))

> דברים שנקלטו בדרך של האזנת סתר בניגוד להוראות חוק זה … לא יהיו קבילים כראיה בבית משפט …

*Gist:* an unlawful wiretap is inadmissible, with narrow criminal-law exceptions. ([s. 13(א)](https://he.wikisource.org/wiki/חוק_האזנת_סתר#סעיף_13))

> חומר שהושג תוך פגיעה בפרטיות יהיה פסול לשמש ראיה בבית משפט, ללא הסכמת הנפגע, זולת אם בית המשפט התיר מטעמים שיירשמו להשתמש בחומר …

*Gist:* material obtained by infringing privacy is inadmissible without the person's consent, unless the court allows it for recorded reasons or the collector has a defence under the Privacy Law. ([Protection of Privacy Law, s. 32](https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות#סעיף_32))

> (3) צילום אדם כשהוא ברשות היחיד;

*Gist:* photographing a person while he is in a private domain is one of the listed privacy infringements; others include stalking, wiretapping and publishing a photo in humiliating circumstances. ([Privacy Law, s. 2](https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות#סעיף_2))

## How it works in practice

### Recording

| Situation | Lawful? | Why |
|---|---|---|
| You record your own phone call with the hotel clerk | Yes | You are a party (s. 1) |
| You record your conversation with the bouncer at the door | Yes | You are a party |
| Your friend, standing next to you and part of the conversation, records it | Yes | A party consented |
| You leave your phone recording on the table and walk away | No | You are no longer a party: wiretapping |
| You record two staff members talking to each other | No | Neither consented |
| You record a job interview you are attending | Yes, under the Wiretap Law | You are a party; some employers' rules forbid it, so weigh the relationship |

A recording of your own conversation is generally admissible, but the court decides how much weight it carries. Keep the original file, do not edit it, and note the device and time.

### Photographing and filming

- From a public place (the street, the queue outside a club, a shop's public floor), filming the scene and the sign at the door is generally lawful.
- Do not photograph people inside private areas (offices, changing rooms, homes) — that is s. 2(3).
- Photograph barriers, signs, menus, notices and the time (a clock, a newspaper, the phone screen).
- Publishing faces of staff or other customers is a separate decision: check lessons 08.1 and 08.4 first, and blur what you do not need.

### Testers

A tester is a person who asks for the same product or service in the same circumstances, to see whether a group is treated differently. In the Nazareth club case, the plaintiffs' Jewish friends went back to the door minutes after the refusal and were let in without any check of the "invitation list"; the court relied on that to find discrimination (Kol Zchut summary, 2018). Testers produce exactly the s. 6(2) and 6(4) comparisons.

Rules for a tester check that holds up:

1. **Same request, same circumstances.** Same time window, same group size, similar dress and age, the same words. The only difference should be the ground you are testing.
2. **Real request.** The tester asks for something the business actually offers. Do not stage a provocation.
3. **No lies about the facts that matter.** A tester may simply not mention why they came; they should not invent documents or identities.
4. **Record only your own conversations.** Each tester may record their own exchange.
5. **Write it down immediately.** Each tester writes a short signed statement the same day: time, place, words, outcome.
6. **Repeat if possible.** Two or three checks on different days answer "it was a one-off" or "we were full that night".
7. **Testers are witnesses.** They must be ready to come to court.

For job applications, matched CVs (identical qualifications, different name or address) work the same way; send them close together and keep the replies.

### Other evidence

- **Screenshots** of advertisements, messages, booking pages and reviews, with the URL and date visible. A discriminatory advertisement is itself a wrong (services law s. 4).
- **Ask the business in writing to preserve CCTV** for the relevant times, the same day or the next morning.
- **Your notes**, written the same day, are evidence of what you remember; write facts, not conclusions.
- **Comparison data**: who else was served, hired or promoted; for employment, the Commission can order data from the employer (s. 18יא).
- **Chain of custody**: keep originals, copy them to a second place, and record in the log who handled each file.

### The evidence log

Keep one table for the whole case: item number, date and time collected, who collected it, how (own recording, screenshot, photo, statement), where the original is stored, what it proves (which element or presumption), and any doubts about it. The template [discrimination-evidence-log.md](../../templates/discrimination-evidence-log.md) gives a ready layout.

## Worked example

**Situation.** Eyal and Dor, a gay couple from Jerusalem, phone a wedding-events garden near Beit Shemesh to book a date. The owner asks, "And who's the bride?" When they explain, he says, "We're fully booked for the next two years." Eyal recorded the call on his phone.

1. **Recording.** Eyal is a party to the call: lawful (s. 1). He saves the original file, its date and length, and a second copy in the cloud. He does not edit it.
2. **Presumption s. 6(1).** The owner asked about a detail related to a ground (sexual orientation) and then refused.
3. **Tester.** The next day their friends Ofir and Maya, a man and a woman, call from their own phone asking for the same dates and the same number of guests. They are offered three dates and a price list by WhatsApp. Ofir records his own call and saves the messages. That supports s. 6(2).
4. **Advertisement.** The garden's website says "dates available this year". Screenshot with URL and date.
5. **Statements.** Eyal, Dor, Ofir and Maya each write a dated, signed paragraph that evening.
6. **Log.** Eight items in the evidence log, each with what it proves. Their demand letter (lesson 09.2) lists them as attachments; the recording is offered as an audio file with a transcript.
7. **Publication.** They want to post about it. They decide to wait until after the demand letter, to post only facts that the recordings prove, and to blur the owner's voice details — after reading 08.1 and 08.2.

## Do it yourself

### You need

- A pen-and-paper plan; no real test is required.
- The template [discrimination-evidence-log.md](../../templates/discrimination-evidence-log.md).
- 45 minutes.

Fictional report: a post in a soldiers' WhatsApp group says a bar in Haifa refuses entry to soldiers in uniform "because the owner doesn't want politics in the bar". Two soldiers say they were refused last Thursday at 22:00 while others in civilian clothes went in.

### Steps

1. Name the ground and section (services law, s. 3(א): wearing the uniform of the security and rescue forces).
2. Write the comparison you need for s. 6(2) and how a tester check would produce it.
3. Plan the check: who, when, what they wear, what they ask, what each one records (own conversations only), and who writes statements.
4. List what you will *not* do, with the reason (for example: no recording of staff talking among themselves; no photos inside the private office; no posting faces).
5. Draft a one-paragraph email asking the bar to preserve its entrance CCTV for last Thursday 21:30–22:30.
6. Fill the first five rows of the evidence log for the two soldiers' account and your planned items.

### Template

- [discrimination-evidence-log.md](../../templates/discrimination-evidence-log.md) — evidence log, tester plan and witness statement skeleton.

### How you know it worked

- Your tester plan changes only one variable (the uniform) and keeps the time, group size and request the same.
- Every recording in your plan is of a conversation the recorder takes part in.
- Each log row says which element or presumption the item proves.

### Self-check

- [ ] I can say why recording my own conversation is not wiretapping.
- [ ] I know that leaving a phone recording after I leave the room is an offence.
- [ ] I can design a tester check that changes one variable only.
- [ ] I know s. 32 of the Privacy Law can exclude improperly obtained material.
- [ ] I ask for CCTV to be preserved within a day.

## Learn more

- **Kol Zchut — ruling summary on the bus passenger who recorded the driver** — FREE-FULL, Hebrew, no signup, 5 minutes: <https://www.kolzchut.org.il/he/פיצוי_בסך_120,000_ש%22ח_על_סירוב_להעלות_נוסעת_לאוטובוס_בגלל_לבושה>. Notice how a recording of her own conversation the next day supplied the driver's reason. Fallback: the Worked example and the recording table above.
- **Wiretap Law, ss. 1–2 and 13** — FREE-FULL, Hebrew, 10 minutes: <https://he.wikisource.org/wiki/חוק_האזנת_סתר>. Read the definitions of "שיחה", "בעל שיחה" and "האזנת סתר". Fallback: the quotes in this lesson.

## What goes wrong

| Mistake | Consequence | How to fix | How to avoid |
|---|---|---|---|
| Leaving a phone recording in the manager's office | Criminal exposure; evidence excluded (s. 13) | Delete it; do not use or share it (s. 2(ב)); get legal advice | Record only conversations you take part in |
| Tester dressed and behaving differently from the claimant | Court finds the comparison not "the same circumstances" | Repeat with a matched tester | Change one variable only |
| Editing or trimming the recording | Authenticity challenged | Produce the original file | Keep and copy the original untouched |
| Notes written a week later | Weak evidence | Add what others wrote at the time | Write the same day |
| Posting the video with staff faces before filing | Privacy or defamation claim; settlement harder | Remove or blur; post only proven facts | Publish after 08.1–08.4 checks |
| Not asking for CCTV | Footage overwritten | Ask the court to order disclosure; rely on witnesses | Send a preservation request the next day |

## Review

- You may record a conversation you are a party to; recording a conversation you are not part of is wiretapping, an offence, and inadmissible.
- Material obtained by infringing privacy may be excluded (Privacy Law s. 32); photograph scenes and barriers from public areas.
- Testers supply the comparison the presumptions need; change only the ground being tested and record only your own conversations.
- Keep originals, write statements the same day, request CCTV preservation, and log every item with what it proves.
- Check defamation and privacy before publishing anything you collected.
