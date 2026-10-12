---
id: "17.3"
module: 17
minutes: 25
practice_minutes: 75
prerequisites: ["17.1", "08.4"]
objectives:
  - "Explain what counts as open-source information under the Berkeley Protocol, and why anything obtained by unauthorised access or deception is outside it (and a crime under the Computers Law)."
  - "Collect an online item to the Berkeley Protocol minimum: URL, full-page capture with date and time, source code, embedded media, metadata, contextual data, collection data and a hash."
  - "Verify an item through source analysis, technical analysis and content analysis, and record what remains unverified."
  - "Plan the six phases of an online inquiry, from search to analysis, with security and data minimisation built in."
volatility: implementation
sources:
  - title: "Berkeley Protocol on Digital Open Source Investigations (OHCHR and UC Berkeley Human Rights Center, HR/PUB/20/2, 2022), chs I–VI and Annex IV (PDF)"
    url: https://www.ohchr.org/sites/default/files/2024-01/OHCHR_BerkeleyProtocol.pdf
  - title: "UC Berkeley Human Rights Center — Berkeley Protocol publication page (English 2020; UN languages)"
    url: https://humanrights.berkeley.edu/publications/berkeley-protocol-on-digital-open-source-investigations/
  - title: "חוק המחשבים, התשנ״ה–1995 — ss. 1, 4, 5, 7 (Hebrew Wikisource)"
    url: https://he.wikisource.org/wiki/חוק_המחשבים
  - title: "חוק הגנת הפרטיות, התשמ״א–1981 — s. 2(1), 2(5) (Hebrew Wikisource)"
    url: https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות
  - title: "Bellingcat — Online Open Source Investigation Toolkit"
    url: https://bellingcat.gitbook.io/toolkit
  - title: "WITNESS Library — Video as Evidence: Verifying Eyewitness Video"
    url: https://library.witness.org/product/video-as-evidence-verifying-eyewitness-video/
last_verified: "2026-10-13"
---

# 17.3 · Open-Source and Digital Evidence: the Berkeley Protocol

Much of what happens in Israel and the region is filmed, posted and deleted within hours. Open-source investigation means finding, collecting, preserving and verifying that public material to a standard a court or a UN body can rely on. In this lesson you learn the Berkeley Protocol — the UN standard for this work — and the Israeli legal line you must never cross, and you collect and verify one public online item from start to finish.

> [!WARNING]
> Open-source work uses only information that any member of the public can see, buy or request. Logging into someone else's account, guessing passwords, using leaked credentials, joining closed groups under a false identity to extract information, or scraping data behind a login you were not given can be a crime under the Computers Law (s. 4: up to three years) and an invasion of privacy. Do not track or profile private individuals: following a person in a way that may harass them is an invasion of privacy (Privacy Law s. 2(1)). Viewing violent footage can be distressing; limit exposure, turn off autoplay and sound, and take breaks. This lesson is not legal advice.

## Why it matters

Videos, photos and posts from phones are now central evidence in human-rights reporting and in courts — and central to disinformation. Footage from Syria is reposted as Gaza; footage from the May 2021 riots in mixed cities is reposted as "tonight"; a real video is cut so that what came before disappears. Each side of every conflict accuses the other of fakes. A documenter who can show where and when a video was filmed, who first posted it, and that the copy has not changed since collection, gives everyone a fact to argue from. A documenter who forwards an unverified clip loses credibility for every later claim.

The Berkeley Protocol on Digital Open Source Investigations, published by OHCHR and the UC Berkeley Human Rights Center (English 2020; UN edition HR/PUB/20/2, 2022; available in all six UN languages), sets minimum professional standards for this work. It does not depend on any particular tool; tools change, the principles stay.

## Key terms

| עברית | Transliteration | English |
|---|---|---|
| מידע מקור גלוי | meida makor galuy | Open-source information: publicly available information |
| איסוף | isuf | Collection: capturing an online item |
| שימור | shimur | Preservation |
| אימות | imut | Verification |
| ייחוס מקור | yichus makor | Attribution: finding who first created or posted an item |
| מטא־דאטה | meta-data | Metadata: data about the file (time, device, location, uploader) |
| איתור מיקום | itur mikum | Geolocation: finding where an image was taken |
| ערך גיבוב | erech gibuv | Hash value: a digital fingerprint of a file |
| חדירה לחומר מחשב שלא כדין | chadira lechomer machshev shelo kadin | Unlawful access to computer material (Computers Law s. 4) |
| זהות בדויה | zehut beduya | Virtual (false) identity online |

