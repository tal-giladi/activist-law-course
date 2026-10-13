# Activist Law — Israeli sources by module

Researched 2026-10-12. Scope: M01–M12, M18, M19, plus Hebrew video lectures.

## How to read this file

Each source line has two tags.

Verification tag:
- ✅ means the page was opened by an automated fetch (WebFetch or curl), or by the in-app browser, and its title or content matched.
- ⚠️ means the page was not opened, was blocked, or its content (usually PDF text) could not be read. The URL itself came from official search results or from a page that was opened.

Access tag:
- **FREE-FULL**: free and complete, with no paywall.
- **FREE-LIMITED**: free, but limited in a way the line describes.
- **PAID/UNAVAILABLE**: these are listed in the "Not recommended" lines only.

Signup:
- Signup is noted wherever it is needed.
- National Digital Identity (הזדהות לאומית) means a free government login.

### Access warnings
- **Bot blocking.** www.gov.il and kolzchut.org.il return HTTP 403 (Cloudflare) to automated tools. Many of their pages were confirmed through the MediaWiki API, the in-app browser or search results instead. An automated link checker will report false failures on these two domains, so check them in a normal browser.
- **Pages that render empty.** main.knesset.gov.il HTML pages are built with JavaScript. A fetch gets an empty shell, so deep links on that site need a manual check.
- **Nevo (nevo.co.il).** Statute pages (`/law_html/...`) are free. Case-law pages (`/psika_html/...`) redirect to a login page and are **PAID**. Never assign Nevo case links. Use the Versa translation or the free Supreme Court search instead.
- **Volatile numbers.** Every fee, ceiling and threshold below is tagged **VOLATILE**:
  - FOI fees update every 1 October.
  - Court fees and the small-claims ceiling update every 1 January.
  - Amuta fees update in April.
  - Re-check each one before publishing.

### Volatile numbers at a glance (as of 2026-10-12)

