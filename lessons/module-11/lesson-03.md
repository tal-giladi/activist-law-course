---
id: "11.3"
module: 11
minutes: 15
practice_minutes: 45
prerequisites: ["11.2", "05.6"]
objectives:
  - "Log in to Net HaMishpat with National Digital Identity and find your own case through 'התיקים שלי'."
  - "Choose the right filing path — opening a case, 'הגשות' (new request, response to an existing request, other filings) or 'הגשה מהירה' — for a given document."
  - "Know when a document counts as served on you and on the court, and what to do when the registry rejects a filing."
  - "Prepare a court-ready PDF filing with a heading, numbered paragraphs and exhibits."
volatility: implementation
sources:
  - title: "Judiciary (gov.il) — מדריך שימוש במערכת נט המשפט, chapter: צדדים בתיק שלא מיוצגים בידי עו״ד (updated 17.9.2026)"
    url: https://www.gov.il/he/pages/netlaw_guide_24?chapterIndex=3
  - title: "Net HaMishpat"
    url: https://www.court.gov.il/NGCS.Web.Site/HomePage.aspx
  - title: "תקנות סדר הדין האזרחי, התשע״ט–2018 — regs 33, 160–162, 179 (Hebrew Wikisource)"
    url: https://he.wikisource.org/wiki/תקנות_סדר_הדין_האזרחי
  - title: "Judiciary (gov.il) — הגשת תביעה קטנה (online filing from a computer only)"
    url: https://www.gov.il/he/service/filing_a_small_claim
  - title: "Judiciary (gov.il) — בקשת פטור מתשלום אגרה או עירבון (filing channels for parties without a lawyer)"
    url: https://www.gov.il/he/service/exempt_from_payment_of_a_fee
last_verified: "2026-10-13"
---

# 11.3 · Net HaMishpat for Unrepresented Parties

Net HaMishpat (נט המשפט) is the courts' online system: you open some cases there, file every later document, read decisions and get notified by SMS and email. Lesson 05.6 showed how to file a petition through it; this lesson covers what a party without a lawyer does inside a civil case — finding the case, picking the right filing path, knowing when something counts as served, and fixing a rejected filing.

## Why it matters

In a civil case, the documents keep coming: the defence, a request to postpone, the court's decisions, an order to file something within 10 days. If you do not see a decision, or you file a response as a "new request" so it never reaches the judge, you can miss a deadline without noticing. The system is simple once you know its three filing paths and its few traps.

## Key terms

| עברית | Transliteration | English |
|---|---|---|
| נט המשפט | net hamishpat | The courts' e-filing and case system |
| הזדהות לאומית | hizdahut le'umit | National Digital Identity: the free government login |
| האזור האישי | ha'ezor ha'ishi | The judiciary's personal area for parties without a lawyer |
| בעל דין בלתי מיוצג | ba'al din bilti meyutzag | A party without a lawyer |
| בקשה חדשה | bakasha chadasha | New request: asks the court for something new |
| הגשה מהירה | hagasha mehira | Quick filing: files into a case without entering it |
| אסמכתא | asmachta | Reference number of a filing |
| מזכירות | mazkirut | Court registry |
| קבלה לרישום | kabala lerishum | Acceptance of a document for filing by the registry |

## The law

> המצאה אלקטרונית של מסמך אלקטרוני לבית המשפט תהיה באמצעות מערכת נט המשפט;