## The law

> Open source information is information that any member of the public can observe, purchase or request, without requiring special legal status or unauthorized access.

*Gist:* if you need a password you were not given, a special status, or a trick to see it, it is not open-source information. ([Berkeley Protocol, ch. I, para. 1](https://www.ohchr.org/sites/default/files/2024-01/OHCHR_BerkeleyProtocol.pdf))

> Hash values are a unique form of digital identification that confirm, through the use of cryptography, that the content collected is unique and has not been modified since the time of collection.

*Gist:* at the point of collection, add a hash to every item so you can later prove it has not changed; choose the hash by the current accepted standard (today SHA-256 is the common choice; 17.4). (Berkeley Protocol, ch. VI.C, para. 155(h))

> החודר שלא כדין לחומר מחשב הנמצא במחשב, דינו – מאסר שלוש שנים; לענין זה, ”חדירה לחומר מחשב“ – חדירה באמצעות התקשרות או התחברות עם מחשב, או על ידי הפעלתו ...

*Gist:* accessing computer material without permission — by connecting to a computer or operating it — carries up to three years; doing so to commit another offence carries five (s. 5), and the victim can also sue (s. 7). Someone else's phone, cloud account, email or closed group is "computer material". ([Computers Law, s. 4](https://he.wikisource.org/wiki/חוק_המחשבים#סעיף_4))

> (5) העתקת תוכן של מכתב או כתב אחר שלא נועד לפרסום, או שימוש בתכנו, בלי רשות מאת הנמען או הכותב ...

*Gist:* copying or using a private message not meant for publication, without permission of the writer or recipient, is an invasion of privacy — a private WhatsApp chat forwarded to you is not open-source material. ([Privacy Law, s. 2(5)](https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות#סעיף_2); lesson [08.4](../module-08/lesson-04.md))

## How it works in practice

### The six phases of an online inquiry

The Berkeley Protocol describes an investigation cycle. Plan each phase before you start (Protocol ch. V: threat assessment, landscape assessment, investigation plan, resilience and self-care, data policies).

| Phase | What you do | Output |
|---|---|---|
| 1. Online inquiries | Search: keywords in Hebrew, Arabic and English, place names, dates, hashtags, accounts of local news and residents | A list of candidate items |
| 2. Preliminary assessment | Is it relevant to the purpose? Prima facie reliable? Likely to be deleted soon? | Items to collect, in order of urgency |
| 3. Collection | Capture each item with its context and collection data | A collection package per item |
| 4. Preservation | Store originals unchanged, hashed, backed up (17.4) | Preserved originals and working copies |
| 5. Verification | Source, technical and content analysis | A verification note per item |
| 6. Investigative analysis | What the verified items show together; gaps; links to the law (15.5, 16.1) | Findings, with confidence levels |

### Collection: the Berkeley minimum

For each online item, capture as much of this as applies (Protocol para. 155):

1. **Target web address** — the exact URL of the post, not of the feed.
2. **Source code** — the page's HTML (in most browsers: save the page, or "View page source" and save it).
3. **Full-page capture** — a screenshot of the whole page with the date and time visible, or "Print → Save as PDF".
4. **Embedded media** — download the video or image itself, in its original format where possible.
5. **Embedded metadata** — uploader name and ID, post ID, upload date and time, geotag, hashtags, view counts.
6. **Contextual data** — comments, replies, the account's earlier posts about the same event.
7. **Collection data** — who collected it, when (with an accurate clock), with what device and software, and whether any account or virtual identity was used.
8. **Hash value** — of each saved file, at the time of collection (commands in 17.4).

Also save a copy to a public archive such as the Internet Archive's "Save Page Now" (17.4), so that a third party holds an independent copy with its own timestamp. Note: an archive copy is public and permanent — do not archive pages that would expose a private victim.

Record everything in the online-item section of [evidence-chain-of-custody.md](../../templates/evidence-chain-of-custody.md), which follows the Protocol's online data collection form (Annex IV).

### Verification: three lenses

Look at the item through all three lenses and compare them; one lens alone is never enough (Protocol paras 176–187).

**Source analysis — who?**
- Find the earliest upload: search the platform for the same clip, use reverse image search on key frames (several engines; results differ), sort by date.
- Look at the account: how old, where it usually posts from, whether it was at the scene before, who it is linked to, how it is funded or affiliated.
- Was the uploader the person who filmed? If not, try to reach the original source (with care, 17.2).

**Technical analysis — the file itself**
- Check the file's metadata where it survives. Most social platforms strip much embedded metadata on upload, so absence proves nothing.
- Look for signs of editing: cuts, changed frame rates, mismatched audio, compression artefacts around inserted objects, signs of AI generation (inconsistent text, hands, shadows, reflections).

**Content analysis — what does it show?**
- **Where (geolocation):** match buildings, signs, terrain, road markings, antennas, minarets or water towers with satellite imagery and street-level photos.
- **When (chronolocation):** the weather that day, shadows and the sun's angle, the season (vegetation, clothing), events visible in the frame, the first known upload.
- **What:** who is visible, uniforms and insignia, vehicles and plates, weapons, the sequence of events — and what happened just before and after the clip.

Write a short verification note: what you checked, what matched, what did not, and your confidence ("confirmed", "likely", "unverified", "false"). Never upgrade "likely" to "confirmed" because the item fits your cause.

### Ethics and security online

- **No deception to obtain information.** The Protocol notes that some investigators browse with a separate research account for safety, but eliciting information from people under a false identity takes you outside open-source investigation, breaches ethics and may break the law. In this course: do not use false identities at all.
- **Protect yourself.** Use a separate browser profile for research, do not like or comment on what you investigate, and do not let your personal accounts follow sources (17.5).
- **Protect people in the material.** Victims, bystanders and minors appear in footage. Do not republish identifiable images of injured people or bodies (Privacy Law ss. 2(4א), 2א); blur when you must show something; never "dox" anyone, including suspects.
- **Terms of service** of platforms may forbid scraping or fake accounts; breaching them is not always a crime, but it can get your account closed and your evidence questioned.

## Worked example

**Situation.** On a tense evening, a 25-second video spreads in Hebrew WhatsApp groups with the caption "Now in Lod: Arabs attacking a Jewish driver". Ayelet Cohen, a volunteer with a coexistence group in Lod, wants to know whether to warn residents or to warn against the video.

1. **Preliminary assessment.** Relevant and urgent (it may cause violence either way); likely to be deleted or re-edited. Collect first.
2. **Collection.** She cannot collect from a private WhatsApp group as "open source", so she searches public platforms for the same clip and finds a public post with the same video. She records the URL, takes a dated full-page PDF, saves the HTML and downloads the video, notes the account and post time, and hashes the files.
3. **Source analysis.** Reverse image searches on three key frames find the same clip posted publicly in **May 2021**, during the riots in mixed cities, by a local news account.
4. **Content analysis.** The street matches a road in Lod on satellite imagery, but a shop sign visible in the clip was replaced in 2023 according to recent street-level imagery; the trees are bare, while it is now summer.
5. **Conclusion.** "Genuine video from May 2021, misdated. Not evidence of an event tonight." Confidence: high.
6. **Use.** The group posts a neutral correction with the original 2021 source, without sharing the violent clip again and without naming the people who forwarded it.

**Mirror test.** The same steps apply to a clip captioned "settlers burning a village now" that turns out to be from another year, a clip of "police beating Kaplan protesters" filmed at a different protest, or a clip of "IDF soldiers abusing detainees" or "Hamas fighters in a kibbutz" whose date and place must be confirmed before anyone relies on it.

## Do it yourself

### You need

- A computer with a modern browser.
- One public post (video or image) about a public event in Israel from the last two years, on any side of any issue. Avoid graphic content for this exercise.
- The online-item section of [evidence-chain-of-custody.md](../../templates/evidence-chain-of-custody.md).
- A hashing command (17.4; for now: `Get-FileHash` in Windows PowerShell, `shasum -a 256` on macOS, `sha256sum` on Linux).
- 75 minutes.

### Steps

1. Write one sentence on why this item matters and what claim it is said to support.
2. Check your computer's clock is set automatically (network time).
3. Collect the item: URL; full-page PDF or screenshot with date and time; saved HTML; the media file itself; uploader, post ID and time; relevant comments.
4. Hash every saved file and record the hashes and the time in the form.
5. Submit the URL to the Internet Archive's Save Page Now and record the archive link (only if the post does not expose a private victim).
6. Verify: earliest upload (reverse image search on two or three frames), account history, geolocation, chronolocation, signs of editing.
7. Write a five-line verification note with your confidence level and what remains unverified.

### Template

- [evidence-chain-of-custody.md](../../templates/evidence-chain-of-custody.md) — part B, "Online item collection", follows the Berkeley Protocol's online data collection form.

### How you know it worked

- Someone else could open your files, re-hash them and get the same values.
- Your verification note names at least one check from each of the three lenses.
- Your conclusion uses a confidence level and lists what you could not confirm.
- You did not log into anything you were not entitled to or use a false identity.

### Self-check

- [ ] I can define open-source information and say why a private group or a hacked account is not.
- [ ] I capture URL, full page, source code, media, metadata, context, collection data and hashes.
- [ ] I verify through source, technical and content analysis.
- [ ] I record uncertainty instead of rounding up to "confirmed".
- [ ] I protect people who appear in the material.

## Learn more

- **Berkeley Protocol, chapter VI "Investigation process" (pp. 53–67) and Annex IV** — FREE-FULL, English (also Arabic, Chinese, French, Russian, Spanish), no signup, about 60 minutes: <https://www.ohchr.org/sites/default/files/2024-01/OHCHR_BerkeleyProtocol.pdf>. Read collection (para. 155), preservation and verification; compare Annex IV with the form you filled. *Fallback:* the [UC Berkeley publication page](https://humanrights.berkeley.edu/publications/berkeley-protocol-on-digital-open-source-investigations/), which links the other language versions.
- **Bellingcat — Online Open Source Investigation Toolkit, categories "Image/Video", "Geolocation" and "Archiving"** — FREE-FULL (most listed tools free; some have caveats), English, no signup, about 30 minutes: <https://bellingcat.gitbook.io/toolkit>. Watch for: which tools are free, who runs them, and where your uploads go (Protocol Annex V asks the same questions). *Fallback:* WITNESS, [Video as Evidence: Verifying Eyewitness Video](https://library.witness.org/product/video-as-evidence-verifying-eyewitness-video/) (FREE-FULL, about 30 minutes).

## What goes wrong

| Mistake | Consequence | How to fix | How to avoid |
|---|---|---|---|
| Screenshot only, no URL, no time | Authenticity challenged; the post may vanish | Return to the URL at once; archive it; record what is missing | Use the Berkeley minimum for every item |
| Collecting from a private group or someone else's account | Computers Law s. 4 or privacy exposure; evidence excluded | Stop; delete; take advice | Public material only; no logins you were not given |
| Trusting one lens (e.g. "the uploader is reliable") | Recycled or edited footage accepted | Run all three lenses | Verification note with all three |
| Re-posting the violent clip to "debunk" it | Spreads it further; harms people shown | Remove; post a text correction with the source | Correct without amplifying |
| No hash at collection | Cannot prove the copy is unchanged | Hash now and record the gap honestly | Hash immediately after saving |
| Researching from your personal account | Sources see you; you become a target | Separate browser profile and accounts | Plan security before searching (17.5) |

## Review

- Open-source information is what any member of the public can see, buy or request, without special status or unauthorised access; accessing others' accounts or devices is a crime under the Computers Law (s. 4).
- The Berkeley Protocol's cycle: online inquiries, preliminary assessment, collection, preservation, verification, investigative analysis.
- Collect the minimum: URL, full-page capture with time, source code, media, metadata, context, collection data, and a hash at the point of collection.
- Verify through source, technical and content analysis, and state your confidence and what remains unverified.
- No deception, no doxxing, and care for the people in the footage and for yourself.
