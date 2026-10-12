# Evidence Chain of Custody (רישום שרשרת משמורת לראיות)

A register that records, for every item of evidence, where it came from, who collected it, its SHA-256 hash, where the original is kept, and every time it changed hands — so that you can later show a court, the police or a UN body that the item is the same one you collected. Part B follows the Berkeley Protocol's online data collection form (Annex IV). Taught in [lesson 17.3](../lessons/module-17/lesson-03.md) and [lesson 17.4](../lessons/module-17/lesson-04.md), and used in the [Module 17 project](../projects/m17-documentation-kit.md).

> [!IMPORTANT]
> For use in your own name or your group's own name. This is not legal advice. Collect only lawful material: public online content, your own recordings of conversations you take part in, and material people gave you with consent. Never access anyone else's account or device (Computers Law s. 4). The register itself contains sensitive information: store it encrypted, separately from the code key (lesson 17.5).

## How to use it

1. Open the register when you open the incident log ([incident-log.md](incident-log.md)). Item numbers (E-01, E-02 …) are shared between the two.
2. **Never work on the original.** Save the original, hash it, store it read-only in two places, and make working copies for viewing, cutting, blurring or transcribing (part F).
3. Hash every original immediately after saving it, with SHA-256. Record the full hash, not a shortened one.
4. Every time an item is copied to another person or body (a lawyer, the police, an NGO, the UN), add a row to part D and record whether the receiver's hash matched.
5. Re-check hashes of originals on a schedule (for example every three months) and record the result in part E.
6. Never delete or overwrite a row. Corrections go in a new row with the date and reason.

### Hash commands (SHA-256, built into each system)

```powershell
# Windows (PowerShell)
Get-FileHash -Algorithm SHA256 "C:\Evidence\E-01_video.mp4"
```

```bat
:: Windows (Command Prompt)
certutil -hashfile "C:\Evidence\E-01_video.mp4" SHA256
```

```bash
# macOS (Terminal) — note: without "-a 256" shasum uses SHA-1
shasum -a 256 ~/Evidence/E-01_video.mp4

# Linux (Terminal)
sha256sum ~/Evidence/E-01_video.mp4
```

## A. Case details — פרטי התיק

| שדה (Field) | תוכן (Entry) |
|---|---|
| שם הפרויקט / התיק (Project or case) | |
| מטרה (Purpose — lesson 17.1) | |
| אחראי/ת על הראיות (Evidence custodian) | |
| מיקום המקור — עותק 1 (Original storage, copy 1) | |
| מיקום המקור — עותק 2 (Original storage, copy 2, off-site) | |
| הצפנה (Encryption used) | |
| שעון מסונכרן? (Computer clock set automatically? yes/no) | |

## B. Online item collection — איסוף פריט מקוון (Berkeley Protocol, Annex IV)

Fill one block per online item.

| שדה (Field) | תוכן (Entry) |
|---|---|
| מס׳ פריט (Item #) | E-__ |
| מאסף/ת (Collector) | |
| תחילת איסוף — תאריך ושעה (Start of collection) | |
| סיום איסוף — תאריך ושעה (End of collection) | |
| כתובת URL מדויקת (Exact URL of the post) | |
| חשבון מעלה, מזהה, שעת העלאה (Uploader account, ID, upload time as shown) | |
| צילום עמוד מלא עם תאריך ושעה — שם קובץ (Full-page capture file) | |
| קוד מקור HTML — שם קובץ (HTML source file) | |
| מדיה מוטמעת — שם קובץ (Embedded media file) | |
| מטא־דאטה שנאספה (Metadata captured: post ID, geotag, hashtags, views) | |
| הקשר (Context: comments, related posts) | |
| עותק בארכיון ציבורי (Public archive link, e.g. Save Page Now — or "not archived: reason") | |
| חשבון ששימש לגישה (Account used to view, if any; never a false identity) | |
| תוכנה ומכשיר (Software, browser and device used) | |
| רשימת ערכי גיבוב — SHA-256 של כל קובץ (Hash list: SHA-256 of each file) | |
| הערות (Notes: anything altered or converted during collection) | |

## C. Evidence register — רשימת ראיות

| מס׳ (Item #) | תיאור (Description) | שם קובץ מקורי (Original file name) | מקור (Source — code or URL) | נאסף ע״י (Collected by) | תאריך ושעת איסוף (Date, time collected) | אופן האיסוף (Method: own recording / download / screenshot / given by source) | SHA-256 | מיקומי שמירה (Storage locations) | הסכמה (Consent ref., if from a person) |
|---|---|---|---|---|---|---|---|---|---|
| E-01 | | | | | | | | | |
| E-02 | | | | | | | | | |
| E-03 | | | | | | | | | |
| E-04 | | | | | | | | | |

## D. Transfer log — יומן העברות

| תאריך ושעה (Date, time) | מס׳ פריט (Item #) | ממי (From) | למי (To) | מטרה (Purpose) | אמצעי העברה (Method: encrypted link, USB, in person) | הגיבוב תאם אצל המקבל? (Receiver's hash matched? yes/no) | חתימות / אישור (Signatures or written confirmation) |
|---|---|---|---|---|---|---|---|
| | | | | | | | |
| | | | | | | | |

## E. Hash re-check log — בדיקות גיבוב חוזרות

| תאריך (Date) | פריטים שנבדקו (Items checked) | מיקום (Storage location) | תוצאה (Result: all match / mismatch in …) | פעולה (Action taken) | בודק/ת (Checked by) |
|---|---|---|---|---|---|
| | | | | | |

## F. Working copies and redactions — עותקי עבודה והשחרות

| קובץ נגזר (Derived file) | נגזר מפריט (From item #) | מה שונה (What changed: cut, blurred, metadata removed, transcribed) | כלי (Tool) | SHA-256 של הקובץ הנגזר (Hash of derived file) | שימוש (Use: publication, complaint, translation) | תאריך ומבצע/ת (Date, by) |
|---|---|---|---|---|---|---|
| | | | | | | |

## Checklist

- [ ] Every original hashed with SHA-256 at the time of saving.
- [ ] Originals stored unchanged in two places, one off-site, encrypted.
- [ ] Working copies listed in part F with what changed; originals never edited.
- [ ] Every transfer recorded in part D with the receiver's hash check.
- [ ] Hashes re-checked on schedule (part E).
- [ ] No item obtained by accessing someone else's account or device.
