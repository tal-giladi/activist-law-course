# External link report

Checked 2026-10-13. Scope: `lessons/module-01` to `module-19` (*.md), `projects/m01`–`m19`, `templates/*.md`, `references/*.md`. Module 20 was not checked.

Method: a script pulled every http(s) URL from 177 files. Each unique URL got `curl -sIL`, then a full GET with a browser User-Agent and a 20–25 s timeout, following redirects. The script recorded the final status, final URL and page `<title>`, so it could catch soft 404s, home-page redirects and wrong-site redirects. When a URL hit a 403, 429 or 504 bot wall, I tried WebFetch once.

## Summary

| Result | Unique URLs |
|---|---|
| Total unique URLs | 706 |
| Fine (opens, right page) | 674 |
| BROKEN / REDIRECTED-WRONG | 2 |
| BLOCKED (manual check) | 30 |
| Paywalled | 0 |

Notes on the "fine" count:
- It includes 17 URLs that curl could not open (Cloudflare 403/400) but WebFetch opened and confirmed: 6 OpenLearn sections, 9 Times of Israel articles (EN and FR), Israel Policy Forum's tracker, and Meta's transparency report.
- All 291 he.wikisource.org links and all kolzchut.org.il links return 200. MediaWiki returns 404 for missing pages, so none of them is a missing page.
- The meida.org.il deep links (`/submit-an-information-request`, `/activities`, two `wp-content` PDFs) open directly. None redirected to abuse.spd.co.il in this check.
- These redirects are harmless:
  - `israelbar.org.il` goes to `israelbar.biz/home/`, the Bar Association's own site, with the same title.
  - Ono's clinics URL goes to `ono.ac.il/clinical-law/`, the same clinics page.
  - Several gov.il `/departments/guides/...` links go to `/pages/...` on the same page.
  - `mavat.iplan.gov.il` sends HEAD requests to a maintenance page, but GET opens normally.
- The OA tags check out: the Cambridge core-reader article is Open Access (CC), the Taylor & Francis book is open access, and both edX courses offer audit.

## BROKEN / REDIRECTED-WRONG

| URL | Used in (file:line) | Status | Final URL | Suggested free replacement (verified opens) |
|---|---|---|---|---|
| https://www.mevaker.gov.il/ombudsman | lessons/module-05/lesson-04.md:16, :166; lessons/module-19/lesson-03.md:21, :206; references/external-resources.md:58 | 302 → 200, lands on home page | https://www.mevaker.gov.il/ (title "דף הבית") | https://www.mevaker.gov.il/ombudsman (200, "נציבות תלונות הציבור"); the online form is https://complaint.mevaker.gov.il/ (200) |
| https://www.cbs.gov.il/he/subjects/Pages/%D7%9E%D7%93%D7%93-%D7%94%D7%9E%D7%97%D7%99%D7%A8%D7%99%D7%9D-%D7%9C%D7%A6%D7%A8%D7%9B%D7%9F.aspx (מחשבון הצמדה) | lessons/module-09/lesson-02.md:21; lessons/module-09/lesson-04.md:23 | 200, but a soft 404: "Oops, Something is wrong / the page is not found" (confirmed by WebFetch) | same URL | No working human-facing CBS calculator URL found. Four guessed CBS paths gave the same error page. Use the CBS index API the course already cites, which returns 200 JSON: https://api.cbs.gov.il/index/data/calculator/120010?value=50000&date=06-20-2007&toDate=09-20-2026&format=json&download=false (change value and dates). Or link the CBS home page https://www.cbs.gov.il/ and tell learners to use its "מחשבון הצמדה" tool. |

## BLOCKED (manual check)

These URLs failed to load for a bot from here, or loaded only a JavaScript shell with no checkable content. Open them in a browser.