| Item | Amount | Source and date |
|---|---|---|
| FOI request fee | ₪24 | FOI Fees Regulations on Wikisource, edited 5.10.2026 |
| FOI handling fee | ₪36/hour from the 4th hour | same |
| FOI pre-commitment cap | ₪180 | same (was ₪173 in Oct 2024, ₪178 in Oct 2025) |
| FOI page copying | ₪0.24/page | same |
| HCJ petition fee (בג"ץ) | ₪2,144 | Court Fees Regulations, item 24, Wikisource, 2026 indexation (ק"ת תשפ"ו 12149) |
| Administrative petition fee (עתירה מינהלית) | ₪2,329 | same, item 20; confirmed by Kovetz Takanot 12149 (25.12.2025) |
| Administrative appeal fee (ערעור מינהלי) | ₪1,654 | Kovetz Takanot 12149 |
| Administrative petition deadline | 45 days | Administrative Courts (Procedure) Regulations, reg. 3 (court may extend) |
| Duty to decide on a written request | 45 days | Decisions and Reasons Law, s.2 |
| FOI answer deadline | 30 days, extendable by 30 | FOI Law, s.7(b) |
| Small claims ceiling | ₪39,900 | from 1.1.2026; Kol Zchut, and the Wikisource annotation to Courts Law s.60 |
| Small claims fee | 1% of the claim, minimum ₪50 | Kol Zchut, Jan 2026 |
| Legal aid income test (state) | ₪9,225 gross/month for 1–3 people; +₪826 per extra person | Kol Zchut, "2026" |
| Legal aid asset test | ₪41,307 | Kol Zchut, 2026. A gov.il snippet shows ₪39,948, probably older; resolve before publishing |
| Amuta annual fee (2026) | ₪1,777 regular; ₪1,338 if paid by 31.3.2026; ₪176 discounted | gov.il search extract; page itself not opened ⚠️ |
| Planning objection | 2 months from deposit publication (s.102), extendable to 3 months | Planning and Building Law; Kol Zchut gives 60 + 30 days |
| Appeals-committee appeal (ערר) against local-committee plan approval | 15 days | Kol Zchut |

---

## M01 — How Israeli law works (איך עובד המשפט הישראלי)

- [Foundations of Law Act 1980 — חוק יסודות המשפט, תש"ם-1980 (Hebrew Wikisource)](https://he.wikisource.org/wiki/חוק_יסודות_המשפט) — the two-section law. s.1 fills gaps in the law from "the principles of freedom, justice, equity and peace of Israel's heritage". Use it for the sources-of-law lesson: statute, then binding precedent, then analogy, then principles. — FREE-FULL, no signup — ✅
- [Courts Law [Consolidated Version] 1984 — חוק בתי המשפט [נוסח משולב], תשמ"ד-1984 (Hebrew Wikisource)](https://he.wikisource.org/wiki/חוק_בתי_המשפט) — full text, with amendments through תשפ"ו. Assign:
  - the Supreme Court chapter and s.15 (High Court of Justice jurisdiction);
  - s.20 (binding precedent);
  - the District and Magistrates' Court chapters;
  - s.60 (small claims);
  - s.68 (public hearings; see M19).
  The page is very long, so give learners the section number to search for. — FREE-FULL — ✅
- [Supreme Court of Israel — Wikipedia (EN)](https://en.wikipedia.org/wiki/Supreme_Court_of_Israel) — English background on the Supreme Court and its double role as the HCJ. — FREE-FULL — ⚠️
- [MFA: "The Judiciary: The Court System" (EN)](https://embassies.gov.il/MFA/AboutIsrael/state/Democracy/Pages/The%20Judiciary-%20The%20Court%20System.aspx) — English overview of the court levels, labour courts and religious courts. From about 2012, so money thresholds are stale. — FREE-FULL — ⚠️
- [Israel Law Review (Cambridge)](https://www.cambridge.org/core/journals/israel-law-review) — English scholarship. Gold open access from the 2025 volume, per a search snippet; earlier articles may be paywalled. — FREE-LIMITED — ⚠️
- [Nevo homepage — free extras](https://www.nevo.co.il/) — a Latin legal dictionary, tutorial videos and a citation-guide PDF are free. Use it as a glossary source. — FREE-LIMITED (extras only) — ✅

### Gaps
- **Official court-structure page.** gov.il returns 403 to bots. Open https://www.gov.il/he/departments/the_judicial_authority in a browser (slug unconfirmed). Go to "אודות", then "מבנה מערכת בתי המשפט", and copy the deep link.
- **Legal Hebrew glossary.** None verified. Candidates to check by hand:
  - Search the judiciary site for "מילון מונחים".
  - Search Kol Zchut for "מילון מונחים משפטיים".
  - Use Nevo's free Latin dictionary.
  - If none is usable, build the glossary in-house.
- **English Foundations of Law Act and Courts Law.** None found. Search WIPO Lex (wipo.int/wipolex, Israel) for both titles. If nothing comes up, teach from the Hebrew text with an English summary.
- **"How to read a statute or a ruling."** No free tutorial was found. Build it in-house, using the Wikisource pages above and a Versa opinion as live examples.

## M02 — Legal research & writing (מחקר וכתיבה משפטית)

- [ספר החוקים הפתוח — Open Law Book (Hebrew Wikisource index)](https://he.wikisource.org/wiki/ספר_החוקים_הפתוח) — an A–Z index of Israeli statutes and regulations, each in full text. This is the primary free statute source for the course. Wikisource can lag behind amendments, so cross-check against the Knesset database. — FREE-FULL — ✅
- [Knesset National Legislation Database — מאגר החקיקה הלאומי](https://main.knesset.gov.il/Activity/Legislation/Laws/Pages/LawHomePage.aspx) — the official database, with each law's history, Reshumot (official gazette) links and bills. Law pages use the pattern `LawPrimary.aspx?lawitemid=<id>`; 2000046 is Basic Law: Human Dignity and Liberty. — FREE-FULL — ⚠️ (the page is JavaScript-rendered and came back empty to the fetch)
- [Supreme Court website — אתר בית המשפט העליון](https://supreme.court.gov.il/) and [judgments search](https://supremedecisions.court.gov.il/) — free search of Supreme Court and HCJ judgments by case number or party name. Lower-court decisions are in Net HaMishpat. — FREE-FULL, no signup — ⚠️ (connection dropped to automated fetch)
- [Judiciary spokesperson's distributed rulings — פסקי דין שהופצו על ידי מערך הדוברות (gov.il)](https://www.gov.il/he/departments/dynamiccollectors/spokmanship_court) — curated notable rulings. — FREE-FULL — ⚠️ (403)
- [Versa — Cardozo Israeli Supreme Court Project](https://versa.cardozo.yu.edu/) — free English translations of landmark opinions, searchable and browsable by topic. Deep links are in M03, M04, M06 and M08. — FREE-FULL, no signup — ✅
- [Nevo — נבו](https://www.nevo.co.il/) — the commercial database.
  - Free: statute pages (`/law_html/`), tutorials, a citation-conventions PDF and a Latin dictionary.
  - Paid: case-law pages and full search.
  — FREE-LIMITED — ✅
- [Mishpatim — משפטים (Hebrew University law journal)](https://lawjournal.huji.ac.il/) — the main Hebrew law review. Article PDFs are hosted on the site and appear free; no access policy is stated. — FREE-FULL (probable) — ✅
- [Iyunei Mishpat forum — עיוני משפט, TAU](https://law.tau.ac.il/Law_Review/forum_1) — the online forum of the TAU law review. Archive access is unclear. — FREE-LIMITED? — ⚠️
- [Israel Democracy Institute — המכון הישראלי לדמוקרטיה](https://www.idi.org.il/) — policy papers. Many have a free PDF download ("הורדה חינם"); some books are sold. — FREE-LIMITED — ✅
- [Kol Zchut — affidavit (תצהיר)](https://www.kolzchut.org.il/he/תצהיר) — what an affidavit is and how it is signed before a lawyer. Use it for the affidavit-writing lesson. — FREE-FULL — ⚠️ (403)
- [MQG FOI administrative petition (.docx)](https://mqg.org.il/wp-content/uploads/2024/10/%D7%A2%D7%AA%D7%9E-35192-09-24-%D7%94%D7%AA%D7%A0%D7%95%D7%A2%D7%94-%D7%9C%D7%9E%D7%A2%D7%9F-%D7%90%D7%99%D7%9B%D7%95%D7%AA-%D7%94%D7%A9%D7%9C%D7%98%D7%95%D7%9F-%D7%A0-%D7%9E%D7%A9%D7%A8%D7%93-%D7%94%D7%A4%D7%A0%D7%99%D7%9D-%D7%95%D7%94%D7%95%D7%A2%D7%93%D7%94-%D7%9C%D7%97%D7%99%D7%95%D7%91-%D7%90%D7%99%D7%A9%D7%99.docx) — an editable model of legal-document structure (also used in M05). — FREE-FULL — ✅
- **Not recommended (paid/unavailable):**
  - Nevo case law and full search: PAID.
  - Takdin (תקדין): PAID.
  - Dinim ve'od (דינים ועוד): PAID.
  - dinrega.com: login-gated.

### Gaps
- **Uniform Citation Rules (כללי האזכור האחיד במשפט העברי).** No free PDF was found in two searches.
  1. Download the free citation-conventions PDF from the Nevo homepage and check whether it is the Uniform Rules or Nevo's own house style.
  2. Search Google for `"כללי האזכור האחיד" filetype:pdf`.
  3. Check the TAU and HUJI law-library guides (lawlib.tau.ac.il; the HUJI law library).
  4. If nothing turns up, teach a short in-house citation sheet.
- **Free judgment search deep link.** Open https://supremedecisions.court.gov.il/ in a browser, confirm the search-by-case-number form, and copy the URL.
- **Journals not checked.** Haifa Law Review (משפט וממשל / עיוני משפט חיפה), Hamishpat (המשפט, College of Management), and "המשפט ברשת". Search each site for "ארכיון גיליונות" and check that the PDFs open without login.
- **Legal letter and memo writing.** No free primary guide was found. On Kol Zchut, search "מכתב התראה" and "פנייה לרשות". Otherwise use the MQG petition and the Movement for FOI templates (M05) as models.

## M03 — Constitutional law & Basic Laws (משפט חוקתי וחוקי היסוד)

### Basic Laws: Hebrew full text and English translations

- **Basic Law: Human Dignity and Liberty**
  - [Hebrew — חוק יסוד: כבוד האדם וחירותו (Wikisource)](https://he.wikisource.org/wiki/חוק_יסוד:_כבוד_האדם_וחירותו) — full text, ss.1–12 including s.1A. — FREE-FULL — ✅
  - [English — Knesset PDF](https://main.knesset.gov.il/EN/activity/documents/BasicLawsPDF/BasicLawLiberty.pdf) — unofficial translation, amended to 2022. — FREE-FULL — ✅
- **Basic Law: Freedom of Occupation**
  - [Hebrew — חוק יסוד: חופש העיסוק (Wikisource)](https://he.wikisource.org/wiki/חוק_יסוד:_חופש_העיסוק) — full text, ss.1–11. — FREE-FULL — ✅
  - [English — Knesset PDF](https://main.knesset.gov.il/EN/activity/documents/BasicLawsPDF/BasicLawOccupation.pdf) — FREE-FULL — ✅ (PDF loads; title not machine-read)
- **Basic Law: The Judiciary**
  - [Hebrew — חוק יסוד: השפיטה (Wikisource)](https://he.wikisource.org/wiki/חוק_יסוד:_השפיטה) — full text. It includes:
    - the 2025 (תשפ"ה) amendment to s.4 and the new ss.4A–4B (the Judicial Selection Committee), which take effect from the 26th Knesset;
    - s.15(ד1) marked as annulled by HCJ 5658/23.
    — FREE-FULL — ✅
  - [English — Knesset PDF](https://main.knesset.gov.il/EN/activity/documents/BasicLawsPDF/BasicLawTheJudiciary.pdf) — dated 2022, so it does **not** include the 2025 amendment. — FREE-FULL, outdated — ✅
- **Basic Law: Israel — the Nation-State of the Jewish People**
  - [Hebrew — חוק יסוד: ישראל – מדינת הלאום של העם היהודי (Wikisource)](https://he.wikisource.org/wiki/חוק_יסוד:_ישראל_–_מדינת_הלאום_של_העם_היהודי) — 11 sections, passed 19.7.2018. Note the en-dash in the URL. — FREE-FULL — ✅
  - [English — Knesset PDF](https://main.knesset.gov.il/EN/activity/documents/BasicLawsPDF/BasicLawNationState.pdf) — FREE-FULL — ✅ (PDF loads, metadata dated Jan 2025)

### Key cases

- [Kol Ha'am v. Minister of Interior, HCJ 73/53 — בג"ץ קול העם (Versa, EN)](https://versa.cardozo.yu.edu/opinions/kol-haam-co-ltd-v-minister-interior) — decided 16.10.1953, opinion by Agranat J. Use it for:
  - freedom of expression;
  - the "near certainty" test;
  - the Declaration of Independence as an aid to interpretation.
  — FREE-FULL — ✅
- [United Mizrahi Bank v. Migdal, CA 6821/93 — ע"א בנק המזרחי (Versa, EN)](https://versa.cardozo.yu.edu/opinions/united-mizrahi-bank-v-migdal-cooperative-village) — decided 9.11.1995. The "constitutional revolution" case on judicial review of statutes under the Basic Laws. It is very long, so assign excerpts from Barak P.'s opinion. — FREE-FULL — ✅
- [Ka'adan v. Israel Land Administration, HCJ 6698/95 — בג"ץ קעדאן (Versa, EN)](https://versa.cardozo.yu.edu/node/167) — decided 8.3.2000. Equality in allocating state land. Use the node link; the slug URL returns nothing. — FREE-FULL — ✅
- **Hasson v. Knesset, HCJ 5555/18 — בג"ץ חסון (Nation-State Law).** Decided 8.7.2021; upheld 10–1, Karra J. dissenting. Versa has no translation, only a [hearing livestream post](https://versa.cardozo.yu.edu/viewpoints/hcj-555518-akram-hasson-v-knesset-livestream). — ⚠️
  - [Adalah's English summary of the judgment](https://www.adalah.org/uploads/uploads/Translation_of_Summary_of_JNSL_Judgment.pdf) — from a petitioner NGO, so flag it as advocacy. — FREE-FULL — ⚠️
  - [Library of Congress Global Legal Monitor summary](https://www.loc.gov/item/global-legal-monitor/2021-07-27/israel-supreme-court-affirms-constitutionality-of-basic-law-israel-nation-state-of-the-jewish-people/) — neutral summary. — FREE-FULL — ⚠️ (403 to fetch)
- **Movement for Quality Government v. Knesset, HCJ 5658/23 — the reasonableness amendment, 1.1.2024.**
  - [Official English abstract with a summary of each justice's opinion (Versa)](https://versa.cardozo.yu.edu/node/704) — use this as the short reading. — FREE-FULL — ✅
  - [Hayut P.'s majority opinion in English (Versa)](https://versa.cardozo.yu.edu/opinions/movement-quality-government-israel-v-knesset) — FREE-FULL — ✅
  - Holding: 12 of 15 justices held that the Court may review Basic Laws in extreme cases; 8 of 15 voided the amendment.

### Judicial reform: status as of the latest sources found

- **Judicial Selection Committee amendment.** Passed 27.3.2025 with 67 votes, while the opposition boycotted.
  - It removes the two Bar Association members and increases coalition influence.
  - It takes effect only from the next (26th) Knesset.
  - The High Court issued a conditional order.
  - On 21.6.2026 an 11-justice panel heard six consolidated petitions. The question is whether this is an "unconstitutional constitutional amendment". The Attorney General supports the petitioners; the state says the challenge is premature.
  - **No ruling was found as of 12.10.2026.**
  - Sources:
    - [Jerusalem Post, 21.6.2026](https://jpost.com/israel-news/politics-and-diplomacy/article-900025) — ✅
    - [Wikipedia: 2025 Israeli judicial reform](https://en.wikipedia.org/wiki/2025_Israeli_judicial_reform) — ✅
    - [Ynet: High Court hears the petitions](https://www.ynetnews.com/article/ggpeg97lh) — ✅
    - [Wikipedia: 2023 Israeli judicial reform (background)](https://en.wikipedia.org/wiki/2023_Israeli_judicial_reform) — ✅
- **Attorney General dismissal.**
  - 23.3.2025: the cabinet passed a no-confidence vote in AG Gali Baharav-Miara.
  - August 2025: the cabinet changed the dismissal procedure (Resolution 3125) and fired her.
  - The Court froze the firing the same month.
  - 14.12.2025: a 7–0 panel, opinion by President Amit, voided the new procedure and the dismissal, so she remains in office. Ministers Levin and Karhi called for defiance.
  - No 2026 reversal was found.
  - Sources:
    - [Times of Israel, 14.12.2025](https://timesofisrael.com/high-court-annuls-firing-of-attorney-general-cabinet-ministers-urge-defiance-of-ruling/) — ✅
    - [Wikipedia: Gali Baharav-Miara](https://en.wikipedia.org/wiki/Gali_Baharav-Miara) — ✅
- **Not recommended (paid/unavailable):**
  - Bloomberg coverage: paywalled.
  - Israel Law Review articles before 2025: may be paywalled.

### Gaps
- **Official Hebrew judgments** for 5555/18, 5658/23 and the December 2025 AG ruling. Get them from https://supremedecisions.court.gov.il/ by case number. For 5658/23, Versa node/704 also links the Hebrew judgment.
- **Judicial Selection ruling after 21.6.2026.** Before publishing, search Times of Israel and idi.org.il for "Judicial Selection Committee ruling". If a ruling has come out, update this section.
- **English Basic Law: The Judiciary with the 2025 amendment.** The Knesset PDF predates it. Teach the amendment from the Hebrew Wikisource text.
- **IDI plain-language explainers.** Search idi.org.il for "הוועדה לבחירת שופטים" and "עילת הסבירות" and pick free articles.

## M04 — Administrative law principles (עקרונות המשפט המינהלי)

- [Administrative Procedure Amendment (Decisions and Reasons) Law 1958 — חוק לתיקון סדרי המינהל (החלטות והנמקות), תשי"ט-1958 (Wikisource)](https://he.wikisource.org/wiki/חוק_לתיקון_סדרי_המינהל_(החלטות_והנמקות)) — the duty to decide and to give reasons.
  - s.2: a written request must be decided and answered within 45 days.
  - s.6(b): silence counts as a refusal without reasons.
  - The Wikisource text of s.6(b) still says "three months". Check this against the Knesset text before teaching it.
  — FREE-FULL — ✅
- [Ressler v. Minister of Defence, HCJ 910/86 — בג"ץ רסלר (Versa, EN PDF)](https://versa.cardozo.yu.edu/sites/default/files/upload/opinions/Ressler%20v.%20Minister%20of%20Defense.pdf) — decided 12.6.1988, 126 pages. The leading case on broad public-petitioner standing and justiciability. Assign the editor's summary and the standing holding. — FREE-FULL — ✅
- [ACRI: "Standing" (זכות העמידה), 21.5.2017 (PDF)](https://law.acri.org.il/he/wp-content/uploads/2017/05/zchut-haamida-210517.pdf) — a 3-page Hebrew position paper on public-petitioner standing. — FREE-FULL — ✅
- [gov.il book chapter: "The Deri-Pinhasi rule" (הלכת דרעי-פנחסי), PDF](https://www.gov.il/BlobFolder/guide/book_75_chapters/he/%D7%94%D7%A4%D7%A8%D7%93%D7%AA%20%D7%A8%D7%A9%D7%95%D7%99%D7%95%D7%AA%20%D7%95%D7%93%D7%99%D7%A0%D7%99%20%D7%93%D7%9E%D7%95%D7%A7%D7%A8%D7%98%D7%99%D7%94.pdf) — Hebrew analysis of HCJ 3094/93 (Deri) and HCJ 4267/93 (Amitai, the Pinhasi case). Use it in place of the full judgments. — FREE-FULL — ✅
- [Versa: Movement for Quality Government v. PM Sharon, HCJ 1993/03 (EN)](https://versa.cardozo.yu.edu/opinions/movement-quality-government-israel-v-prime-minister-mr-ariel-sharon) — ministerial appointments; applies Deri-Pinhasi. — FREE-FULL — ⚠️
- [Versa commentary: "The Deri Appointment: Further Hearing Rules with Bite…"](https://versa.cardozo.yu.edu/viewpoints/deri-appointment-further-hearing-rules-bite-anti-corruption-rhetoric-without-teeth) — the 2023 Deri litigation, traced back to the 1993 rule. — FREE-FULL — ✅
- [Versa: "The Court's decision on reasonableness" (HCJ 5658/23)](https://versa.cardozo.yu.edu/viewpoints/courts-decision-reasonableness) — a bridge from Dapei Zahav to 2024. — FREE-FULL — ✅
- [Versa topic index: administrative law / reasonableness](https://versa.cardozo.yu.edu/taxonomy/term/190) — more English reading. — FREE-FULL — ✅
- [Dapei Zahav, HCJ 389/80 — בג"ץ דפי זהב נגד רשות השידור (Hebrew Wikipedia)](https://he.wikipedia.org/wiki/בג"ץ_דפי_זהב_נגד_רשות_השידור) — a summary of the reasonableness doctrine. The full text (פ"ד לה(1) 421) is on Nevo only, which is PAID. — FREE-FULL — ✅
- [The Deri-Pinhasi rule — הלכת דרעי-פנחסי (Hebrew Wikipedia)](https://he.wikipedia.org/wiki/הלכת_דרעי-פנחסי) — summarises HCJ 3094/93 (פ"ד מז(5) 404) and HCJ 4267/93 (פ"ד מז(5) 441). — FREE-FULL — ✅
- [Ressler — בג"ץ רסלר נגד שר הביטחון (Hebrew Wikipedia)](https://he.wikipedia.org/wiki/בג"ץ_רסלר_נגד_שר_הביטחון) and the [Versa HTML version of Ressler](https://versa.cardozo.yu.edu/opinions/ressler-v-minister-defence) — FREE-FULL — ✅
- Hebrew Wikipedia background articles. All FREE-FULL — ✅:
  - [Reasonableness — עילת הסבירות](https://he.wikipedia.org/wiki/עילת_הסבירות)
  - [Standing — זכות עמידה](https://he.wikipedia.org/wiki/זכות_עמידה) — links a free Kohelet e-book that criticises broad standing, which balances the ACRI paper.
  - [Administrative petition — עתירה מנהלית](https://he.wikipedia.org/wiki/עתירה_מנהלית)
- [Attorney General Guidelines database — הנחיות היועצת המשפטית לממשלה (gov.il)](https://www.gov.il/he/Departments/DynamicCollectors/legal-advisor-guidelines) — 243 guidelines, which can be filtered by chapter (for example "משפט מנהלי" or "חופש המידע"). Includes guideline 3.1200 on freedom of demonstration (see M06) and guideline 1.1555 on conflicts of interest. — FREE-FULL — ✅ (in-app browser)
- [AG legal opinions collection — חוות דעת מטעם היועמ"ש (gov.il)](https://www.gov.il/he/Departments/DynamicCollectors/legal-opinions-attorney-general) — FREE-FULL — ✅ (in-app browser)
- [State Attorney guidelines — הנחיות פרקליט המדינה (gov.il)](https://www.gov.il/he/Departments/DynamicCollectors/guidelines-state-attorney) — FREE-FULL — ⚠️ (403)
- **Not recommended (paid/unavailable):**
  - Nevo full text of the old rulings: PAID.
  - Quimbee case briefs: PAID.

### Gaps
- **Dapei Zahav, HCJ 389/80 (בג"ץ דפי זהב; reported at PD 35(1) 421).** No free full text and no Versa translation.
  - Try https://supremedecisions.court.gov.il/ with "389/80"; older rulings may be missing there.
  - Fallback: a public or university library Nevo terminal.
  - Otherwise, teach it through the reasonableness texts above.
- **Deri and Pinhasi full texts (3094/93 and 4267/93; PD 47(5) 404 and 441).** Same route as above. Until then, use the gov.il chapter.
- **AG guideline on the right to a hearing (זכות הטיעון).** Not yet located. In the AG database above, filter by the "משפט מנהלי" chapter and search "שימוע" and "זכות הטיעון".
- **Supreme Court free search coverage.** It covers rulings from about 1997 onward only. Older landmark rulings (Dapei Zahav, Deri, Pinhasi, and the Hebrew Ressler) need Versa, Wikipedia summaries, or a law library.
- **Right to a hearing and exhaustion of remedies (מיצוי הליכים).** No standalone free primer was verified. Search Kol Zchut for "זכות הטיעון" and "מיצוי הליכים". Otherwise write it in-house from Ressler and the ACRI standing paper.

## M05 — Administrative toolbox (ארגז הכלים המינהלי)

### Freedom of Information
- [Freedom of Information Law 1998 — חוק חופש המידע, התשנ"ח-1998 (Wikisource)](https://he.wikisource.org/wiki/חוק_חופש_המידע) — full text.
  - s.7(b): the authority must answer within 30 days, extendable by 30 more.
  - s.17: a petition goes to the Administrative Court, or to the Supreme Court if a secrecy certificate was issued.
  — FREE-FULL — ✅
- English translations:
  - [WIPO Lex entry](https://wipo.int/wipolex/en/legislation/details/15370) — unofficial 2014 translation. Link the entry page, because its PDF link expires. — FREE-FULL — ✅
  - [Cyrilla, section by section](https://cyrilla.org/en/entity/9k2ywjxyk8d) — FREE-FULL — ✅
- [FOI Fees Regulations 1999 — תקנות חופש המידע (אגרות), תשנ"ט-1999 (Wikisource)](https://he.wikisource.org/wiki/תקנות_חופש_המידע_(אגרות)) — **VOLATILE.** Edited 5.10.2026, current to ק"ת תשפ"ז 94.
  - Fees: request ₪24; handling ₪36/hour from the 4th hour; pre-commitment cap ₪180 (reg. 4(a)); ₪0.24 per page. Indexed every 1 October under reg. 7.
  - Reg. 6 exemptions: information about yourself, registered amutot and public-benefit companies, benefit recipients, and academic research.
  - Reg. 6A: an authority that missed the statutory deadline may not charge handling fees.
  — FREE-FULL — ✅
- [Official 2026 FOI fee notice — Kovetz Takanot 12538, 5.10.2026 (PDF)](https://olaw.org.il/takanot/takanot-12538.pdf) — the primary source for the FOI fees. — FREE-FULL — ✅
  - Amounts: request fee ₪24; handling fee ₪36/hour from the 4th hour (from the 8th hour if you are exempt); production ₪0.24/page or ₪3.01/CD; pre-commitment cap ₪180.
  - Previous year: [notice 12053 (Oct 2025)](https://olaw.org.il/takanot/takanot-12053.pdf), cap ₪178 — ✅
- [Government FOI Unit — fees page (אגרות חופש המידע)](https://www.gov.il/he/pages/fees_foi) — updated 5.10.2026 and matches the notice. It also states that an authority that missed its deadline may not charge handling fees. — FREE-FULL — ✅ (in-app browser)
- [Government FOI Unit landing page (foi.gov.il)](https://www.gov.il/he/departments/foi/govil-landing-page) — links to the officer search, an answers database, the annotated law, and a guide. — FREE-FULL — ✅ (in-app browser)
- FOI Unit sub-pages, linked from the landing page. All FREE-FULL — ⚠️ not opened:
  - [Officer search (חיפוש רשויות וממונים)](https://www.gov.il/he/Departments/DynamicCollectors/memunim-test)
  - [Answers database (מאגר התשובות)](https://www.gov.il/he/Departments/DynamicCollectors/repository-of-answers?skip=0)
  - [Annotated FOI law (החוק בראי הפסיקה)](https://www.gov.il/he/pages/annotated_foi_law)
  - [Guide to a good request (מדריך להגשת בקשה טובה)](https://www.gov.il/he/pages/foi_guide)
  - [Complaint to the FOI Unit](https://www.gov.il/he/service/freedom-of-information-complaint-submission) — the step before going to court.
  - [Recognition of an amuta for the fee exemption](https://www.gov.il/he/service/freedom-of-information-fees-exemptions)
- [Movement for FOI: "How to submit an information request" (איך להגיש בקשת מידע)](https://www.meida.org.il/submit-an-information-request) — how to find the FOI officer, the deadlines, reminders, the complaint step, and rebutting exemptions. Its fee figures (₪20 / ₪149) are out of date. — FREE-FULL — ✅
- **Note:** hofesh.org.il is a different organisation (one opposing religious coercion). The Movement for Freedom of Information is at **meida.org.il**.
- [Kol Zchut: filing an FOI request — הגשת בקשה לקבלת מידע לפי חוק חופש המידע](https://www.kolzchut.org.il/he/הגשת_בקשה_לקבלת_מידע_לפי_חוק_חופש_המידע) — practical walkthrough with links to the forms. Its fee figures still show October 2025 (₪178 cap). — FREE-FULL — ✅
- Government online request forms. Both need ID details and online payment. — FREE — ⚠️ (403)
  - [gov.il service: פנייה לקבלת מידע במסגרת חוק חופש המידע](https://www.gov.il/he/service/make-a-freedom-of-information-act-request)
  - [gov.il service: הגשת בקשת חופש המידע](https://www.gov.il/he/service/freedom_of_information_submission)
- [Government FOI Unit — היחידה הממשלתית לחופש המידע](https://www.gov.il/he/departments/units/freedom_of_information_supervisor) — supervises government bodies and takes complaints. — FREE — ⚠️ (403)
- [Government FOI procedure, Dec 2025 (PDF)](https://www.gov.il/BlobFolder/policy/regulation-4-1/he/freedom_of_information_procedure_foi_webpage_dec2025.pdf) — how ministries must handle requests. — FREE-FULL — ✅
- [Movement for Freedom of Information — התנועה לחופש המידע](https://www.meida.org.il/) — has a usage guide and a free-help contact form. Its latest item is a 29.9.2026 petition. — FREE-FULL — ✅
  - [Active petitions list (models)](https://www.meida.org.il/activities) — ✅
  - ["How to FOI" guide and template (PDF)](https://www.meida.org.il/wp-content/uploads/2007/11/how-to-FOI.pdf) — old fee amounts, but the process is still valid. — ✅

### Public Complaints Commissioner (נציב תלונות הציבור)
- [State Comptroller Law [Consolidated] — חוק מבקר המדינה, תשי"ח-1958 (Wikisource)](https://he.wikisource.org/wiki/חוק_מבקר_המדינה) — chapter 7 is ss.31–48:
  - s.33: anyone may complain;
  - s.36: which bodies a complaint can be against;
  - s.38: exclusions;
  - s.39(2): a one-year time limit.
  — FREE-FULL — ✅
- [Online complaint form](https://complaint.mevaker.gov.il/) ([English version](https://complaint.mevaker.gov.il/?lang=en)) and the [mevaker.gov.il complaints section](https://www.mevaker.gov.il/ombudsman) — FREE; the form is a JavaScript app, so it was not confirmed whether it needs signup — ✅
- [Kol Zchut: complaining to the Commissioner — הגשת תלונה לנציב תלונות הציבור (מבקר המדינה)](https://www.kolzchut.org.il/he/הגשת_תלונה_לנציב_תלונות_הציבור_(מבקר_המדינה)) — you can file orally, in writing, online or by post (POB 1081, Jerusalem 9101001). The one-year limit applies, and mediation is available. — FREE-FULL — ✅

### Courts, procedure, fees
- [Administrative Courts Law 2000 — חוק בתי משפט לעניינים מינהליים, התש"ס-2000 (Wikisource)](https://he.wikisource.org/wiki/חוק_בתי_משפט_לענינים_מינהליים) — First Schedule item 2 covers FOI decisions. — FREE-FULL — ✅
- [Administrative Courts (Procedure) Regulations — תקנות בתי משפט לעניינים מינהליים (סדרי דין), התשס"א-2000 (Wikisource)](https://he.wikisource.org/wiki/תקנות_בתי_משפט_לעניינים_מינהליים_(סדרי_דין)) — **reg. 3: 45 days (confirmed)**, unless another law sets a different deadline. The clock runs from the earliest of publication, notice or knowledge. The court may extend it (reg. 3(ג)). — FREE-FULL — ✅
- [HCJ Procedure Regulations — תקנות סדר הדין בבית המשפט הגבוה לצדק, התשמ"ד-1984 (Wikisource)](https://he.wikisource.org/wiki/תקנות_סדר_הדין_בבית_המשפט_הגבוה_לצדק) — **still in force**; the last amendments are from 2021.
  - reg. 2: Form 1 (the petition);
  - reg. 3: an Israeli address for service;
  - reg. 4: Form 2 (supporting affidavit);
  - reg. 21A: imports the 2018 Civil Procedure Regulations.
  — FREE-FULL — ✅
- [Court Fees Regulations — תקנות בתי המשפט (אגרות), התשס"ז-2007 (Wikisource)](https://he.wikisource.org/wiki/תקנות_בתי_המשפט_(אגרות)) — **VOLATILE, 2026 amounts:**
  - HCJ petition (item 24): **₪2,144**;
  - administrative petition (item 20): **₪2,329**;
  - indexed every 1 January under reg. 11;
  - reg. 14: exemption for inability to pay. It requires an affidavit on assets and 6 months of income, and the proceeding must show a cause of action;
  - reg. 19: parties exempt by status.
  — FREE-FULL — ✅
- [Official 2026 court-fee notice — Kovetz Takanot 12149, 25.12.2025 (PDF)](https://olaw.org.il/takanot/takanot-12149.pdf) — confirms the 2026 fees: administrative petition ₪2,329, HCJ petition ₪2,144, administrative appeal ₪1,654. **VOLATILE.** — FREE-FULL — ✅
- [gov.il: fee or deposit exemption request — בקשת פטור מתשלום אגרה או עירבון](https://www.gov.il/he/service/exempt_from_payment_of_a_fee) — FREE — ✅ (in-app browser)
  - Help: *3852, 077-2703333, or WhatsApp 050-6255727.
  - Form PDFs, not opened: [exemption-from-paying-fees.pdf](https://www.gov.il/BlobFolder/service/exempt_from_payment_of_a_fee/he/exemption-from-paying-fees.pdf) (named on the service page) and [exempt_from_payment_of_a_fee_2.pdf](https://www.gov.il/BlobFolder/service/exempt_from_payment_of_a_fee/he/exempt_from_payment_of_a_fee_2.pdf) (named by Kol Zchut) — ⚠️
- [Net HaMishpat — נט המשפט](https://www.court.gov.il/NGCS.Web.Site/HomePage.aspx) — the courts' e-filing system. Unrepresented people log in with National Digital Identity or a smart card. — FREE to use (court fees still apply) — ✅
- [Official judiciary guide: Net HaMishpat for parties without a lawyer — צדדים בתיק שלא מיוצגים בידי עו"ד](https://www.gov.il/he/pages/netlaw_guide_24?chapterIndex=3) — updated 17.9.2026. It covers filing through the "הגשות" (filings) tab or "הגשה מהירה" (quick filing), and reading your documents, and has a graphic PDF guide. The [main page of the guide (chapter 0)](https://www.gov.il/he/pages/netlaw_guide_24) covers login. — FREE-LIMITED (reading is free; filing needs a login) — ✅ (in-app browser)

### Model petitions to read
- [MQG FOI administrative petition, עת"מ 35192-09-24 (.docx)](https://mqg.org.il/wp-content/uploads/2024/10/%D7%A2%D7%AA%D7%9E-35192-09-24-%D7%94%D7%AA%D7%A0%D7%95%D7%A2%D7%94-%D7%9C%D7%9E%D7%A2%D7%9F-%D7%90%D7%99%D7%9B%D7%95%D7%AA-%D7%94%D7%A9%D7%9C%D7%98%D7%95%D7%9F-%D7%A0-%D7%9E%D7%A9%D7%A8%D7%93-%D7%94%D7%A4%D7%A0%D7%99%D7%9D-%D7%95%D7%94%D7%95%D7%A2%D7%93%D7%94-%D7%9C%D7%97%D7%99%D7%95%D7%91-%D7%90%D7%99%D7%A9%D7%99.docx) — an editable Word file. The best template in this list. — FREE-FULL — ✅
- Movement for FOI administrative petitions: [State Archives petition (PDF)](https://www.meida.org.il/wp-content/uploads/2021/03/State-Archives-petiton.pdf) and ["femi" petition (PDF, 2022)](https://www.meida.org.il/wp-content/uploads/2022/03/femi.pdf) — FREE-FULL — ✅
- [Movement for Quality Government — legal-action archive](https://mqg.org.il/legal-action/) — can be filtered to HCJ petitions or administrative petitions, for 2020–2026. — FREE-FULL — ✅
- ACRI petitions:
  - [ACRI English legal archive](https://law.acri.org.il/en/tag/legal-work/) — FREE-FULL — ✅
  - law.acri.org.il/he now redirects to acri.org.il, but the old PDF links still work. No current Hebrew petitions archive was found. — ⚠️
- [Regavim — Legal Library](https://www.regavim.org/publications/legal-library/) — petitions filed by a right-wing NGO, for balance. — FREE-FULL — ✅
- [HaMoked — advanced legal search](https://hamoked.org.il/adv_search.php) — HCJ petitions, responses and judgments, many in English. — FREE-FULL — ✅
- [HaMoked — המוקד להגנת הפרט](https://hamoked.org.il/) — HCJ petitions, including English documents. — FREE-FULL — ✅
- [Kohelet amicus brief, HCJ 8665/14 (PDF hosted by ACRI)](https://law.acri.org.il/he/wp-content/uploads/2015/02/hit8665kohelet-amicus.pdf) — a conservative-side filing, for balance. — FREE-FULL — ✅
- [Kohelet Policy Forum](https://kohelet.org.il/) and [Regavim](https://www.regavim.org/) — home pages only; no petition PDF was located. — FREE — ✅
- **Not recommended (paid/unavailable):** Nevo and Takdin full text: PAID.

### Gaps
- **FOI officer database (מאגר הממונים).** Open gov.il in a browser, search "ממונים על חופש המידע", and copy the DynamicCollectors URL. An earlier note gives https://www.gov.il/he/Departments/DynamicCollectors/memunim-test.
- **HCJ filing by a petitioner without a lawyer.** The Net HaMishpat guide above covers the Magistrates' and District Courts only, not the Supreme Court. Call *3852 (077-2703333, or WhatsApp 050-6255727) and ask: "How does an unrepresented petitioner file a בג"ץ petition — through Net HaMishpat or at the Supreme Court registry — and how is the fee paid?"
- **Reduced fee for FOI petitions.** None was found in the fee schedule, so item 20 (₪2,329) appears to apply. Confirm by calling *3852.
- **Movement for FOI templates.** None were found online; the site has only the guide. Email through https://www.meida.org.il/contact-us and ask for sample request, complaint and petition templates. Otherwise build them in-house from FOI Law s.7 and FOI Fees Regulations regs 6–7.
- **Fee-exemption page content.** Open the gov.il link above in a browser and record the eligibility list and the form fields.
- **Regavim and Kohelet petition PDFs.** Search each site for "עתירה", or find a docket number and pull the filing from supremedecisions.court.gov.il.

## M06 — Protest, expression & police (מחאה, ביטוי ומשטרה)

- [Police Ordinance [New Version] 1971 — פקודת המשטרה [נוסח חדש], תשל"א-1971 (Wikisource)](https://he.wikisource.org/wiki/פקודת_המשטרה) — chapter 6, part B, "Assemblies and processions":
  - s.83 definitions: 50 or more people;
  - s.84: the district commander may require a written licence application at least 5 days ahead;
  - s.85: the licence may be granted, granted with conditions, or refused;
  - s.87: cancelling a licence;
  - s.89: an unlicensed or condition-breaking event counts as an unlawful assembly.
  — FREE-FULL — ✅
- [Levi v. Commander of the Southern District, HCJ 153/83 — בג"ץ לוי (Versa, EN)](https://versa.cardozo.yu.edu/opinions/levi-v-commander-southern-district-israeli-police) — decided 13.5.1984; the anchor case for the module.
  - A ban needs a high probability of serious harm, based on real facts.
  - Reasonable policing measures must be tried first.
  - Versa's abstract says "near certainty" but the opinion says "substantial probability", so cite the opinion.
  — FREE-FULL — ✅
- [Majority Camp v. Israel Police, HCJ 2557/05 (Versa)](https://versa.cardozo.yu.edu/opinions/majority-camp-v-israel-police) — decided 12.12.2006. Police must secure protests and may not pass security costs to the organisers. — FREE-FULL — ✅
- [Dayan v. Wilk, HCJ 2481/93 (Versa)](https://versa.cardozo.yu.edu/opinions/dayan-v-wilk) — decided 9.2.1994. A protest outside a public figure's home, balanced against privacy. — FREE-FULL — ✅
- [Amit v. Southern District Police Commander (Versa)](https://versa.cardozo.yu.edu/opinions/amit-v-southern-district-police-commander) — protest licensing. The page loads; its case number was not checked. — FREE-FULL — ✅
- [Versa topic: freedom of assembly](https://versa.cardozo.yu.edu/topics/freedom-assembly) — FREE-FULL — ✅
- [Kol Zchut: no licence needed for rule-of-law and corruption protests — אין צורך בקבלת רישיון… (HCJ 6536/17, 8.10.2017)](https://www.kolzchut.org.il/he/אין_צורך_בקבלת_רישיון_מהמשטרה_כדי_לקיים_הפגנות_בנושא_שלטון_החוק,_שחיתות_שלטונית_וטוהר_מידות_של_נבחרי_ציבור) — the Petah Tikva protests outside the Attorney General's home. — FREE-FULL — ✅
- [Kol Zchut: getting a protest licence — הוצאת רישיון להפגנה](https://www.kolzchut.org.il/he/הוצאת_רישיון_להפגנה) — a licence is needed only for an outdoor event of 50+ people gathered for a political speech or lecture, or for a procession. Apply 5 days ahead. — FREE-FULL — ✅
- [Kol Zchut: megaphones, cameras and traffic — הזכות להשתמש במגפון ובמצלמות ולהפריע לתנועה במהלך הפגנה](https://www.kolzchut.org.il/he/הזכות_להשתמש_במגפון_ובמצלמות_ולהפריע_לתנועה_במהלך_הפגנה) — filming police is lawful, and an officer generally may not order you to stop. The page cites:
  - Police procedure 220.001.20 (16.6.2020);
  - National HQ order 12.01.06;
  - AG guideline 3.1200 "חירות ההפגנה" (Freedom of Demonstration).
  Use it for the filming-police lesson. — FREE-FULL — ✅
- [Kol Zchut: dispersal — פיזור הפגנה על ידי המשטרה](https://www.kolzchut.org.il/he/פיזור_הפגנה_על_ידי_המשטרה) and [detaining a protester — עיכוב מפגין](https://www.kolzchut.org.il/he/עיכוב_מפגין) — detention limit is 3 hours (6 in some cases), and the officer must identify themselves. — FREE-FULL — ✅
- [Kol Zchut: freedom of expression rulings — חופש הביטוי/פסקי דין](https://www.kolzchut.org.il/he/חופש_הביטוי/פסקי_דין) — a collection of ruling summaries. — FREE-FULL — ✅
- [ACRI Protest Guide — המדריך למחאה](https://protest.acri.org.il/) — the main practical handout. — FREE-FULL — ✅
- [ACRI "Know your rights" hub](https://www.acri.org.il/know-your-rights) — FREE-FULL — ✅
  - [Filming police (4.6.2023)](https://www.acri.org.il/post/__881) — ✅
- [ACRI guide "Contact with the Police" (זכותון מגע עם המשטרה), ch.14 "The right to protest"](https://law.acri.org.il/he/?p=20864) — from 2012, so check each rule against current sources. — FREE-FULL — ✅
- [IDI policy paper 198 (2024): "Freedom of protest and demonstration" (חופש המחאה וחופש ההפגנה)](https://www.idi.org.il/books/55013) and its [PDF](https://www.idi.org.il/media/24587/freedom-of-assembly-and-the-right-to-protest.pdf) — the best current overview of Israeli protest law. — FREE-FULL — ✅
- [Zulat (2024): "The Legal Infrastructure for the Suppression of Protests in Israel" (EN PDF)](https://en.zulat.org.il/wp-content/uploads/2024/05/The-Legal-Infrastructure-for-the-Supression-of-Protests-in-Israel.pdf) — an advocacy critique. — FREE-FULL — ✅
- [ACRI letter quoting AG guideline 3.1200 (2011, PDF)](https://law.acri.org.il/he/wp-content/uploads/2012/02/demonstrations281111.pdf) — a stand-in until the guideline itself is found. — FREE-FULL — ✅
- Police procedures (PDFs). Both load but are served as downloads and were not machine-read. — FREE — ✅ (loads)
  - [Procedure 220.001.20 — licensing assemblies](https://www.police.gov.il/menifa/90.220.001.20_1.pdf)
  - [HQ order 12.01.06](https://www.police.gov.il/menifa/02.12.01.06_1.pdf)
- [HCJ 8510/23 ruling (PDF, hosted by Adalah)](https://www.adalah.org/uploads/uploads/HCJ_8510_23_ruling.pdf) — 2023, wartime refusals of anti-war protests in Arab towns. The outcome is **not verified**. — ⚠️
- **Police complaints:**
  - [gov.il: complaint to the Police Investigations Department — הגשת תלונה למחלקה לחקירות שוטרים (מח"ש)](https://www.gov.il/he/service/filing_a_complaint_against_police) — the criminal route; hotline *2906. — FREE — ✅ (in-app browser)
  - [gov.il: Police Public Complaints Unit — היחידה לתלונות הציבור](https://www.gov.il/he/departments/guides/police_public_complaints_unit?chapterIndex=1) — the disciplinary route; updated 1.9.2026. — FREE — ✅ (in-app browser)
  - [ACRI: complaining to מח"ש about police violence](https://www.acri.org.il/post/__119) — evidence, testimony, and the 60-day appeal (ערר) deadline. — FREE-FULL — ✅
  - [ACRI: disciplinary complaints](https://www.acri.org.il/post/_1226) — FREE-FULL — ✅
  - [ACRI guide ch.18: criminal investigation of police](https://law.acri.org.il/he/?p=20877) and [ch.19: disciplinary proceedings](https://law.acri.org.il/he/?p=20880) — FREE-FULL — ✅
- **Not recommended (paid/unavailable):**
  - Nevo full text of HCJ 6536/17: PAID (login).
  - Old AG guideline PDF on justice.gov.il: UNAVAILABLE (now redirects to the gov.il home page).

### Gaps
- **AG guideline 3.1200 "חירות ההפגנה" (freedom of demonstration).** It is in the AG Guidelines database (https://www.gov.il/he/Departments/DynamicCollectors/legal-advisor-guidelines, ✅). Open the database in a browser, search "3.1200", and copy the PDF link. Until then, cite the ACRI 2011 letter.
- **Written police procedure on citizens filming police.** None is published. Say so in the lesson, and cite the Kol Zchut page and ACRI.
- **Recent protest rulings, 2020–2025.** Balfour/COVID (HCJ 6312/20, 5469/20) and HCJ 8510/23 and 8007/23. Read the outcomes on https://supremedecisions.court.gov.il/ by case number before citing. The Adalah PDF for 6312/20 is https://www.adalah.org/uploads/uploads/HCJ_6312_20_ruling.pdf (⚠️ not read).
- **English Police Ordinance.** None was found. Teach from the Hebrew text plus the Versa cases.

## M07 — Criminal law & procedure for activists (משפט פלילי וסדר דין)

- [Penal Law 1977 — חוק העונשין, תשל"ז-1977 (Wikisource)](https://he.wikisource.org/wiki/חוק_העונשין) — full text. These section headings were checked against the text:
  - Sedition, incitement and assembly:
    - s.133 sedition;
    - s.144ב incitement to racism;
    - s.144ד2 incitement to violence;
    - s.151 unlawful assembly;
    - s.152 riot;
    - s.153 dispersal order;
    - s.155 continuing a riot after a dispersal order.
  - Public order:
    - s.192 threats;
    - s.194 disturbance and insult in a public place;
    - s.196 defacing property (graffiti);
    - s.215 public nuisance;
    - s.216 improper conduct in a public place.
  - Police and officials:
    - s.273 assaulting a police officer;
    - s.275 and s.275א obstructing a police officer (basic and aggravated);
    - s.287 breach of a lawful order;
    - s.288 insulting a public servant.
  - Roads and safety:
    - s.332 endangering life on a traffic route (road blocking);
    - s.338 reckless or negligent acts.
  — FREE-FULL — ✅
- [Penal Law, English (ICJ-hosted PDF)](https://www.icj.org/wp-content/uploads/2013/05/Israel-Penal-Law-5737-1977-eng.pdf) — an older unofficial translation; its amendment level is unknown. — FREE-FULL — ✅ (loads)
- [Criminal Procedure (Enforcement Powers — Arrests) Law 1996 — חוק סדר הדין הפלילי (סמכויות אכיפה – מעצרים), תשנ"ו-1996 (Wikisource)](https://he.wikisource.org/wiki/חוק_סדר_הדין_הפלילי_(סמכויות_אכיפה_–_מעצרים)):
  - s.23: arrest without a warrant;
  - s.29: being brought before a judge;
  - s.32: explaining rights to the person arrested;
  - s.33: notifying a relative;
  - s.34: meeting a lawyer;
  - ss.67–71: short detention (עיכוב).
  — FREE-FULL — ✅
- [Public Defender Law 1995 — חוק הסניגוריה הציבורית (Wikisource)](https://he.wikisource.org/wiki/חוק_הסניגוריה_הציבורית) — eligibility is in s.18. — FREE-FULL — ✅
- [Criminal Information and Rehabilitation of Offenders Law 2019 — חוק המידע הפלילי ותקנת השבים, תשע"ט-2019 (Wikisource)](https://he.wikisource.org/wiki/חוק_המידע_הפלילי_ותקנת_השבים) — **this replaced the 1981 Criminal Register and Rehabilitation Law (חוק המרשם הפלילי ותקנת השבים)**, so lessons must use the 2019 name. The [1981 law page](https://he.wikisource.org/wiki/חוק_המרשם_הפלילי_ותקנת_השבים) is for history only. — FREE-FULL — ✅
- Kol Zchut rights pages. All FREE-FULL ✅. Start from the [criminal proceedings hub — אנשים בהליכים פליליים](https://www.kolzchut.org.il/he/אנשים_בהליכים_פליליים).
  - Arrest and detention:
    - [Arrest by a police officer — מעצר בידי שוטר](https://www.kolzchut.org.il/he/מעצר_בידי_שוטר): up to 24 hours without a warrant (48 in urgent cases).
    - [Remand for investigation — מעצר ימים (מעצר לצורך חקירה)](https://www.kolzchut.org.il/he/מעצר_ימים_%28מעצר_לצורך_חקירה%29): the remand-hearing lesson.
    - [Release on bail by an officer — חלופת מעצר בהחלטת קצין ממונה](https://www.kolzchut.org.il/he/חלופת_מעצר_בהחלטת_קצין_ממונה_%28שחרור_בערבות%29)
    - [Short detention — עיכוב](https://www.kolzchut.org.il/he/עיכוב)
    - [Police ID demands — שוטר רשאי לדרוש הצגת תעודת זהות…](https://www.kolzchut.org.il/he/שוטר_רשאי_לדרוש_הצגת_תעודת_זהות_אך_לא_רשאי_לבצע_פעולות_שיטור_נוספות_ללא_חשד_לביצוע_עבירה): links a December 2025 ruling, reportedly HCJ 244/23 (⚠️ unverified).
  - Rights during interrogation:
    - [Right to silence — זכות השתיקה במהלך חקירה](https://www.kolzchut.org.il/he/זכות_השתיקה_במהלך_חקירה)
    - [Consulting a lawyer in custody — התייעצות של אנשים במעצר עם עורך דין](https://www.kolzchut.org.il/he/התייעצות_של_אנשים_במעצר_עם_עורך_דין)
  - Public Defender:
    - [Public defender representation — ייצוג על ידי סניגור ציבורי בהליך פלילי](https://www.kolzchut.org.il/he/ייצוג_על_ידי_סניגור_ציבורי_בהליך_פלילי)
    - [The Public Defender's Office — הסניגוריה הציבורית](https://www.kolzchut.org.il/he/הסניגוריה_הציבורית)
  - Criminal records:
    - [Criminal record — מרשם פלילי](https://www.kolzchut.org.il/he/מרשם_פלילי)
    - [Viewing your own record — עיון של אדם במידע פלילי על עצמו](https://www.kolzchut.org.il/he/עיון_של_אדם_במידע_פלילי_%28מרשם_פלילי_או_משטרתי%29_על_עצמו)
    - [Deleting closed-case police records — ביטול רישום משטרתי של תיקים סגורים](https://www.kolzchut.org.il/he/ביטול_רישום_משטרתי_של_תיקים_סגורים)
    - [Limitation and deletion periods — תקופת ההתיישנות ותקופת המחיקה](https://www.kolzchut.org.il/he/תקופת_ההתיישנות_ותקופת_המחיקה_של_פרט_במרשם_הפלילי)
- [Public Defender — information for detainees (מידע לעצור), gov.il](https://www.gov.il/he/departments/guides/public_defender_public_information?chapterIndex=3) — official eligibility guide, updated 4.2.2026. — FREE-FULL — ✅ (in-app browser)
- [gov.il: online request for Public Defender representation](https://www.gov.il/he/service/request-for-representation-by-the-public-defender-office) — online form. District phones, Sun–Thu 08:00–16:00, **VOLATILE**:
  - Tel Aviv 073-3923600
  - Jerusalem 073-3926035
  - South 073-3922500
  - Haifa 073-3921001
  - North 073-3929801
  - Centre 073-3923555
  - National 073-3923500
  — FREE — ✅ (in-app browser)
- [ACRI: arrested at a protest — contacting the Public Defender (2020)](https://www.acri.org.il/post/__471):
  - Only people under arrest are eligible, not people briefly detained (מעוכבים).
  - The first consultation at the station is free.
  - Minors are always eligible.
  - Its phone numbers are from 2020, so check them against gov.il.
  — FREE-FULL — ✅
- [gov.il Israel Police: deleting closed-case records](https://www.gov.il/he/departments/general/police_criminal_information_closed_cases) — waiting periods. Updated 4.10.2026. — FREE — ✅ (in-app browser)
- ACRI guide "Contact with the Police" (2012), chapters. All FREE-FULL ✅; dated, so check against current sources:
  - [Ch.3 short detention (עיכוב)](https://law.acri.org.il/he/20302)
  - [Ch.4 arrest](https://law.acri.org.il/he/?p=20305)
  - [Ch.10 right to legal representation](https://law.acri.org.il/he/?p=20849)
  - [Ch.12 criminal record](https://law.acri.org.il/he/?p=20854)
  - [Guide index](https://law.acri.org.il/he/?p=20121)
- **Not recommended (paid/unavailable):** Nevo case pages: PAID (login).

### Gaps
- **English translations** of the Arrests Law, the 2019 Criminal Information Law and the Public Defender Law. None was found. Search WIPO Lex (Israel). If nothing exists, mark them "Hebrew only" in the course.
- **ACRI PDFs "tips for conduct at a protest and on arrest".** Open https://www.acri.org.il/post/__881 in a browser and copy the PDF links.
- **HCJ 244/23 (police ID checks, December 2025).** Confirm the date and holding on supremedecisions.court.gov.il before citing.

## M08 — Defamation, privacy, online speech (לשון הרע, פרטיות, ביטוי ברשת)

- [Prohibition of Defamation Law 1965 — חוק איסור לשון הרע, תשכ"ה-1965 (Wikisource)](https://he.wikisource.org/wiki/חוק_איסור_לשון_הרע) — the defences, with a direct anchor to [s.13](https://he.wikisource.org/wiki/חוק_איסור_לשון_הרע#סעיף_13):
  - s.13 permitted publications (פרסומים מותרים);
  - s.14 truth plus public interest (הגנת אמת הפרסום);
  - s.15 good faith (הגנת תום לב);
  - s.7א compensation without proof of damage.
  — FREE-FULL — ✅
- Kol Zchut defamation pages. All FREE-FULL ✅:
  - [Defamation hub — לשון הרע](https://www.kolzchut.org.il/he/לשון_הרע) and [its rulings collection](https://www.kolzchut.org.il/he/לשון_הרע/פסקי_דין)
  - The defences:
    - [Truth and public interest — פרסום שיש בו אמת ועניין ציבורי](https://www.kolzchut.org.il/he/פרסום_שיש_בו_אמת_ועניין_ציבורי_%28טענת_הגנה_לאדם_שהוגשה_נגדו_תביעה_בגין_פרסום_לשון_הרע%29)
    - [Good faith — פרסום בתום לב](https://www.kolzchut.org.il/he/פרסום_בתום_לב_%28טענת_הגנה_לאדם_שהוגשה_נגדו_תביעה_בגין_פרסום_לשון_הרע%29)
    - [Permitted publications — פרסומים מותרים](https://www.kolzchut.org.il/he/פרסומים_מותרים_החסינים_בפני_תביעת_לשון_הרע)
  - Bringing or facing a case:
    - [Civil defamation suit](https://www.kolzchut.org.il/he/הליך_משפטי_אזרחי_במקרה_של_פרסום_לשון_הרע_%28תביעה_לפיצוי_כספי%29)
    - [Private criminal complaint (קובלנה פלילית)](https://www.kolzchut.org.il/he/הליך_משפטי_פלילי_במקרה_של_פרסום_לשון_הרע_%28קובלנה_פלילית%29)
  - Online:
    - [Rights and duties online — מדריך זכויות וחובות בגלישה ברשת](https://www.kolzchut.org.il/he/מדריך_זכויות_וחובות_בגלישה_ברשת)
- [Anonymous v. Orbach, CFH 2121/12 (Versa, EN)](https://versa.cardozo.yu.edu/opinions/anonymous-v-orbach) — decided 18.9.2014, the further hearing of CA 751/10 (the Ilana Dayan "Uvda" case). It created the "responsible journalism" test inside the s.15 good-faith defence. This is the key case for activists who publish accusations. — FREE-FULL — ✅
- [Israel Electric Corp. v. Ha'aretz (Versa PDF, EN)](https://versa.cardozo.yu.edu/sites/default/files/upload/opinions/Israel%20Electric%20Corp.%20v.%20Ha%27aretz.pdf) — a classic case on criticism and good faith. — FREE-FULL — ✅
- [Versa topic: defamation](https://versa.cardozo.yu.edu/topics/defamation) — more English cases. The Versa opinion [Doe Co. v. Doe](https://versa.cardozo.yu.edu/opinions/doe-co-ltd-v-doe) cites Mor v. Barak, LCA 4447/07 (25.3.2010), where the majority refused to unmask an anonymous user. — FREE-FULL — ✅
- [Kol Zchut: "share" is publication, "like" is not (LCA 1239/19, 8.1.2020)](https://www.kolzchut.org.il/he/משתמשים_ששיתפו_%28share%29_פוסט_מכפיש_בפייסבוק,_חוייבו_בתשלום_פיצויים_לנפגע_בשל_פרסום_לשון_הרע) — the leading social-media defamation ruling. — FREE-FULL — ✅
- **Anti-SLAPP:**
  - **Status:** no anti-SLAPP statute is in force. Courts rely on the ss.13–15 defences, on striking out claims for abuse of process, and on costs awards.
  - [Bill P/6532/25 (Knesset PDF)](https://fs.knesset.gov.il/25/law/25_lst_11195949.pdf) — a private bill by MK Keti Shitrit, tabled 2.2.2026. It would:
    - cap compensation without proof of damage at ₪1,000 for an online comment;
    - add s.7ב, allowing costs and compensation against SLAPP plaintiffs.
    Its stage is unknown. — FREE-FULL — ✅
  - [IDI (2022): "SLAPP suits: characteristics, dangers and ways of coping" (תביעות השתקה), Hebrew PDF](https://www.idi.org.il/media/17839/slapps-characteristics-dangers-and-ways-of-contending-with-them.pdf) and [web PDF](https://en.idi.org.il/media/24575/slapps-characteristics-dangers-and-ways-of-contending-with-them_web.pdf) — FREE-FULL — ✅ (loads)
  - [Knesset Research and Information Center (ממ"מ): comparative review of anti-SLAPP laws (c.2020, PDF)](https://fs.knesset.gov.il/globaldocs/MMM/93b8b24e-ad0a-ea11-8102-00155d0aee38/2_93b8b24e-ad0a-ea11-8102-00155d0aee38_11_14983.pdf) — FREE-FULL — ✅
  - ACRI background PDFs: [2011 position paper on defamation amendments](https://law.acri.org.il/he/wp-content/uploads/2011/10/leshon-hara041011.pdf) and ["The Silencer" (2013)](https://law.acri.org.il/he/wp-content/uploads/2013/02/TheSilencer-mavo.pdf) — FREE-FULL — ✅
- [Protection of Privacy Law 1981 — חוק הגנת הפרטיות, תשמ"א-1981 (Wikisource)](https://he.wikisource.org/wiki/חוק_הגנת_הפרטיות) — consolidated with **Amendment 13** (ס"ח תשפ"ד 1430), which took effect 14.8.2025.
  - It introduces the term "personal information" (מידע אישי).
  - Chapter ד׳3 sets administrative fines.
  - The page was edited 12.10.2026.
  — FREE-FULL — ✅
- English: [WIPO Lex translation, 2014](https://www.wipo.int/wipolex/en/legislation/details/15372) — pre-Amendment 13. — FREE-FULL — ✅
- English: [Amendment 13, unofficial translation by the EBN law firm (.docx)](https://ebnlaw.co.il/wp-content/uploads/2024/09/Amendment-13-Israeli-Privacy-Law-non-formal-translation.docx) — FREE-FULL — ✅
- [Privacy Protection Authority — public complaints and inquiries (תלונות ופניות הציבור)](https://www.gov.il/he/Departments/General/public_inquiries_ilita) — online form, phone *3103, fax, post. Tagged "Amendment 13", updated 12.5.2026. — FREE — ✅ (in-app browser)
  - The complaint form it links: https://govforms.gov.il/mw/forms/ashrai3@justice.gov.il#!details1 — ⚠️
- [Kol Zchut: complaint to the Privacy Protection Authority](https://www.kolzchut.org.il/he/הגשת_תלונה_או_פנייה_אל_הרשות_להגנת_הפרטיות_בנושא_הגנת_הפרטיות_במאגרי_מידע) — a complaint leads to enforcement, not personal compensation. — FREE-FULL — ✅
- Kol Zchut privacy pages: [Protection of Privacy Law — חוק הגנת הפרטיות](https://www.kolzchut.org.il/he/חוק_הגנת_הפרטיות) and [the right to privacy — הזכות לפרטיות](https://www.kolzchut.org.il/he/הזכות_לפרטיות) — FREE-FULL — ✅
- [Library of Congress Global Legal Monitor, 17.11.2025: Amendment 13 in force](https://www.loc.gov/item/global-legal-monitor/2025-11-17/israel-amendment-to-privacy-protection-law-goes-into-effect/) — FREE — ⚠️
- **Not recommended (paid/unavailable):**
  - Nevo full texts of LCA 1239/19 and other defamation rulings: PAID.
  - gov.il/en/departments/legalInfo/priv_law: UNAVAILABLE (page not found).

### Gaps
- **Full texts of Mor v. Barak (LCA 4447/07) and LCA 1239/19.** Get them from https://supremedecisions.court.gov.il/ by case number.
- **Official Amendment 13 overview.** Open the Privacy Protection Authority page above in a browser and click "תיקון 13 לחוק הגנת הפרטיות" (the link goes to govextra.gov.il) and the Q&A at https://www.gov.il/he/pages/tikun13_qa.
- **Bill P/6532/25 stage.** Search main.knesset.gov.il bills for "6532" or "תביעות השתקה".
- **SLAPP ruling in the Nahal HaAsi / Kibbutz Nir David case.** Case number not verified. Search Kol Zchut "לשון הרע/פסקי דין" for "תביעת השתקה".
- **English Defamation Law.** None was found. Use the Versa Orbach opinion, which quotes ss.13–15 in English.

## M09 — Equality & anti-discrimination (שוויון ואיסור הפליה)

- [Equal Employment Opportunities Law 1988 — חוק שוויון ההזדמנויות בעבודה, התשמ"ח-1988 (Wikisource)](https://he.wikisource.org/wiki/חוק_שוויון_ההזדמנויות_בעבודה):
  - s.2: prohibition of discrimination;
  - s.9: the burden of proof shifts to the employer;
  - s.10: Labour Court jurisdiction and remedies;
  - ss.18א–18ח: the Commission.
  — FREE-FULL — ✅
  - English: [ICJ-hosted PDF](https://www.icj.org/wp-content/uploads/2013/05/Israel-Employment-Equal-Opportunities-Law-5748-1988-eng.pdf) — about 2008, so outdated. — FREE-FULL — ⚠️
- [Kol Zchut: Equal Employment Opportunities Commission — נציבות שוויון הזדמנויות בעבודה](https://www.kolzchut.org.il/he/נציבות_שוויון_הזדמנויות_בעבודה) — the Commission advises, mediates and can sue in the Labour Court. Phone 074-7696565. The law applies to employers with 6+ employees, except retaliation over sexual harassment, which covers all employers. — FREE-FULL — ✅
- [Online complaint form, Equal Employment Opportunities Commission (govforms)](https://govforms.gov.il/mw/forms/Shivion@moital.gov.il) — FREE; may require National Digital Identity — ✅
- [Commission unit page (gov.il)](https://www.gov.il/he/departments/Units/equal-opportunities-at-work-unit) — FREE — ⚠️ (403)
- [Prohibition of Discrimination in Products, Services and Entry into Places of Entertainment and Public Places Law 2000 — חוק איסור הפליה במוצרים, בשירותים ובכניסה למקומות בידור ולמקומות ציבוריים, התשס"א-2000 (Wikisource)](https://he.wikisource.org/wiki/חוק_איסור_הפליה_במוצרים,_בשירותים_ובכניסה_למקומות_בידור_ולמקומות_ציבוריים):
  - s.3: the prohibition;
  - s.4: discriminatory advertising;
  - s.5: up to ₪50,000 (indexed) without proof of damage;
  - s.6: evidentiary presumptions;
  - s.7: an organisation may sue.
  The page was last edited in 2020, so check for later amendments. — FREE-FULL — ✅
  - [Kol Zchut: discrimination in public places — איסור אפליה במקומות ציבוריים](https://www.kolzchut.org.il/he/איסור_אפליה_במקומות_ציבוריים) — FREE-FULL — ✅
  - [English Wikipedia summary](https://en.wikipedia.org/wiki/Prohibition_of_Discrimination_in_Products,_Services_and_Entry_into_Places_of_Entertainment_and_Public_Places_Law,_2000) — background only; no statute text. — FREE-FULL — ✅
- [Equal Rights for Persons with Disabilities Law 1998 — חוק שוויון זכויות לאנשים עם מוגבלות, התשנ"ח-1998 (Wikisource)](https://he.wikisource.org/wiki/חוק_שוויון_זכויות_לאנשים_עם_מוגבלות):
  - Chapter ה׳1: accessibility;
  - s.19ג: discrimination;
  - s.19נא(ב): up to ₪50,000 without proof of damage;
  - ss.20–26: the Commission;
  - s.12: right to sue in employment.
  The page is very long. — FREE-FULL — ✅
  - English: [UN DESA PDF](https://social.desa.un.org/sites/default/files/migrated/15/2019/11/Israel_The-Equal-Rights-of-Persons-with-Disabilities-Law-5758-1998.pdf) — version unknown. — FREE-FULL — ⚠️
  - [Kol Zchut: Commission for Equal Rights of Persons with Disabilities — נציבות שוויון זכויות לאנשים עם מוגבלות](https://www.kolzchut.org.il/he/נציבות_שוויון_זכויות_לאנשים_עם_מוגבלות) — public line *6763. — FREE-FULL — ✅
  - [gov.il: disability discrimination or inaccessibility complaint](https://www.gov.il/he/service/complaint_discrimination_inaccessibility_people_with_disabilities) — *6763, fax 02-6462881, POB 34255 Jerusalem. — FREE — ⚠️ (403)
  - [gov.il: accessibility query service](https://www.gov.il/he/service/accessibility_query_people_with_disabilities) — FREE — ⚠️ (403)
- [Women's Equal Rights Law 1951 — חוק שיווי זכויות האשה, התשי"א-1951 (Wikisource)](https://he.wikisource.org/wiki/חוק_שיווי_זכויות_האשה):
  - s.1א: one law for women and men;
  - s.1ב: affirmative action;
  - s.6: equal social rights;
  - s.6ב: protection from violence;
  - s.6ג: representation of women in public bodies.
  Amendment notes run to 2024. — FREE-FULL — ✅
  - English, historical: [Wikipedia, with the 1951 text](https://en.wikipedia.org/wiki/Women%27s_Equal_Rights_Law_of_Israel_(1951)) — not current; the 2000 amendment rewrote most of the law. — ✅
  - English: [LSE PDF of Amendment No. 4 (2005)](https://www.lse.ac.uk/women-peace-security/assets/documents/NAPS-Website/6.Policy/2005-Israel-Equality-of-Womens-Rights-Law-5765-2005-Amendment-No.-4-English-translation-Israel-2005.pdf) — ⚠️
- **Not recommended (paid/unavailable):** none.

### Gaps
- **Current English translations.** None found. Tell learners that the English versions are unofficial and outdated and that the Hebrew text governs.
- **Class Actions Law, Second Schedule, discrimination item.** Not verified. Open https://he.wikisource.org/wiki/חוק_תובענות_ייצוגיות, find "התוספת השנייה", and quote the item number exactly.
- **gov.il complaint pages.** Open each in a browser and confirm whether the form needs a National Digital Identity login.

## M10 — Planning, land, environment (תכנון, קרקע וסביבה)

- [Planning and Building Law 1965 — חוק התכנון והבניה, התשכ"ה-1965 (Wikisource)](https://he.wikisource.org/wiki/חוק_התכנון_והבניה) — the page is very large, so use the anchor `#סעיף_100`.
  - Objections:
    - **s.100**: who may object. Anyone with an interest in land, a building or another planning detail who considers themselves harmed, plus public and professional bodies the Interior Minister has approved.
    - **s.102**: the deadline is 2 months from publication of the deposit; the planning body may extend it to at most 3 months.
    - s.103: where to file.
    - s.106: hearing the objection.
  - Appeals:
    - s.12ב: powers of the appeals committee (ועדת ערר);
    - s.110: appeal to the National Council;
    - s.111: appeal from an appeals committee to the district committee.
  — FREE-FULL — ✅
  - English: [Adalah PDF](https://www.adalah.org/uploads/oldfiles/Public/files/Discriminatory-Laws-Database/English/07-National-Planning-Building-Law-1965.pdf) — old and unofficial. — FREE-FULL — ⚠️
- [Kol Zchut: filing an objection to a building plan — הגשת התנגדות לתוכנית בניה](https://www.kolzchut.org.il/he/הגשת_התנגדות_לתוכנית_בניה) — the best walkthrough.
  - Objecting is free; the window is 60 days, extendable by 30.
  - Hearing: at least 14 days' notice.
  - Appeal against a local-committee approval: to the district appeals committee within 15 days.
  - Appeal against a district-committee approval: ask the chair for leave within 15 days, then appeal to the National Council within 30 days.
  - An appeal (ערר) carries a fee.
  - Cites CA 2962/97: prima facie harm is enough to object.
  — FREE-FULL — ✅
- [Planning and Building (Procedure in Appeals Committees) Regulations — תקנות התכנון והבניה (סדרי הדין בועדות ערר) (Wikisource)](https://he.wikisource.org/wiki/תקנות_התכנון_והבניה_(סדרי_הדין_בועדות_ערר)) — FREE-FULL — ⚠️
- [Mavat — מבא"ת, the national plan search](https://mavat.iplan.gov.il/) — deposited plans, documents and deadlines. Online objections to district plans are filed here. — FREE-FULL, no signup to browse — ✅ (JavaScript app)
- [gov.il: online objection to Planning Administration plans — הגשת בקשת התנגדות לתוכנית](https://www.gov.il/he/service/filing-objection) — requires National Digital Identity. Objection files are published, so keep private details out of them. — FREE — ⚠️ (403)
- [gov.il: filing an appeal to an appeals committee — הגשת ערר לוועדת ערר לתכנון ובניה](https://www.gov.il/he/service/licensing-appeal-submission) — National Digital Identity login; fee payable. — ⚠️ (403)
- [gov.il district committees and appeals-committees directory](https://www.gov.il/he/departments/topics/district_planning_1) — ⚠️ (403)
- [Bimkom — במקום, Planners for Planning Rights](https://www.bimkom.org/) — planning-rights NGO. — FREE-FULL — ✅ (home page)
  - [Archives](https://www.bimkom.org/archives) — real objection letters to use as models.
  - [Ma'ale Adumim objection (2025, PDF)](https://bimkom.org/media/pages/archives/6f5ca3f7f4-1766584168/obj-420_1_7_59_2-maale-adomim-c-2025-heb.pdf) — ⚠️
  - [Bimkom YouTube channel](https://www.youtube.com/@bimkomplannersforplanningr1623) — ⚠️
- [Adam Teva V'Din — אדם טבע ודין](https://adamteva.org.il/) — environmental NGO. — FREE-FULL — ✅ (home page)
  - [Sample s.100 objection, April 2024 (PDF)](https://adamteva.org.il/wp-content/uploads/2024/05/התנגדות-לתכניות-507-0915108-ו-507-0973057-אדם-טבע-ודין-21.4.24.pdf) — ⚠️
- [Clean Air Law 2008 — חוק אוויר נקי, התשס"ח-2008 (Wikisource)](https://he.wikisource.org/wiki/חוק_אוויר_נקי):
  - s.3: prohibition of air pollution;
  - s.8: the public's right to air data;
  - s.21: public participation — anyone may comment on a draft emission permit within 45 days;
  - s.70: pollution is a civil wrong (tort);
  - s.71: environmental bodies may sue.
  — FREE-FULL — ✅
  - English: [FAOLEX PDF](https://faolex.fao.org/docs/pdf/isr219536E.pdf) and [UNEP LEAP record](https://leap.unep.org/en/countries/il/national-legislation/clean-air-law-2008) — reflect the 2012 amendment. — ⚠️
- [Prevention of Environmental Hazards (Civil Claims) Law 1992 — חוק למניעת מפגעים סביבתיים (תביעות אזרחיות), התשנ"ב-1992 (Wikisource)](https://he.wikisource.org/wiki/חוק_למניעת_מפגעים_סביבתיים_(תביעות_אזרחיות)) — this law lets a citizen sue a polluter. ([Nevo copy of the statute](https://www.nevo.co.il/law_html/law01/251_002.htm), free.)
  - s.2: an injunction suit by anyone harmed or likely to be harmed;
  - s.5: 60 days' prior notice to the polluter and the Minister;
  - s.6 and Schedule: standing for listed NGOs (Adam Teva V'Din, SPNI, Zalul and others);
  - s.10: group claim.
  — FREE-FULL — ✅
- [Kol Zchut: group claim over an environmental hazard — הגשת תובענה קבוצתית לטיפול במפגע סביבתי](https://www.kolzchut.org.il/he/הגשת_תובענה_קבוצתית_לטיפול_במפגע_סביבתי) — FREE-FULL — ✅
- [Class Actions Law 2006 — חוק תובענות ייצוגיות, התשס"ו-2006 (Wikisource)](https://he.wikisource.org/wiki/חוק_תובענות_ייצוגיות):
  - Second Schedule item 6: a claim over an environmental hazard against whoever causes it;
  - s.4(a)(3): an organisation may file when it would be hard for an individual to do so.
  — FREE-FULL — ✅
- Kol Zchut environment pages. All FREE-FULL ✅:
  - [Clean air and air pollution — אוויר נקי ומניעת זיהום אוויר](https://www.kolzchut.org.il/he/אוויר_נקי_ומניעת_זיהום_אוויר) — where and how to complain.
  - [Ministry of Environmental Protection — המשרד להגנת הסביבה](https://www.kolzchut.org.il/he/המשרד_להגנת_הסביבה) — 24/7 hotline *6911 / 1-222-6911; public inquiries 073-2733351.
- [Real-time air-quality data (air.sviva.gov.il)](https://air.sviva.gov.il/) — exercise: pull data for your area. — FREE-FULL — ✅
- Further pages (all ⚠️, 403):
  - [Kol Zchut: complaining about an environmental hazard](https://www.kolzchut.org.il/he/הגשת_תלונה_על_מפגע_סביבתי_לרשויות)
  - [Kol Zchut: private suit against polluters](https://www.kolzchut.org.il/he/הגשת_תביעה_פרטית_נגד_מזהמים)
  - [gov.il: Ministry public-inquiries guide](https://www.gov.il/he/departments/guides/moep_public_inquiries?chapterIndex=2)
  - [gov.il: report a noise hazard](https://www.gov.il/he/service/report_noise_hazard)
  - [gov.il: Green Police](https://www.gov.il/he/departments/units/green_police_dept)
- **Not recommended (paid/unavailable):**
  - Nevo full text of CA 2962/97: PAID.
  - Bimkom's old `/wp-content/uploads/` info sheet: UNAVAILABLE (404 since the site moved).

### Gaps
- **Bimkom objection info sheet ("דף מידע התנגדות לתכנית").** Search bimkom.org/archives, or email bimkom@bimkom.org for the current version.
- **Ministry of Environmental Protection public-participation page.** Not found. Search gov.il for "המשרד להגנת הסביבה שיתוף ציבור".
- **Group-claim routes.** Teach both the 1992 s.10 group claim and the 2006 Class Actions Law route. Add a line that which one applies should be checked with a clinic.

## M11 — Civil litigation for self-represented people (התדיינות אזרחית בלי עורך דין)

- [Civil Procedure Regulations 2018 — תקנות סדר הדין האזרחי, התשע"ט-2018 (Wikisource)](https://he.wikisource.org/wiki/תקנות_סדר_הדין_האזרחי) — in force since 1.1.2021, amended to 2025. Verified provisions:
  - Principles:
    - regs 1–5: purposes and principles;
    - reg 3: good faith;
    - reg 4: abuse of process.
  - Pleadings:
    - reg 9: statement of claim and defence. The defence is due within 60 days. A Magistrates' Court claim has a 2-page summary and 9 pages of detail.
    - reg 10: the heading, including the fee or the exemption relied on;
    - reg 29: objections to jurisdiction. It is **not** a pre-action letter; no general pre-action letter rule was found.
  - Hearings:
    - regs 34–37: preliminary meeting between the parties and the מהו"ת meeting;
    - regs 61–63: pre-trial.
  - Costs and service:
    - regs 151–157: costs (reg 157 is security for costs);
    - regs 158–169: service.
  — FREE-FULL — ✅
- [gov.il: Q&A on the 2018 regulations (PDF)](https://www.gov.il/BlobFolder/guide/guide_to_civil_procedure_01012021/he/commonqa.pdf) — FREE-FULL — ⚠️ (text not read)
- [Courts Law, s.60 (small claims), Wikisource](https://he.wikisource.org/wiki/חוק_בתי_המשפט) — small claims are open to individuals only. The annotation reads "in 2026, ₪39,900". — FREE-FULL — ✅
- [Courts (Small Claims Procedure) Regulations 1976 — תקנות שיפוט בתביעות קטנות (סדרי דין), התשל"ז-1976 (Wikisource)](https://he.wikisource.org/wiki/תקנות_שיפוט_בתביעות_קטנות_(סדרי_דין)):
  - reg 3: the claim; from 11.4.2025 it must include email and a mobile number;
  - reg 6: fees;
  - reg 13: the court actively investigates, and may hear by video or decide on the papers;
  - reg 16: appeal.
  — FREE-FULL — ✅
- [Kol Zchut: filing a small claim — הגשת תביעה קטנה](https://www.kolzchut.org.il/he/הגשת_תביעה_קטנה) — **VOLATILE:**
  - ceiling ₪39,900 (Jan 2026);
  - fee 1% of the claim, minimum ₪50;
  - online filing from a computer only, PDFs up to 30 MB;
  - links to the claim form and the fee-exemption form.
  — FREE-FULL — ✅
- [gov.il: file a small claim](https://www.gov.il/he/service/filing_a_small_claim) and [small claims guide](https://www.gov.il/he/pages/small_claims_courts_guide?chapterIndex=2) — official. Filing needs National Digital Identity. — FREE — ⚠️ (403)
- gov.il civil forms. All ⚠️ (403):
  - [Statement of claim (expedited procedure)](https://www.gov.il/he/service/filing-a-statement-of-claim)
  - [Statement of defence](https://www.gov.il/he/service/filing-letter-of-defense)
  - [Appeal or leave to appeal in civil proceedings](https://www.gov.il/he/service/appeal-or-requesting-leave-to-appeal-in-civil-proceedings)
  - [Update contact details in a court file](https://www.gov.il/he/service/request-update-contact-details-in-court-file)
- [Net HaMishpat — נט המשפט](https://www.court.gov.il/NGCS.Web.Site/HomePage.aspx) — e-filing and case tracking with National Digital Identity. Judiciary information centre: **\*3852 / 077-2703333** (chat and email too; Friday 08:00–12:30). — FREE — ✅
- [Protocol: Net HaMishpat explainer (commercial site)](https://protocol.co.il/net-court/) — FREE-FULL — ⚠️
- Fee exemption (פטור מאגרה): Court Fees Regulations, reg. 14 (see M05).
  - [Kol Zchut: exemption from a court fee or security deposit](https://www.kolzchut.org.il/he/פטור_מתשלום_אגרה_או_מהפקדת_ערבון_בהגשת_תביעה_לבית_המשפט_או_לבית_הדין) — FREE-FULL — ⚠️ (403)
- [Kol Zchut: free state legal aid — סיוע משפטי חינם מטעם משרד המשפטים](https://www.kolzchut.org.il/he/סיוע_משפטי_חינם_מטעם_משרד_המשפטים) — **VOLATILE, 2026:**
  - Income test: up to ₪9,225 gross a month for 1–3 people, plus ₪826 for each additional person.
  - Assets test: up to ₪41,307.
  - You must also show a legal chance of success.
  - Covered matters **include representation in administrative petitions and HCJ petitions**, as well as money claims, defamation, housing, employment and National Insurance.
  — FREE-FULL — ✅
- [Kol Zchut: applying for legal aid — הגשת בקשה לסיוע המשפטי](https://www.kolzchut.org.il/he/הגשת_בקשה_לסיוע_המשפטי_ממשרד_המשפטים) — FREE-FULL — ✅
  - How to apply: the [online form (govforms)](https://govforms.gov.il/mw/forms/LegalAid@justice.gov.il#!details) (⚠️), phone *6405 (Sun–Thu 8:00–16:00), or a district office by appointment.
  - [Legal Aid public-inquiries form](https://publicinquiries.justice.gov.il/) — ✅
- [gov.il: legal aid application](https://www.gov.il/he/service/legal_aid_application) and the [economic eligibility guideline 1.1.0001 (PDF)](https://www.gov.il/BlobFolder/service/legal_aid_application/he/1.pdf) — ⚠️ (403)
- [Kol Zchut: "Schar Mitzva" Bar Association pro bono — שכר מצווה](https://www.kolzchut.org.il/he/שכר_מצווה_–_סיוע_משפטי_בהתנדבות_למעוטי_אמצעים) — an option for people just above the state thresholds. — FREE-FULL — ⚠️ (403)
- **Not recommended (paid/unavailable):** Nevo and Takdin case law: PAID.

### Gaps
- **Legal aid asset cap.** Kol Zchut gives ₪41,307; a gov.il snippet gives ₪39,948. Open the gov.il legal_aid_application page and use the figure it marks "2026".
- **Official Net HaMishpat registration guide for unrepresented parties.** Not found. Call \*3852 and ask for the link, or check "מדריכים" inside Net HaMishpat.
- **Official 2026 minimum small-claims fee.** Check the judiciary fee-table PDF (https://www.gov.il/BlobFolder/generalpage/fees_3/he/8869-11-19_fees_8869-11-19_fees_scf1126.pdf, not fetched), or call \*3852.
- **Typical costs awards.** Not available. Teach the principle from regs 151–157 and say amounts are at the judge's discretion. Do not quote numbers.

## M12 — Knesset & local government (הכנסת והשלטון המקומי)

- [Knesset Law 1994, ch.12 "Lobbyists" — חוק הכנסת, התשנ"ד-1994, פרק י"ב שדלנים (Wikisource)](https://he.wikisource.org/wiki/חוק_הכנסת) — ss.65–71:
  - s.66: a lobbyist needs a House Committee permit and must list clients;
  - s.68: badge and disclosure of the client;
  - s.69: prohibited conduct;
  - s.70: a public register of lobbyists.
  An activist working for their own cause is generally not a "lobbyist", but check the s.65 definition. — FREE-FULL — ✅
- [IDI: "Citizens in Knesset Committees" (אזרחים בוועדות הכנסת), 2010](https://idi.org.il/parliaments/11110/11125) — there are two ways to appear before a committee: by invitation, or by your own request, which is rarely refused. Background for the position-paper lesson. — FREE-FULL — ✅
- [Open Knesset — הכנסת הפתוחה](https://oknesset.org) — MKs, committees, protocols and votes from Knesset open data, refreshed daily. — FREE-FULL — ✅
- [Knesset Channel — ערוץ כנסת](https://www.knesset.tv) — live broadcasts and recordings of plenum and committee sessions. — FREE-FULL — ✅
- [Knesset legislative process explainer (PDF)](https://m.knesset.gov.il/Activity/Legislation/Documents/Explanation2.pdf) — about 40 pages. Title not confirmed. — FREE-FULL — ⚠️
- [Knesset Rules of Procedure — תקנון הכנסת (PDF)](https://m.knesset.gov.il/Activity/Documents/RulesOfProcedure.pdf) — bill stages, parliamentary questions and committees. — FREE-FULL — ⚠️
- [Knesset Research and Information Center — מרכז המחקר והמידע (ממ"מ)](https://main.knesset.gov.il/Activity/Info/MMM/Pages/default.aspx) — research reports for MKs. A sample report is the anti-SLAPP review in M08. — FREE-FULL — ⚠️ (JavaScript page)
- [ACRI "Open Democracy" report (PDF)](https://law.acri.org.il/he/wp-content/uploads/2016/03/open-democracy0216.pdf) — barriers to public participation. — FREE-FULL — ⚠️
- Local government: [Kol Zchut: complaints to the Public Complaints Commissioner (covers local authorities)](https://www.kolzchut.org.il/he/הגשת_תלונה_לנציב_תלונות_הציבור_(מבקר_המדינה)) — FREE-FULL — ✅
- Further Kol Zchut pages. All FREE-FULL ⚠️ (403):
  - [Reasoned reply to public inquiries — קבלת תשובה מנומקת על פניות הציבור](https://www.kolzchut.org.il/he/%D7%A7%D7%91%D7%9C%D7%AA_%D7%AA%D7%A9%D7%95%D7%91%D7%94_%D7%9E%D7%A0%D7%95%D7%9E%D7%A7%D7%AA_%D7%A2%D7%9C_%D7%A4%D7%A0%D7%99%D7%95%D7%AA_%D7%94%D7%A6%D7%99%D7%91%D7%95%D7%A8_%D7%9C%D7%A8%D7%A9%D7%95%D7%99%D7%95%D7%AA_%D7%A6%D7%99%D7%91%D7%95%D7%A8%D7%99%D7%95%D7%AA)
  - [Local authorities must run an information website — רשויות מקומיות מחויבות להפעיל אתר אינטרנט](https://www.kolzchut.org.il/he/%D7%A8%D7%A9%D7%95%D7%99%D7%95%D7%AA_%D7%9E%D7%A7%D7%95%D7%9E%D7%99%D7%95%D7%AA_%D7%9E%D7%97%D7%95%D7%99%D7%99%D7%91%D7%95%D7%AA_%D7%9C%D7%94%D7%A4%D7%A2%D7%99%D7%9C_%D7%90%D7%AA%D7%A8_%D7%90%D7%99%D7%A0%D7%98%D7%A8%D7%A0%D7%98_%D7%94%D7%9E%D7%A1%D7%A4%D7%A7_%D7%9E%D7%99%D7%93%D7%A2_%D7%9C%D7%A6%D7%99%D7%91%D7%95%D7%A8)
  - [Public participation hub — שיתוף ציבור](https://www.kolzchut.org.il/he/שיתוף_ציבור)
- Municipal FOI: the FOI Law (M05) applies to local authorities. Each authority has its own FOI officer.
- **Not recommended (paid/unavailable):** none.

### Gaps
- **Official "how a bill becomes law" page.** In a browser, go to main.knesset.gov.il, then "חקיקה", then "הליך החקיקה", and copy the URL.
- **Parliamentary questions (שאילתות) page and Research Center report search.** In a browser, go to main.knesset.gov.il, then "פעילות הכנסת", and find each page. Copy the URLs.
- **Lobbyist register.** Search main.knesset.gov.il for "שדלנים".
- **Local Authorities (Public Complaints Commissioner) Law 2008 (חוק הרשויות המקומיות (נציב תלונות הציבור), התשס"ח-2008).** The guessed Wikisource title returned 404. Search he.wikisource.org for "נציב תלונות הציבור" and use the exact title.
- **Openness of council meetings.** Search Wikisource for "פקודת העיריות". The rules on public council meetings and closed sessions are in the Second Schedule (התוספת השנייה); quote them from there. Also search Kol Zchut for "ישיבות מועצת העירייה".

## M18 — Organising: amutot, funding, and what non-lawyers may not do (התארגנות)

- [Amutot Law 1980 — חוק העמותות, התש"ם-1980 (Wikisource)](https://he.wikisource.org/wiki/חוק_העמותות) — founding, bylaws, organs, prohibited distribution, reporting, dissolution.
  - s.66(1): the fee regulations are תקנות העמותות (אגרות), התשנ"ח-1998.
  - s.59(a)(1): an amuta that does not pay its fee within 90 days may be treated as inactive.
  Edited 12.3.2026. — FREE-FULL — ✅
- [gov.il: register a new amuta online — רישום עמותה](https://www.gov.il/he/service/association_registration) — founders file online with National Digital Identity or a smart card. — ⚠️ (403)
- [gov.il: amuta annual fee — אגרה שנתית לעמותה](https://www.gov.il/he/service/association-annual-fee) — **VOLATILE, 2026, from a search-engine extract of this page:**
  - ₪1,777 regular, from 1.4.2026;
  - ₪1,338 if paid by 31.3.2026;
  - ₪176 discounted, for an amuta in its first two years or with turnover of ₪300,000 or less that filed its 2024 reports online.
  — ⚠️
- [Registrar of Associations: proper-management guidelines, 2018 (PDF)](https://www.gov.il/BlobFolder/policy/proper_management_guidelines/ar/association-2018.pdf) — the path is /ar/, so this may be the Arabic version; look for a /he/ copy. — ⚠️
- [Foreign State Entity Disclosure Law 2011, as amended 2016 — חוק חובת גילוי לגבי מי שנתמך על ידי ישות מדינית זרה (Wikisource)](https://he.wikisource.org/wiki/חוק_חובת_גילוי_לגבי_מי_שנתמך_על_ידי_ישות_מדינית_זרה) — the "transparency law":
  - s.2: quarterly reports;
  - s.5: disclosure on the organisation's website;
  - s.5א: if foreign-state entities are its main funder, the organisation must say so in publications, in letters to officials and at Knesset committees.
  — FREE-FULL — ✅
- [IDI: "The Amutot bill" (Kallner bill), 10.6.2025](https://www.idi.org.il/articles/59638) — the bill would:
  - impose an 80% tax on donations from foreign state entities;
  - bar organisations funded that way from petitioning the courts.
  It passed a preliminary reading in February 2025. A December 2025 report says a committee was debating it. **No later reading was found; status unknown.** — FREE-FULL — ✅
- **CRITICAL — [Bar Association Law 1961 — חוק לשכת עורכי הדין, התשכ"א-1961 (Wikisource)](https://he.wikisource.org/wiki/חוק_לשכת_עורכי_הדין)** — FREE-FULL — ✅
  - **s.20 (ייחוד פעולות המקצוע — acts reserved to lawyers):** "הפעולות המנויות להלן, לא יעשה אותן דרך עיסוק, או בתמורה אף שלא דרך עיסוק, אלא עורך דין". The reserved acts are:
    1. representing another person, and any argument or other action on their behalf, before courts, tribunals, arbitrators and quasi-judicial bodies;
    2. representing another person before listed authorities (Execution Office, Land Registry, the registrars, tax assessors and others);
    3. "עריכת מסמכים בעלי אופי משפטי בשביל אדם אחר" — drafting documents of a legal character for another person, including negotiating toward such a document;
    4. "ייעוץ וחיווי דעת משפטיים" — giving legal advice and legal opinions.
  - **s.21 (שמירת הוראות — savings):** s.20 does not affect the Attorney General's powers or "ייצוג לפני בתי דין דתיים ולפני בתי דין צבאיים" (representation before religious and military courts). The further items were not extracted.
  - **s.96 (הסגת גבול המקצוע — unauthorised practice), full text:** "מי שאינו עורך דין ועושה פעולה שנתייחדה לפי חוק זה לעורכי דין, דינו – קנס כאמור בסעיף 61(א)(2) לחוק העונשין." s.97 separately covers impersonating a lawyer.
  - **Course rule.** This is our reading of the text, not a ruling; have a lawyer review it before publishing.
    - The ban covers acts done **for another person** and **as an occupation or for payment**.
    - Doing these acts for yourself is outside s.20.
    - A one-off, unpaid favour is textually outside it, but organised or repeated NGO activity may count as "an occupation".
    - The course must teach learners to act **for themselves**, and should not offer drafting or advice for others.
- [Bar National Ethics Committee decision on amutot giving free legal services, Ethics Bulletin 29, Feb 2009 (.doc)](https://www.colman.ac.il/media/cxnjkaky/gilion-29hahlata_lenian_amotot_ml.doc) — per the search snippet:
  - an amuta or clinic representing clients for free must be run like a law office, by lawyers;
  - students act only under supervision;
  - no payment of any kind, including membership fees.
  — FREE-FULL — ⚠️ (file not decoded)
- [Bar Ethics Rules — כללי לשכת עורכי הדין (אתיקה מקצועית) (Wikisource)](https://he.wikisource.org/wiki/%D7%9B%D7%9C%D7%9C%D7%99_%D7%9C%D7%A9%D7%9B%D7%AA_%D7%A2%D7%95%D7%A8%D7%9B%D7%99_%D7%94%D7%93%D7%99%D7%9F_(%D7%90%D7%AA%D7%99%D7%A7%D7%94_%D7%9E%D7%A7%D7%A6%D7%95%D7%A2%D7%99%D7%AA)) — FREE-FULL — ⚠️
- [17th Knesset bill to let students and NGO volunteers do basic legal acts under supervision (.doc)](https://fs.knesset.gov.il/17/law/17_lst%20%20_85246.doc) — shows the current law does not allow this. Not known to have been enacted. — ⚠️
- **Not recommended (paid/unavailable):** Nevo and Takdin case law on s.96: PAID.

### Gaps
- **Rulings interpreting ss.20 and 96.** None verified, so cite none until one is checked.
  1. Search https://supremedecisions.court.gov.il/ and Kol Zchut for "הסגת גבול המקצוע", "סעיף 20 לחוק לשכת עורכי הדין" and "דרך עיסוק" together with "ייעוץ משפטי".
  2. Confirm any Supreme Court criminal appeal (ע"פ or רע"פ) found.
  3. Have a lawyer review the course wording.
- **Who else may represent someone.**
  - Labour courts: check s.34 of the Labour Court Law (חוק בית הדין לעבודה), on organisation representatives and relatives.
  - Small claims: check the Courts Law small-claims sections on representation.
  - Civil courts: check the Civil Procedure Regulations 2018 rule on representing a party.
  - Read the full list of s.21 savings on Wikisource.
- **Registration fee for a new amuta (2026).** Open the gov.il association_registration page and copy the amount and its date. Otherwise call the Corporations Authority (*5601, unverified).
- **Proper-management certificate (אישור ניהול תקין).** Search gov.il for "אישור ניהול תקין לעמותה" and record the conditions and the yearly cycle. It matters because it exempts amutot from FOI fees (M05).
- **Foreign-funding bill stage, 2026.** Search main.knesset.gov.il bills for "ישות מדינית זרה" and read the stage field.

## M19 — Practicum: courts, clinics, NGOs (התנסות)

- **Court observation.** Hearings are public under Basic Law: The Judiciary and Courts Law s.68, with exceptions.
  - [Kol Zchut: the right to attend court hearings — הזכות לנוכחות בבית המשפט](https://www.kolzchut.org.il/he/%D7%94%D7%96%D7%9B%D7%95%D7%AA_%D7%9C%D7%A0%D7%95%D7%9B%D7%97%D7%95%D7%AA_%D7%91%D7%91%D7%99%D7%AA_%D7%94%D7%9E%D7%A9%D7%A4%D7%98) — FREE-FULL — ⚠️ (403)
  - [Kol Zchut: closed hearings in family matters (s.68(ה))](https://www.kolzchut.org.il/he/%D7%93%D7%99%D7%95%D7%9F_%D7%91%D7%93%D7%9C%D7%AA%D7%99%D7%99%D7%9D_%D7%A1%D7%92%D7%95%D7%A8%D7%95%D7%AA_%D7%91%D7%A2%D7%A0%D7%99%D7%99%D7%A0%D7%99_%D7%9E%D7%A9%D7%A4%D7%97%D7%94) — FREE-FULL — ⚠️ (403)
  - [Kol Zchut: closed hearings in sex-offence cases (s.68(ב))](https://www.kolzchut.org.il/he/דיון_בדלתיים_סגורות_בעבירות_מין) — FREE-FULL — ⚠️ (403)
  - The statute itself: [Courts Law on Wikisource](https://he.wikisource.org/wiki/חוק_בתי_המשפט), s.68 — ✅
- **University legal clinics.** Clinics mostly serve clients or enrolled students; they are not courses.

| Clinic | What it covers | Check |
|---|---|---|
| [TAU — הקליניקות המשפטיות](https://en-law.tau.ac.il/clinics) | 9 clinics: human rights, refugees, workers, Knesset, class action, privacy | ✅ |
| [HUJI — המרכז לחינוך משפטי קליני](https://lawclinics.huji.ac.il/) | 10 clinics: international human rights, disability, innocence, cyber rights | ✅ |
| [Haifa — הקליניקות המשפטיות](https://law.haifa.ac.il/en/law-clinics/) | 8 clinics: environmental justice, human rights, public defender, war-time legal aid | ✅ |
| [Bar-Ilan — מערך הקליניקות](https://law-clinics.biu.ac.il/) | 8 clinics: disability, equality, environmental regulation, civil aid under Jewish law | ✅ |
| [Ono — המרכז למשפט קליני-חברתי](https://www.ono.ac.il/the-ono-center-for-social-and-clinical-law/clinics/) | labour, debt, public housing, National Insurance, prisoners, anti-SLAPP | ✅ |
| [Reichman — experiential programs](https://www.runi.ac.il/en/schools/law/special-programs/experiential-array) | health rights, anti-racism, public defender | ⚠️ |
| [Sapir — Legal Clinics](https://sapir.ac.il/en/node/1696) | Negev social rights, Bedouin access to rights | ⚠️ |

- **Public-interest NGOs, balanced across the spectrum.** Homepages are ⚠️ (not fetched) unless marked ✅.
  - Civil liberties and human rights:
    - [ACRI — האגודה לזכויות האזרח](https://www.acri.org.il) — the broadest civil-rights litigator. ✅ (law and protest subsites opened)
    - [Movement for Freedom of Information — התנועה לחופש המידע](https://www.meida.org.il) — FOI requests and petitions. ✅
    - [Movement for Quality Government — התנועה למען איכות השלטון](https://www.mqg.org.il) — governance petitions. ⚠️
    - [Bimkom — במקום](https://bimkom.org) — planning rights. ✅
    - [Yesh Din — יש דין](https://www.yesh-din.org) — legal aid and monitoring in the West Bank. ⚠️
    - [B'Tselem — בצלם](https://www.btselem.org) — human-rights documentation in the territories. ⚠️
    - [Kav LaOved — קו לעובד](https://www.kavlaoved.org.il) — workers' rights. ⚠️
    - [HIAS Israel](https://hias.org.il/) — legal aid for refugees and asylum seekers. ⚠️
    - [ASSAF — אס"ף](https://assaf.org.il) — aid to refugees and asylum seekers. ⚠️
    - [Adalah — עדאלה](https://www.adalah.org) — Arab minority rights. ⚠️
    - [Tag Meir — תג מאיר](https://www.tag-meir.org.il/en/) — against racism and "price tag" attacks. ⚠️
    - [HaMoked — המוקד להגנת הפרט](https://hamoked.org.il) — Palestinians' individual rights. ✅
  - Right-leaning and conservative:
    - [Regavim — רגבים](https://www.regavim.org) — land-use enforcement petitions. ✅
    - [Kohelet Policy Forum — פורום קהלת](https://kohelet.org.il) — conservative-libertarian policy and amicus briefs. ✅
    - [Lavi — ארגון לביא](https://www.lavi.org.il/%D7%90%D7%95%D7%93%D7%95%D7%AA/) — governance, through petitions to the High Court. ✅
    - [Choosing Life Forum — פורום בוחרים בחיים](https://chooselife.org.il) — bereaved families; terror deterrence, including legal action. ⚠️
    - Shurat HaDin — שורת הדין — lawsuits against terror funders. Only a [Facebook page](https://www.facebook.com/shurat.hadin.israel.law.center/) was found. ⚠️
    - Further options to verify: the Legal Forum for the Land of Israel (הפורום המשפטי למען ארץ ישראל) and Tzav 9 (צו 9).
- **Not recommended (paid/unavailable):** none. Clinics are free to their clients, but taking part as a student requires university enrolment.

### Gaps
- **Rules for entering a courthouse** (security check, ID, phones, filming ban). Search the judiciary site on gov.il for "כניסה לבית המשפט" or "ביקור בבית המשפט". Otherwise call the specific courthouse or \*3852.
- **Supreme Court live-stream page.** Hearings have been streamed since 2020. Open supreme.court.gov.il, find "שידורים חיים", and copy the URL.
- **Shurat HaDin official site.** Find and verify it, or drop the organisation.
- **NGO homepages marked ⚠️.** Click-check each one before publishing.

## Video lectures and audio (Hebrew)

Free Hebrew video teaching of Israeli law is scarce. Verified so far:

- [Knesset Channel — ערוץ כנסת (live and recordings)](https://www.knesset.tv) — committee and plenum recordings; the best "watch law-making" source. — FREE-FULL, no signup — ✅
- [Israel Democracy Institute YouTube channel](https://www.youtube.com/channel/UCoIxKW1Bof19buUQAbU9JJQ) — explainers and panels on the judiciary, the Knesset and the constitution. The channel loads; its playlists were not visible to the fetch. — FREE-FULL — ✅
- [Bimkom YouTube channel](https://www.youtube.com/@bimkomplannersforplanningr1623) — planning-rights videos. — FREE — ⚠️
- [TAU Law podcast "Medabrim Mishpatim" — מדברים משפטים](https://law.tau.ac.il/Podcasts_Medabrim-Mishpatim) — audio only. — FREE-FULL — ⚠️
- [TAU Law conferences and lectures archive](https://law.tau.ac.il/berg_main/conferences_lectures) — some events have video. — FREE — ⚠️
- [HUJI Law lectures listing](https://law.huji.ac.il/%D7%A1%D7%99%D7%95%D7%95%D7%92-%D7%90%D7%99%D7%A8%D7%95%D7%A2%D7%99%D7%9D/%D7%94%D7%A8%D7%A6%D7%90%D7%94) — not confirmed that recordings exist. — ⚠️
- [Campus IL — קמפוס IL (national free online-course platform)](https://campus.gov.il/en/) — all courses are free but **need free registration**. No law, civics or human-rights course was identified, and the site search returned HTTP 500. — FREE-FULL (platform) — ⚠️
- [Nevo free tutorial videos](https://www.nevo.co.il/) — videos on how to research legal databases. — FREE-LIMITED — ✅

### Gaps
- **Campus IL courses.** On campus.gov.il, open "קורסים" and filter or search for "משפטים", "אזרחות", "זכויות אדם", "חוקה" and "דמוקרטיה". Record each course URL and note "free registration required".
- **Open University (האוניברסיטה הפתוחה).** On YouTube, search the official channel for "משפט" or "חוקה". Also check the Open University's open-lessons pages and its Campus IL courses.
- **Law-faculty YouTube channels (TAU, HUJI, Haifa, BIU, Reichman).** Search YouTube for "הפקולטה למשפטים" plus the university name. Open Playlists and copy the deep links to conference series.
- **Judiciary YouTube.** Search for "הרשות השופטת" and check for an official verified channel. Otherwise use the Supreme Court live-stream page (M19 gap).
- **IDI Hebrew playlists.** On the IDI channel, open Playlists and pick the series on the Knesset, the judiciary and the constitution.
