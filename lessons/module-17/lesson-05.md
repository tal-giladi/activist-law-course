---
id: "17.5"
module: 17
minutes: 20
practice_minutes: 60
prerequisites: ["17.4", "07.2"]
objectives:
  - "Write a security plan (threat model) for a documentation project using the six EFF questions."
  - "Secure the basics on your own devices and accounts: updates, screen lock and encryption, unique passwords, two-factor authentication, and the active-sessions check."
  - "Choose a messaging setup for sources and the team that protects content and limits metadata, with disappearing messages where suitable."
  - "Know where to get help in a digital emergency, and why you never answer an attack by accessing the attacker's accounts or devices."
volatility: implementation
sources:
  - title: "EFF Surveillance Self-Defense — Your Security Plan (last reviewed 27 Oct 2023)"
    url: https://ssd.eff.org/module/your-security-plan
  - title: "EFF Surveillance Self-Defense — Communicating With Others (last reviewed 6 Aug 2024)"
    url: https://ssd.eff.org/module/communicating-others
  - title: "EFF Surveillance Self-Defense — Attending a Protest (last reviewed 26 Jun 2026)"
    url: https://ssd.eff.org/module/attending-protest
  - title: "Access Now — Digital Security Helpline"
    url: https://www.accessnow.org/help/
  - title: "Access Now — Helpline mandate"
    url: https://www.accessnow.org/helpline-mandate/
  - title: "Berkeley Protocol on Digital Open Source Investigations (OHCHR and UC Berkeley, HR/PUB/20/2, 2022), ch. IV Security and ch. V.A (PDF)"
    url: https://www.ohchr.org/sites/default/files/2024-01/OHCHR_BerkeleyProtocol.pdf
  - title: "חוק המחשבים, התשנ״ה–1995 — ss. 4, 7 (Hebrew Wikisource)"
    url: https://he.wikisource.org/wiki/חוק_המחשבים
  - title: "חוק האזנת סתר, התשל״ט–1979 — ss. 1, 2 (Hebrew Wikisource)"
    url: https://he.wikisource.org/wiki/חוק_האזנת_סתר
last_verified: "2026-10-13"
---

# 17.5 · Digital Security for Activists

Documentation creates exactly the material that others may want to steal, seize, leak or delete: names of witnesses, testimonies, footage, the group's internal chats. In this lesson you learn to think like the EFF's security plan — what to protect, from whom, and at what cost — secure your devices, accounts and messaging, and know whom to call when something goes wrong. You finish with a written security plan for your documentation project and a hardened phone and email account.

> [!WARNING]
> Digital security reduces risk; it never removes it. If someone is in physical danger, contact the police or emergency services first. Never respond to hacking, harassment or surveillance by breaking into the other side's accounts or devices, "hacking back" or doxxing: that is a crime under the Computers Law (s. 4) and can turn a victim into a defendant. Seized devices and police searches are covered in lessons [06.3](../module-06/lesson-03.md) and [07.2](../module-07/lesson-02.md). This lesson is not legal advice.

## Why it matters

A documentation project is a target from several directions at once: people who want to know who testified against them, online harassers from the other side of the issue, scammers who send fake "document" links, a lost phone on a bus, a volunteer who leaves the group angry and still has access to the shared drive. Most real incidents are not sophisticated: a reused password, an account without two-factor authentication, a WhatsApp group with fifty members nobody remembers adding, a laptop without a password. Fixing the basics protects your sources more than any advanced tool.

## Key terms

| עברית | Transliteration | English |
|---|---|---|
| מודל איומים | model iyumim | Threat model: what you protect, from whom, and how likely the harm is |
| תוכנית אבטחה | tochnit avtacha | Security plan |
| הצפנה מקצה לקצה | hatzpana mikatze lekatze | End-to-end encryption |
| אימות דו־שלבי | imut du-shlavi | Two-factor authentication (2FA) |
| מנהל סיסמאות | menahel sisma'ot | Password manager |
| דיוג | diyug | Phishing |
| רוגלה | rogla | Spyware |
| הודעות נעלמות | hoda'ot ne'elamot | Disappearing messages |
| מטא־דאטה של תקשורת | meta-data shel tikshoret | Communication metadata: who talked to whom, when and from where |