*Gist:* filing a document electronically with the court is done through Net HaMishpat. ([Civil Procedure Regulations 2018, reg. 161(1)(ב)](https://he.wikisource.org/wiki/תקנות_סדר_הדין_האזרחי#סעיף_161))

> אם בעל הדין אינו מיוצג בידי עורך דין, יגיש את המסמך למזכירות בית המשפט, שתפעל להמצאתו.

*Gist:* a lawyer must send copies of filings to the other side, but a party without a lawyer files with the registry and the registry serves it. ([reg. 160](https://he.wikisource.org/wiki/תקנות_סדר_הדין_האזרחי#סעיף_160))

> אם השולח הוא אינו בית המשפט והנמען הוא בעל דין שאינו מיוצג בידי עורך דין, זולת אם הנמען נתן את הסכמתו לכך בכתב;

*Gist:* the other side may not serve you by email unless you agreed in writing; the first document in a case (the claim) is served by post or by hand. ([reg. 162(1)–(2)](https://he.wikisource.org/wiki/תקנות_סדר_הדין_האזרחי#סעיף_162))

> ואם נשלחה הודעה אלקטרונית מבית המשפט לנמען שאינו מיוצג בידי עורך דין כאמור בתקנת משנה (א), מועד פתיחת המסמך האלקטרוני כפי שמופיע בשעון פנימי כאמור יהיה מועד ההמצאה של המסמך האלקטרוני,

*Gist:* when the court notifies you electronically, the document counts as served when you open it; after 17:00, or on a Friday or rest day, it counts from the next working day. ([reg. 161(1)(ד)](https://he.wikisource.org/wiki/תקנות_סדר_הדין_האזרחי#סעיף_161))

> לא התקבל המסמך לרישום, יראו אותו כאילו לא הוגש מלכתחילה, ואולם יהיה ניתן לתקן את הפגם עד היום האחרון להגשתו או בתוך שבעה ימים מהמועד שלא קובל, לפי המאוחר;

*Gist:* a document the registry refuses (for example, too many pages or a missing heading item) counts as never filed, but you may fix it by the deadline or within seven days of the refusal, whichever is later; you may ask a judge to review the refusal within seven days. ([reg. 33(ג), (ה)](https://he.wikisource.org/wiki/תקנות_סדר_הדין_האזרחי#סעיף_33))

Checked on Hebrew Wikisource and the judiciary's guide (updated 17.9.2026) on 13 October 2026.

## How it works in practice

### Getting in

1. Use a computer, not a phone: the small-claims filing service and Net HaMishpat work from a computer only.
2. Open [Net HaMishpat](https://www.court.gov.il/NGCS.Web.Site/HomePage.aspx) and log in with National Digital Identity (הזדהות לאומית). If you have never set it up, the judiciary information centre (*3852, 077-2703333, or WhatsApp 050-6255727) helps with registration.
3. The judiciary's personal area (האזור האישי) shows your cases, documents and messages; Net HaMishpat is where you file.

### Finding your case

Type the case number in the top bar and press "אתר". If you do not know it: "איתור תיקים" → "התיקים שלי", optionally by date range or court. If you get "אינך מורשה לבצע פעולות בתיק", your ID number is not attached to the case correctly — ask to add it through "הגשה מהירה", by fax, or at the registry counter.

### The three filing paths

| Path | Use it for | Do not use it for |
|---|---|---|
| **Opening a case** ("פתיחת תיק") | A new small claim (through the judiciary's small-claims service), or a new proceeding | — |
| **"הגשות" → בקשה חדשה** | Asking for something new: postponing a hearing, an extension, permission to add a document, summoning a witness | Answering the other side's request |
| **"הגשות" → כתב טענות לבקשה קיימת** | Your response to a request that already has a number (write that number) | A new request |
| **"הגשות" → הגשות אחרות** | Documents that are neither requests nor responses: a defence, an affidavit, an expert opinion, a counterclaim | — |
| **"הגשה מהירה"** | Filing when you cannot enter the case, or your ID is not attached | Opening any case, including a small claim; urgent orders (those go to the registry counter) |

Each request gets its own number in the order filed (request 2, request 3…), and every response and decision about it is filed under that number. That is how the judge sees the whole thread.

### Fees for requests

Some requests carry a fee. When you file a new request, choose the right category and request type; the system shows whether a fee applies and sends you to the government payment service. The registry rejects a request that needed a fee and was not paid.

### Files

PDF only for documents; up to 70 MB per file (judiciary guide, 17.9.2026). Scan exhibits legibly, name them (נספח 1, נספח 2…) and refer to each in a numbered paragraph. Audio and video: follow the court's instructions; in small claims they go to the registry on USB drives with a transcript (lesson 11.2).

### After you file

You get a reference number (אסמכתא). From the end of the next working day you can check the filing's status under "הגשות" → search by reference. Decisions arrive as SMS and email notices; open them promptly, because opening starts the clock (reg. 161(1)(ד)).

### A fee exemption request

The judiciary's fee-exemption page lists online filing in Net HaMishpat for lawyers only; a party without a lawyer files it by registered mail or at a registry counter (lesson 11.6). For a small claim, ask *3852 whether the online small-claims service accepts your exemption request with the claim.

## Worked example

**Situation.** Yulia, an immigrant from Kharkiv who campaigns for civil marriage, filed a small claim against a wedding-planning company that kept her ₪5,200 deposit after she cancelled within the period the contract allowed. The company filed a defence. Two weeks before the hearing Yulia gets an SMS: a new decision in her case.

1. **Read the decision.** She logs in with National Digital Identity and opens the case from "התיקים שלי". The decision: "The defendant asks to postpone the hearing (request 2). The claimant will respond within 5 days." The clock started when she opened the notice that evening at 19:30 — so it counts from the next working day.
2. **Respond in the right place.** She goes to "הגשות" → "כתב טענות לבקשה קיימת" and enters request number 2. Her one-page response: she objects, because she has arranged leave from work and her witness; alternatively, any new date should be soon.
3. **Add a document.** She also has a new email from the company admitting the cancellation was on time. Adding it needs the court's permission, so she files "בקשה חדשה": a request to add a document, with the email as נספח 1.
4. **Check status.** The next evening she searches her two references; both show as received. A day later: request 2 refused; request 3 granted.

## Do it yourself

### You need

- A computer and your National Digital Identity login (or the free registration).
- The fictional case below, or a real case you are a party to.
- 45 minutes.

Fictional case: you sued a bus company in small claims after a driver refused to stop for you at a stop near your yeshiva. The court gave a decision: "The claimant will state within 7 days whether he agrees to a hearing by video." You also want to ask for a later hearing date because of your exams.

### Steps

1. Log in to Net HaMishpat with National Digital Identity (if you have no case, stop at the home screen and explore "איתור תיקים").
2. For each document below, write which filing path you would use and why: (a) your answer about the video hearing; (b) your request for a later date; (c) your affidavit if the court orders one; (d) a document from a person who has no access to the case.
3. Draft (b) as a one-page PDF: heading with the court and case number, the parties, "בקשה לדחיית מועד דיון", numbered reasons, the new dates you propose, whether the other side agrees, signature and date.
4. Write when your 7 days for (a) end if you opened the notice on a Monday at 18:15.
5. Write what you would do if the registry rejected (b) for a missing detail.

> [!IMPORTANT]
> This exercise is a dry run. If you file in a real case: act in your own name only. This is not legal advice — check current rules before filing.

### Template

- [small-claim-statement.md](../../templates/small-claim-statement.md) — its heading block works for any later filing in a small claim; replace the title with your request type.

### How you know it worked

- Each of (a)–(d) is matched to the right path: (a) response to an existing request or the path the decision names; (b) new request; (c) other filings; (d) quick filing.
- Your draft request has a heading, numbered reasons, a proposed date and the other side's position.
- Your notice counts as served on Tuesday (the next working day), not Monday.

### Self-check

- [ ] I can log in with National Digital Identity from a computer.
- [ ] I know a response goes under the existing request number, not as a new request.
- [ ] I know quick filing cannot open a small claim.
- [ ] I know when an electronic notice counts as served on me.
- [ ] I know a rejected document counts as not filed, and how long I have to fix it.

## Learn more

- **Judiciary — Net HaMishpat guide, chapter for parties without a lawyer** — FREE-FULL, Hebrew, no signup to read, 15 minutes: <https://www.gov.il/he/pages/netlaw_guide_24?chapterIndex=3>. Open both sections (הגשות; הגשה מהירה) and the attached graphic PDF guide. Fallback: call *3852 and ask them to walk you through "הגשות" on the phone.

## What goes wrong

| Mistake | Consequence | How to fix | How to avoid |
|---|---|---|---|
| Response filed as a new request | The judge may not see it in the thread | File it again under the request number | Always enter the existing request number |
| Trying to open a small claim by quick filing | Not accepted | Use the small-claims service / "פתיחת תיק" | Read the judiciary guide first |
| "אינך מורשה לבצע פעולות בתיק" | You cannot file in your case | Ask to attach your ID via quick filing or the registry | Use the same ID on every filing |
| Not opening notices | You miss decisions and deadlines | Open the case daily during active periods | Turn on SMS and email updates; check weekly |
| Registry rejects a filing | It counts as not filed | Fix within the deadline or 7 days (reg. 33(ג)); ask a judge within 7 days (reg. 33(ה)) | Check pages, heading and fee before sending |
| Phone-only access | Cannot file | Use a computer at a library or volunteer station | Plan computer access before deadlines |

## Review

- Log in to Net HaMishpat with National Digital Identity from a computer; find your case through "התיקים שלי".
- Three paths: new request; response under an existing request number; other filings — plus quick filing when you cannot enter the case.
- A party without a lawyer files with the registry, which serves the other side (reg. 160); you need not accept email service from the other side without consent (reg. 162).
- An electronic notice counts as served when you open it, or the next working day after 17:00 (reg. 161).
- A rejected filing counts as not filed; fix it within the deadline or seven days (reg. 33).
