---
id: "17.4"
module: 17
minutes: 20
practice_minutes: 60
prerequisites: ["17.3", "08.4"]
objectives:
  - "Compute and record a SHA-256 hash of a file with the tools built into Windows, macOS and Linux, and re-check it later."
  - "Keep a chain of custody: untouched originals in two places, working copies for every edit, and a log of every transfer."
  - "Archive a public web page with the Internet Archive's Save Page Now and record the archive link."
  - "Decide when to preserve metadata (originals and evidence) and when to strip it (copies for publication), and do both."
volatility: implementation
sources:
  - title: "Berkeley Protocol on Digital Open Source Investigations (OHCHR and UC Berkeley, HR/PUB/20/2, 2022), ch. VI.C–D, paras 155–175 (PDF)"
    url: https://www.ohchr.org/sites/default/files/2024-01/OHCHR_BerkeleyProtocol.pdf
  - title: "Microsoft Learn — Get-FileHash (PowerShell 7.6; default algorithm SHA256)"
    url: https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/get-filehash
  - title: "Microsoft Learn — certutil, -hashfile"
    url: https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/certutil
  - title: "SS64 — shasum (macOS)"
    url: https://ss64.com/mac/shasum.html
  - title: "man7.org — sha256sum(1), GNU coreutils 9.11"
    url: https://man7.org/linux/man-pages/man1/sha256sum.1.html
  - title: "Internet Archive — Save Page Now"
    url: https://web.archive.org/save
  - title: "Internet Archive Help Center — Using the Wayback Machine"
    url: https://help.archive.org/help/using-the-wayback-machine/
  - title: "Apple — Personal Safety User Guide: Manage location metadata in Photos"
    url: https://support.apple.com/guide/personal-safety/ips0d7a5df82
  - title: "Publications Office of the EU — Removing metadata and personal information (Windows)"
    url: https://op.europa.eu/en/web/webguide/removing-metadata-and-personal-information
  - title: "ExifTool by Phil Harvey (version 13.59, 27 May 2026)"
    url: https://exiftool.org/
  - title: "WITNESS Library — Activists' Guide to Archiving Video (v1.2, 2017)"
    url: https://library.witness.org/product/activists-guide-to-archiving-video/
  - title: "חוק הגנת הפרטיות, התשמ״א–1981 — s. 17 (Hebrew Wikisource)"
    url: https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות
last_verified: "2026-10-13"
---

# 17.4 · Preserving and Archiving Evidence

Evidence that is lost, changed or cannot be traced is worth little. In this lesson you learn to keep originals untouched, fingerprint every file with a SHA-256 hash using tools already on your computer, log every hand-over in a chain of custody, archive public pages before they disappear, and handle metadata the right way — keep it on originals, strip it from what you publish. You finish by running the full routine on files of your own.

> [!WARNING]
> Preserved evidence about real people is sensitive personal information. A leaked archive can expose victims and witnesses to retaliation, and as the holder you are responsible for keeping it secure (Privacy Law s. 17; lesson [08.4](../module-08/lesson-04.md)). Publishing a photo with its location data can reveal where the person who filmed it lives. Archive publicly only what is safe to be public forever. This lesson is not legal advice.

## Why it matters

Posts are deleted by their authors and removed by platforms, phones are lost or seized, cloud accounts are closed, and files are quietly re-saved by apps that change them. Months later, when a complaint is investigated or a petition is heard, the other side will ask: is this the same file you collected? Who had it? Was it edited? A simple routine answers those questions: a hash recorded at collection, an untouched original, a log of every transfer. It costs minutes per item and is the difference between evidence and an anecdote.

## Key terms

| עברית | Transliteration | English |
|---|---|---|
| שרשרת משמורת | sharsheret mishmoret | Chain of custody: the record of who held an item, when and why |
| קובץ מקור | kovetz makor | Original file |
| עותק עבודה | otek avoda | Working copy |
| ערך גיבוב | erech gibuv | Hash value (SHA-256) |
| שלמות | shlemut | Integrity: the file has not changed |
| מקוריות | mekoriyut | Authenticity: the item is what it claims to be |
| גיבוי | gibuy | Backup |
| ארכוב | arkuv | Archiving |
| הסרת מטא־דאטה | hasarat meta-data | Metadata stripping |
| מאגר מידע | ma'agar meida | Database (Privacy Law) |

## The law