## The law

> החודר שלא כדין לחומר מחשב הנמצא במחשב, דינו – מאסר שלוש שנים ...

*Gist:* breaking into a computer, phone or online account without permission carries up to three years; it protects you when someone breaks into your accounts — and it binds you: no "hacking back". The victim may also sue for damage (s. 7). ([Computers Law, s. 4](https://he.wikisource.org/wiki/חוק_המחשבים#סעיף_4))

> ”שיחה“ – בדיבור או בבזק, לרבות בטלפון, בטלפון אלחוטי ברדיו טלפון נייד, במכשיר קשר אלחוטי, בפקסימיליה, בטלקס, בטלפרינטר או בתקשורת בין מחשבים;

*Gist:* a "conversation" under the Wiretap Law includes communication between computers, so secretly intercepting your messages without any party's consent is wiretapping, an offence with up to five years (s. 2). ([Wiretap Law, s. 1](https://he.wikisource.org/wiki/חוק_האזנת_סתר#סעיף_1))

> All individuals conducting investigations online should have basic operational security awareness to ensure that they minimize their digital trail and are aware of the potential risks.

*Gist:* the Berkeley Protocol treats security as a professional duty: assess digital threats and risks before you start, build security into your tools ("security by design"), and protect the confidentiality, integrity and availability of your data. ([Berkeley Protocol, ch. II.A, para. 29; ch. IV](https://www.ohchr.org/sites/default/files/2024-01/OHCHR_BerkeleyProtocol.pdf))

Your group's testimonies and contact lists are also a database with sensitive information, and its holder is responsible for securing it (Privacy Law s. 17; lessons [08.4](../module-08/lesson-04.md) and [17.4](lesson-04.md)).

## How it works in practice

### Step 1 — your security plan

The EFF's security plan asks six questions. Answer them in writing for the project, not for "security in general".

1. **What do I want to protect?** For example: witnesses' identities and contact details, raw testimonies, original footage, the code key, the team's chats, your own location.
2. **Who do I want to protect it from?** The people documented and their supporters, online harassers, criminals and scammers, curious acquaintances, platforms that might delete content, and accidents. Be specific and fair: list risks from every side of your issue.
3. **How bad are the consequences if I fail?** A leaked witness name may mean physical danger; a lost video may mean a lost case.
4. **How likely is it?** Mass phishing is very likely; targeted spyware is rare but possible for prominent activists.
5. **How much trouble am I willing to go through?** A plan the team will not follow is useless; choose measures people will actually use.
6. **Who are my allies?** A tech-savvy volunteer, a partner NGO, the Access Now helpline.

Write the result in the project's security plan: assets, threats, likelihood, measures, who is responsible, and a review date.

### Step 2 — devices

- **Update** the operating system and apps; most attacks use known, patched holes.
- **Screen lock** with a strong passcode (six digits is a minimum; a longer passphrase is better). Make sure device encryption is on — on current phones it is usually tied to the passcode; check the security settings. Encrypt laptops too (BitLocker or Device Encryption on Windows, FileVault on macOS, full-disk encryption on Linux) and external drives that hold evidence.
- **Biometric unlock:** convenient, but someone can hold the phone to your face or finger. EFF advises turning it off when you may be detained (for example on the day of a protest). In Israel a phone search needs a judge's warrant; do not unlock on request (07.2).
- **Separate profiles:** use a separate browser profile, without your personal accounts, for open-source research (17.3).
- **Lost device plan:** turn on "find my device" and remote wipe; keep an encrypted backup so wiping does not destroy evidence (17.4).

### Step 3 — accounts

- **Unique passwords for every account,** stored in a password manager. Never reuse the email password anywhere.
- **Two-factor authentication** on email, cloud storage, social media and messaging. An authenticator app or a hardware security key is stronger than SMS codes.
- **Check active sessions and connected devices** regularly (email, cloud, WhatsApp "Linked devices", Telegram "Devices", Signal "Linked devices") and remove anything you do not recognise.
- **Shared drives:** give access to named people only, remove volunteers who leave on the day they leave, and avoid "anyone with the link".
- **Phishing:** do not open unexpected attachments or log in from links in messages, even from people you know; type the address yourself. Be especially careful with messages that create urgency ("your account will be closed", "urgent video of the attack").

### Step 4 — messaging and metadata

- **End-to-end encryption** means only the sender and the recipients can read the content, not the app provider. Signal and WhatsApp use it by default; in Telegram, only "secret chats" are end-to-end encrypted. SMS and regular calls are not.
- **Metadata** — who you contacted, when and from where — is not protected by encryption and can reveal a source on its own. EFF notes that Signal collects less metadata than alternatives such as WhatsApp.
- **Disappearing messages** for sensitive coordination and source contact, so that a seized or lost phone holds less. Do not use them for material you need as evidence — save that properly first (17.4).
- **Groups:** small groups for sensitive work; admins approve members; no witness names in group chats; codes only (17.1).
- **Sources:** let them choose the channel; explain what each channel protects; never add a source to a group.

### Step 5 — when something goes wrong

1. **Contain:** change the password from a clean device, log out all other sessions, turn on 2FA, check email forwarding rules.
2. **Preserve:** capture evidence of the attack (messages, login alerts) with hashes (17.4) before cleaning up.
3. **Tell** the people who may be affected, especially sources.
4. **Get help.** Access Now's **Digital Security Helpline** is free for civil-society groups, activists, journalists and human-rights defenders, available 24/7, with a first reply within two hours, by email to helpline@accessnow.org (a PGP key is on its page). It works in English, Spanish, French, German, Portuguese, Russian, Tagalog, Arabic, Italian and Ukrainian — **not Hebrew**. Every request is vetted: it does not serve people under 18, people affiliated with current political office holders, criminal groups or armed groups, and it handles digital security only. (Checked 13.10.2026.)
5. **Report** crimes (threats, account break-ins, extortion) to the police; for online harassment and takedowns see lesson [08.5](../module-08/lesson-05.md).

## Worked example

**Situation.** Netanel Shapira coordinates eight volunteers in a South Hebron Hills settlement who document stone-throwing attacks on Israeli drivers and the army's response, for complaints and a report to a Knesset committee. Their material sits in one WhatsApp group of 46 members and a shared drive "anyone with the link can view".

1. **Assets:** drivers' names and car numbers, dash-cam videos, the volunteers' home locations, the report draft.
2. **Threats:** people who might retaliate against drivers who complained; online harassers who dispute the documentation; scammers; volunteers who leave; a lost phone.
3. **Measures chosen:** a new Signal group of the eight volunteers with admin approval and disappearing messages after one week for coordination; videos sent as files to one evidence custodian, hashed and stored in two encrypted places (17.4); the drive limited to three named people; codes instead of drivers' names in all shared files; 2FA on every volunteer's email and the drive; biometric unlock off for volunteers who film near clashes.
4. **Old group:** archived and closed after evidence was exported and hashed.
5. **Review:** every three months, and immediately if a volunteer leaves.

**Mirror test.** The same plan fits a group of Ethiopian-Israeli parents documenting police stops of their teenagers, a Bedouin council documenting home demolitions, or a Tel Aviv protest group documenting attacks on demonstrators. The six questions and the basics do not change; the threats in question 2 do.

## Do it yourself

### You need

- Your own phone and main email account.
- About an hour, and the project issue you chose in 17.1.
- Optional: a password manager (many reputable free options exist).

### Steps

1. Write a one-page security plan for your project with the six EFF questions, a table of assets, threats, likelihood and measures, and a review date.
2. Update your phone's operating system and apps.
3. Check that your phone has a strong passcode and that encryption is on; decide when you will turn off biometric unlock.
4. Turn on two-factor authentication (authenticator app or security key) on your main email account; save the backup codes somewhere safe and offline.
5. Review active sessions and linked devices on your email, cloud storage and messaging apps; remove anything you do not recognise.
6. In your messaging app, turn on disappearing messages for one sensitive conversation and check who is in each group you use for activism.
7. Write down three emergency steps for "my account was taken over" and the Access Now helpline address.

### Template

None. Use the security plan structure in "Step 1" above; the evidence storage rules are in [evidence-chain-of-custody.md](../../templates/evidence-chain-of-custody.md).

### How you know it worked

- Your plan names specific assets and threats from every side of your issue, not "hackers" in general.
- Your email asks for a second factor when you log in from a new browser.
- No unknown session or device is linked to your accounts.
- You can say which of your conversations are end-to-end encrypted and which are not.

### Self-check

- [ ] I have a written security plan with a review date.
- [ ] My devices are updated, locked with a strong passcode and encrypted.
- [ ] My important accounts have unique passwords and two-factor authentication.
- [ ] I know encryption protects content but not metadata, and I use disappearing messages where suitable.
- [ ] I know where to get help and I never "hack back".

## Learn more

- **EFF Surveillance Self-Defense — "Your Security Plan", "Communicating With Others" and "Attending a Protest"** — FREE-FULL, English (and Arabic, Spanish, French, Russian, Turkish and other languages; no Hebrew version found), no signup, about 45 minutes: <https://ssd.eff.org/module/your-security-plan>, <https://ssd.eff.org/module/communicating-others>, <https://ssd.eff.org/module/attending-protest>. Note that the protest guide is written for US law; for Israeli phone-search rules use lesson 07.2. *Fallback:* the Berkeley Protocol, ch. IV "Security" (pp. 31–41), free PDF: <https://www.ohchr.org/sites/default/files/2024-01/OHCHR_BerkeleyProtocol.pdf>.
- **Access Now — Digital Security Helpline** — FREE-FULL service, English and nine other languages including Arabic, 10 minutes to read the page and the mandate: <https://www.accessnow.org/help/> and <https://www.accessnow.org/helpline-mandate/>. *Fallback:* EFF's [Security Scenarios](https://ssd.eff.org/module-categories/security-scenarios).

## What goes wrong

| Mistake | Consequence | How to fix | How to avoid |
|---|---|---|---|
| Reusing one password across accounts | One breach opens everything | Change all, starting with email; turn on 2FA | Password manager, unique passwords |
| Large open groups with witness names | A member leaks or a phone is lost | Close the group; move to a small, admin-approved group; notify sources | Codes only; small groups |
| SMS as the only second factor | SIM-swap takeover | Move to an authenticator app or key | Use app or key from the start |
| Volunteer who left still has drive access | Data leak or deletion | Remove access; review the log | Remove access the day someone leaves |
| "Hacking back" an attacker's account | Computers Law s. 4 offence; evidence excluded | Stop; take legal advice | Contain, preserve, report |
| Relying on disappearing messages for evidence | Evidence is gone | Ask the sender to resend as a file | Save and hash evidence before it disappears |

## Review

- Start with a written security plan: what you protect, from whom, how bad, how likely, what effort, and who helps.
- Basics first: updates, strong passcode and encryption, unique passwords, two-factor authentication, regular session checks.
- End-to-end encryption protects content, not metadata; use small groups, codes and disappearing messages where suitable.
- The Computers Law and the Wiretap Law protect your data and communications — and forbid you from hacking back.
- In an emergency: contain, preserve, tell, get help (Access Now's helpline, free and 24/7, in ten languages but not Hebrew) and report crimes.