**www.gov.il**: Cloudflare 403 to both curl and WebFetch ("Just a moment..."). Other gov.il URLs, such as BlobFolder PDFs and `/service/filing-objection`, did open, so this is bot blocking, not dead pages.
- https://www.gov.il/he/Departments/DynamicCollectors/legal-advisor-guidelines
- https://www.gov.il/he/departments/foi/govil-landing-page
- https://www.gov.il/he/service/freedom-of-information-complaint-submission
- https://www.gov.il/he/service/exempt_from_payment_of_a_fee
- https://www.gov.il/he/pages/netlaw_guide_24?chapterIndex=3
- https://www.gov.il/he/service/filing_a_complaint_against_police
- https://www.gov.il/he/pages/complaint_against_police
- https://www.gov.il/he/departments/guides/police_public_complaints_unit?chapterIndex=1
- https://www.gov.il/he/departments/guides/public_defender_public_information?chapterIndex=3
- https://www.gov.il/he/departments/general/police_criminal_information_closed_cases
- https://www.gov.il/he/Departments/General/public_inquiries_ilita
- https://www.gov.il/he/service/complaint_discrimination_inaccessibility_people_with_disabilities
- https://www.gov.il/he/service/accessibility_query_people_with_disabilities
- https://www.gov.il/he/service/licensing-appeal-submission
- https://www.gov.il/he/departments/guides/moep_public_inquiries?chapterIndex=2
- https://www.gov.il/he/service/filing_a_small_claim
- https://www.gov.il/he/pages/small_claims_description_guide
- https://www.gov.il/he/service/legal_aid_application
- https://www.gov.il/he/service/association_registration
- https://www.gov.il/he/service/association-annual-fee

**govforms.gov.il**: returns 200, but it is a React shell and the form content cannot be checked by fetch.
- https://govforms.gov.il/mw/forms/Shivion@moital.gov.il

**main.knesset.gov.il**: non-standard HTTP 247 with an empty body (bot wall). The Knesset PDF and OData links opened fine.
- https://main.knesset.gov.il/apps/legislation/main/laws
- https://main.knesset.gov.il/apps/legislation/main/laws/2000832
- https://main.knesset.gov.il/Activity/Info/research/Pages/default.aspx

**www.icc-cpi.int**: 504 to curl, 403 to WebFetch. otplink.icc-cpi.int opened fine.
- https://www.icc-cpi.int/palestine

**ihl-databases.icrc.org**: 200, but a JavaScript single-page app with an empty shell, so the content cannot be checked by fetch.
- https://ihl-databases.icrc.org/en/customary-ihl
- https://ihl-databases.icrc.org/en/ihl-treaties/api-1977/state-parties
- https://ihl-databases.icrc.org/en/ihl-treaties/hague-conv-iv-1907/regulations-art-42

**library.oapen.org**: 403 "Making sure you're not a bot!". WebFetch dropped the connection.
- https://library.oapen.org/bitstream/20.500.12657/88272/1/9781040010235.pdf (references/external-resources.md:151)

**web.archive.org**: repeated 429 rate limit, and WebFetch cannot fetch from this domain. `web.archive.org/save` opened (200).
- https://web.archive.org/web/20160102015819/http://www.mfa.gov.il/mfa/foreignpolicy/peace/guide/pages/israeli%20settlements%20and%20international%20law.aspx

## Module 20 (checked 2026-10-13)

Scope: `lessons/module-20/*.md` and quizzes, `projects/m20-capstone.md`, and the templates `theory-of-change.md`, `legal-strategy-map.md`, `campaign-execution-log.md`, `press-release.md` and `campaign-retrospective.md`. There are 33 unique URLs. Each got a GET with a browser User-Agent, and the check recorded the final URL and the page title.

| Result | Unique URLs |
|---|---|
| Fine | 32 |
| BROKEN / REDIRECTED-WRONG | 0 |
| BLOCKED (manual check) | 1 |

- All 19 he.wikisource links return 200 with the right page title. Every `#סעיף_N` anchor exists on its page: Basic Law: Judiciary s. 15, Administrative Procedure Amendment Law ss. 2 and 6, FOI Law s. 7, State Comptroller Law s. 45, Penal Law s. 144ד2, Administrative Courts Regulations s. 3 and HCJ Procedure Regulations s. 6.
- Kol Zchut "לשון הרע" and the three OpenLearn sections returned a Cloudflare 403 to the scripted GET, but they are live:
  - Kol Zchut: confirmed by HEAD 200 and by the MediaWiki API (page id 16284).
  - OpenLearn: confirmed by WebFetch. The pages are "Starting with law" §1, "Judicial decision making" section "6 Precedent and interpretation", and "Human rights and law" §2.1.
- These open with the right content:
  - the three Holistic Security chapters (1.2, 2.3, 4.1.11), checked by their chapter headings;
  - Front Line Defenders, theoryofchange.org, edX LouvainX, Versa and the UN AVL lecture series;
  - the TAU LL.B. booklet PDF, dated 12/08/26.
- BLOCKED: https://main.knesset.gov.il/Activity/Info/research/Pages/default.aspx (lessons/module-20/lesson-05.md:207) returns HTTP 247. This is the same Knesset bot wall listed above. The page is not dead, so it was left unchanged; open it in a browser to confirm.

No module-20 links needed changing.