> Authenticity refers to the ability to demonstrate that a digital item remains unchanged from when it was collected. It requires that a digital item remain unaltered while in an archive or that any modifications to it are documented.

*Gist:* keep the item unchanged, and if you must change anything, document exactly what and when. ([Berkeley Protocol, ch. VI.D, para. 160](https://www.ohchr.org/sites/default/files/2024-01/OHCHR_BerkeleyProtocol.pdf))

> It is therefore important to maintain backup copies and regularly monitor storage infrastructure and the permanence of stored files, such as by checking the hash values of random samples on a regular basis to ensure that no degradation has occurred.

*Gist:* every storage device eventually fails; keep backups and re-check hashes on a schedule. (Berkeley Protocol, para. 172)

> (א) בעל שליטה במאגר מידע ומחזיק במאגר מידע, כל אחד מהם אחראי לאבטחת המידע שבמאגר המידע.

*Gist:* whoever controls or holds a database of personal information is responsible for securing it. A group's collection of testimonies, names and photos is very likely a "מאגר מידע" with information of special sensitivity, so the security duties of Amendment 13 apply (lesson 08.4). ([Privacy Law, s. 17(א)](https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות#סעיף_17))

## How it works in practice

### Originals and working copies

1. **Save the original** exactly as received: the downloaded video, the voice note, the photo from your camera. Do not rename by "opening and saving", do not edit, do not send through apps that compress (many messaging apps re-encode photos and video; send as a "document/file" instead).
2. **Name and store it** in a folder per case: `E-01_2026-03-14_voice-note.m4a`. Codes, not names (17.1).
3. **Hash it at once** (below) and enter the hash in the evidence register ([evidence-chain-of-custody.md](../../templates/evidence-chain-of-custody.md), part C).
4. **Keep two copies of the originals** in two different places, at least one off-site (for example an encrypted external drive at home and an encrypted cloud folder). Mark the originals folder read-only.
5. **Work on copies.** Every trimmed clip, blurred photo, transcript or translation is a new, derived file. Record it in part F: from which original, what changed, its own hash.

### Hashing with built-in tools

A hash is a short fingerprint of the file's content. Change one byte and the hash changes completely; rename the file and it stays the same. SHA-256 is today's common standard; MD5 and SHA-1 are no longer considered secure (Microsoft's documentation says so) and should not be used for evidence.

**Windows** (PowerShell is built in; `Get-FileHash` uses SHA-256 by default — checked on PowerShell 7.6 and Windows PowerShell 5.1):

```powershell
Get-FileHash -Algorithm SHA256 "C:\Evidence\E-01_video.mp4"

# Hash every file in a folder and save the list
Get-FileHash -Algorithm SHA256 "C:\Evidence\originals\*" | Export-Csv "C:\Evidence\hashes_2026-10-13.csv" -NoTypeInformation

# Re-check one file later against the recorded value (the comparison ignores upper/lower case)
(Get-FileHash -Algorithm SHA256 "C:\Evidence\E-01_video.mp4").Hash -eq "PASTE-THE-RECORDED-HASH-HERE"
```

Alternative in the Command Prompt: `certutil -hashfile "C:\Evidence\E-01_video.mp4" SHA256`.

**macOS** (Terminal). `shasum` uses SHA-1 unless you add `-a 256`:

```bash
shasum -a 256 ~/Evidence/E-01_video.mp4

# Hash all originals into a list, then re-check them all later
cd ~/Evidence/originals
shasum -a 256 * > ../hashes_2026-10-13.txt
shasum -a 256 -c ../hashes_2026-10-13.txt
```

**Linux** (Terminal, GNU coreutils):

```bash
sha256sum ~/Evidence/E-01_video.mp4

cd ~/Evidence/originals
sha256sum * > ../hashes_2026-10-13.txt
sha256sum -c ../hashes_2026-10-13.txt
```

The check command prints `OK` for each file that has not changed and `FAILED` for any that has. Keep the hash lists with the register, and hash the list file itself too.

### Chain of custody

Every time an item leaves your hands — to a lawyer, the police, the Police Investigation Department, an NGO, a UN body — add a row to the transfer log (part D): date, item, from, to, purpose, method, and whether the receiver's hash matched yours. Send the hash list with the files and ask the receiver to confirm. Re-check your stored originals every few months and log the result (part E). If a hash ever fails, do not "fix" it: record it, restore from the other copy, and note what happened.

### Archiving web pages: Save Page Now

The Internet Archive's Save Page Now (<https://web.archive.org/save>) captures "a web page as it appears now for use as a trusted citation in the future". Paste the URL and save; the result is a Wayback Machine address with the capture date and time in it. Record that address in the register (part B).

- **Options** (checked 13.10.2026): "Save outlinks" and "Save error pages" are open to all; signing in to a free account adds "Save screenshot", saving to "My Web Archive", and e-mailing the results or a WACZ file.
- **Limits:** it saves one page at a time; some platforms (especially pages behind a login and some social networks) do not capture well, so always keep your own capture too (17.3). Site owners can ask the Archive to exclude material, so an archive link is a second copy, not a substitute for your original.
- **Think before archiving:** an archived page is public and practically permanent. Do not archive a page whose main effect would be to keep a private victim's identity online.

### Metadata: preserve or strip?

Photos and videos usually carry metadata: date and time, device, and often GPS coordinates. The rule is simple:

| File | Metadata | Why |
|---|---|---|
| Original, kept as evidence | **Preserve**, untouched | It helps prove when and where; editing it breaks authenticity |
| Copy sent to a lawyer or investigator | **Preserve** (send the original, with hash) | They need what you have |
| Copy for publication, a newsletter or a public report | **Strip** location and device data | It can reveal where the filmer lives or who they are |
| Copy shared with people outside the team | **Strip** unless they need it | Data minimisation (17.1) |

Ways to strip, with built-in tools (checked 13.10.2026):

- **iPhone/iPad:** in Photos, select → Share → *Options* → turn off *Location* before sharing. To remove the location from a copy in your library: Info → *Adjust* → *No Location*.
- **Mac Photos:** Image → Location → *Hide Location* (for a copy you export).
- **Windows:** right-click the file → Properties → Details → *Remove Properties and Personal Information* → choose *Create a copy with all possible properties removed*. Use the copy option, so the original keeps its metadata.
- **Any system, free tool:** ExifTool (version 13.59 at the time of writing) reads metadata with `exiftool photo.jpg` and removes it with `exiftool -all= photo.jpg`, keeping the untouched file as `photo.jpg_original`. ExifTool warns that removal is not guaranteed to be complete for formats other than JPEG; check the result.

Stripping metadata changes the file, so the stripped copy has a new hash: log it in part F as a derived file.

### Capturing new footage

If your group expects to receive footage from people filming their own experiences in the future, apps such as **eyeWitness to Atrocities** (Android) capture photos and video with embedded verification metadata and transmit them securely to the eyeWitness organisation, which keeps custody for legal use. Read its terms first: the footage goes to a third party. Ordinary phone footage is still usable if you keep the original and log its custody.

## Worked example

**Situation.** Michal Ezra, an activist in the hostage families' protest movement, receives threats: public comments under her posts on a social network ("we know where you live", with her street name), and three direct messages from an account with no name. She wants to file a police complaint and keep the evidence safe.

1. **Lawful collection.** The public comments are open source. The direct messages were sent *to her*, so she may keep and use them as the recipient (she does not access anyone else's account).
2. **Capture.** For each public comment: URL, full-page PDF with date and time, the account's profile page. For the direct messages: screenshots showing the account name and time, plus the platform's own data download of her account, which includes the messages.
3. **Hash and register.** She saves everything in `Evidence/originals`, runs `Get-FileHash` on the folder, exports the list, and opens the evidence register with items E-01 to E-07.
4. **Archive?** The comments include her own street name. She does **not** submit them to Save Page Now (it would preserve her address publicly); her own captures and the platform's data download are enough.
5. **Two copies.** An encrypted USB drive at her parents' home and an encrypted cloud folder.
6. **Transfer.** At the police station, she hands over a USB with copies and the hash list, and asks the officer to note the files received. She records the transfer in part D, with the complaint number.
7. **Publication.** For a post about the threats, she makes a working copy of one screenshot with her street name blacked out and logs it in part F.

**Mirror test.** The same routine fits a Druze council member threatened over a vote, a settler leader whose family is threatened online, or an LGBT activist doxxed in a Telegram channel: own captures, hashes, two copies, a transfer log, and nothing archived publicly that endangers the person.

## Do it yourself

### You need

- Your computer (Windows, macOS or Linux), with no extra installation.
- Three files of your own: a photo you took with your phone (with location on), a short voice memo, and a public web page about any public issue.
- The template [evidence-chain-of-custody.md](../../templates/evidence-chain-of-custody.md).
- 60 minutes.

### Steps

1. Create a folder `Evidence/originals` and copy the photo and the voice memo into it as files (not through a messaging app). Save the web page as a PDF into the same folder.
2. Hash all three files with your system's command and save the hash list with today's date in the file name.
3. Fill part C of the register for E-01 to E-03.
4. Submit the web page's URL to Save Page Now and record the archive address and capture time in part B.
5. Make a copy of the photo with its location removed (iPhone Share → Options, Windows "Create a copy…", or ExifTool). Hash the copy and log it in part F. Confirm that the original still has its location.
6. Change one character in a copy of the PDF's file name, re-hash it, and confirm the hash did *not* change. Then open the voice memo copy in an editor, trim one second, save, and confirm the hash *did* change.
7. Run the check command (`shasum -a 256 -c` or `sha256sum -c`, or the PowerShell comparison) on the originals and log the result in part E.
8. Store a second copy of the originals and the register in a second place, and write both locations in part A.

### Template

- [evidence-chain-of-custody.md](../../templates/evidence-chain-of-custody.md) — case details, online item collection (Berkeley Annex IV), evidence register with SHA-256, transfer log, hash re-check log, working copies and redactions.

### How you know it worked

- Re-hashing the originals gives exactly the recorded values.
- Renaming a file did not change its hash; editing it did.
- The published copy of the photo has no location; the original still does.
- You have an archive address for the web page, with a capture date in it.

### Self-check

- [ ] I hash every original with SHA-256 at the time I save it.
- [ ] I keep originals untouched in two places and work only on copies.
- [ ] I log every transfer and ask the receiver to confirm the hash.
- [ ] I know what Save Page Now saves, what it does not, and when not to use it.
- [ ] I preserve metadata on originals and strip it from copies I publish.

## Learn more

- **WITNESS — Activists' Guide to Archiving Video** — FREE-FULL, English (also Arabic, Spanish, Portuguese), no signup, about 45 minutes for the "Store", "Catalog" and "Preserve" stages: <https://library.witness.org/product/activists-guide-to-archiving-video/>. The PDF downloads from a third-party host (MediaFire). Watch for: file naming, metadata catalogues and how often to check storage. *Fallback:* Berkeley Protocol, ch. VI.D "Preservation", paras 157–175 (PDF, 20 minutes): <https://www.ohchr.org/sites/default/files/2024-01/OHCHR_BerkeleyProtocol.pdf>.
- **Microsoft Learn — Get-FileHash** — FREE-FULL, English, 10 minutes: <https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/get-filehash>. Read the description and the note on MD5 and SHA-1. *Fallback:* [sha256sum(1)](https://man7.org/linux/man-pages/man1/sha256sum.1.html) or [shasum on SS64](https://ss64.com/mac/shasum.html).

## What goes wrong

| Mistake | Consequence | How to fix | How to avoid |
|---|---|---|---|
| Editing or "re-saving" the original | Authenticity challenged; the hash no longer matches | Restore from the second copy; log what happened | Read-only originals; edit copies only |
| Sending evidence through a messaging app as a photo | The app compresses it and strips metadata | Re-send as a file; keep the original | Send files as documents, or via an encrypted link |
| Using `shasum` without `-a 256` | You recorded a SHA-1 value | Re-hash with SHA-256 and note the correction | Use the commands in this lesson |
| One copy only, on the phone | Lost or seized phone means lost evidence | Recover from cloud if possible | Two copies, two places, from day one |
| Archiving a page that names a private victim | Their identity stays online publicly | Ask the Archive to exclude it | Think before archiving |
| Publishing a photo with GPS data | Reveals the filmer's home | Remove the post; publish a stripped copy | Strip metadata from every published copy |

## Review

- Originals stay untouched in two places; every edit is a logged working copy with its own hash.
- SHA-256 with built-in tools: `Get-FileHash` (Windows), `shasum -a 256` (macOS), `sha256sum` (Linux); re-check with `-c` or a comparison and log the result.
- A chain of custody records every hand-over and the receiver's hash check.
- Save Page Now gives an independent, dated copy of a public page — not a substitute for your own capture, and not for pages that expose private victims.
- Preserve metadata on originals; strip it from copies you publish; and secure the whole collection as a sensitive database (Privacy Law s. 17).
