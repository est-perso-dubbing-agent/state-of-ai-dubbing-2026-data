# Methodology: State of AI Dubbing 2026 (v2.0, Mid-Year Update)

> Companion methodology document for *State of AI Dubbing 2026: A Multi-Vertical Analysis*, Mid-Year Update.
> Released under CC BY 4.0. Free to cite with attribution to Perso Dubbing.
> Version 2.0 · Updated September 2026 · Version 1.0 published June 4, 2026

---

## 0. What changed in v2.0 (change log)

| Change | Detail |
|---|---|
| New chapters M0 to M7 | A paid-cohort analysis for December 1, 2025 to August 31, 2026, measured in dubbed minutes. The June chapters remain online below the new chapters as an annotated copy (annotations listed in the "June chapters" row); the original page and PDF are archived at `/v1/`. |
| Data window extended | Cumulative figures now cover January 1, 2025 to August 31, 2026 (20 months; 386,068 platform projects of every type and status, including audio-only and cancelled projects). |
| Data files | The 12 June files are regenerated on the extended period with a single denominator rule (Section 4). The June versions are archived unchanged under `data/v1/`. Column sets changed in two regenerated files: `quarterly-trends-2026.csv` gains a `note` column, and `use-case-map-counts-2026.csv` and `use-case-map-pct-2026.csv` follow the current target-language set. The v2.0 files use CRLF line endings; read columns by name, not position. 25 new files are added, most for the paid cohort (Section 8). |
| Correction | The June text stated that the top 1% creator cohort (n = 47) averaged 15 target languages. In the June data file, 15 is the minimum of that cohort; the average is 20.3. |
| Findings re-tested | June Finding 1 is corrected, Finding 2 is retired, Finding 3 is confirmed (Chapter M6). |
| Reproducibility | v2.0 is produced by a deterministic script chain (Section 9). Re-running the June period through it reproduces the June headline figures (Section 6.4). |
| Share-link-enabled rate (June: "share rate") | Published for the whole period as a descriptive statistic; no period is used as a finding (Section 6.2). The June reading of the figure as evidence that videos were "shared immediately" is withdrawn. |
| Growth rates | None reported (Section 6.3). |
| Author of record | Taeksoon Kwon, Chief Technology Officer, ESTsoft (Perso Dubbing), is the named author from v2.0; data preparation and analysis by the Perso Dubbing Data Team. |
| Naming | The platform is referred to as Perso Dubbing throughout v2.0; the June text used Perso AI. The author of record from v2.0 is Taeksoon Kwon, Chief Technology Officer, ESTsoft (Perso Dubbing), with the Perso Dubbing Data Team (the June text carries the byline "Perso AI Data Team"); the license line is "attribution to Perso Dubbing" on the page, the PDFs and the press kit. The June scoping qualifier is kept as "within Perso Dubbing's data". |
| June chapters | Kept online below the new chapters as an annotated copy. Annotations to the June text on the page: the three finding headings are relabeled and each carries a correction notice linking to Chapter M6; a "Superseded" line precedes the paragraph "How these three findings connect"; the "Top 1% (n = 47)" table cell is annotated with the cohort average (20.3); the "Methodology" heading is relabeled "Dataset (June 2026 edition, v1.0)" and its "Period" and "Geographic reach" rows are annotated; headings are demoted one level. The June text is otherwise as published. The June PDF and data files are archived byte-identical at `v1/state-of-ai-dubbing-2026-v1.pdf` and `data/v1/`. The archived page at `/v1/` keeps the June body text byte-identical, with archival changes around it: an archive banner, a noindex tag, an archived-edition title and social description, the structured data removed, the download links repointed, the byline corrected and the placeholder DOI removed from the meta tags and footer. The main PDF (state-of-ai-dubbing-2026.pdf) carries the current edition with the annotated June text appended after an errata sheet. |

---

## 1. Data Sources and Scope

**Platform**: Perso Dubbing (perso.ai), an AI dubbing platform with paying customers in 119 billing countries over the subscription ledger's lifetime (68 with an active subscription on September 7, 2026). The ledger predates the data period, so 119 describes the customer base as of September 7, 2026 and is not a figure for January 2025 to August 2026.

**Project data**: two complete project-level exports from the platform, covering January 1, 2025 to April 28, 2026 (the June edition's export, 316,856 projects) and April 29 to August 31, 2026 (69,212 projects). Timestamps are in the platform's operating timezone (UTC+9). One row is one project; each target language is its own project. All generation types (dubbing, lip-sync, audio separation, transcription) and all lifecycle statuses (active, system-deleted, user-deleted, cancelled) are present in the raw data.

**Joined records**: the platform credit ledger (plan tier and credits per charged project, available from December 1, 2025), subscription and enterprise-contract records (plan and workspace), the payment platform's customer record (billing country), and a platform list of multi-account abuse accounts.

**Scope of findings**: findings describe activity on Perso Dubbing. They are not estimates of the AI dubbing market. Single-platform data carries user-acquisition bias and product-specific behavior (Section 6).

**Personal data**: e-mail addresses and titles are dropped at load. Only aggregates are published; project-level data is not released.

---

## 2. Three Analytical Lenses

### 2.1 Lens A : Cumulative platform (January 2025 to August 2026)

All 386,068 platform projects, all statuses, as in the June edition. Used for: platform scale, language and pair counts, the cumulative Use Case Map, the professional-creator multi-language distribution, the share-link-enabled rate through June 10, 2026, and the advisory quarterly table.

Lens A applies no exclusions: it keeps the multi-account abuse accounts, the internal and demo workspaces and the cancelled projects that Lenses B and C remove (Section 3). Cumulative counts are therefore not directly comparable with paid-cohort counts, and any marketing use of the cumulative total inherits these inclusions.

### 2.2 Lens B : Paid cohort (December 2025 to August 2026)

Projects created on a paid plan (Starter, Creator, PRO, Team, Enterprise) between December 1, 2025 and August 31, 2026, after exclusions (Section 3). Used for the paid-cohort figures in Chapters M2 to M6. The free comparison column in M2 uses Lens C, and the cumulative re-test rows in M6 use Lens A. The window starts when the credit ledger starts, which is also the day usage-based pricing replaced unlimited plans.

### 2.3 Lens C : Free comparison cohort

Free-plan projects in the same window with the same exclusions. Used as the comparison column in Chapter M2 and for the free-cohort rows of the June re-test in Chapter M6 (Section 6.5).

---

## 3. Key Definitions

**Professional creator** (Lens A): a creator account with six or more projects in the period. Cumulative n = 4,290. **Single-use creator**: exactly one project; n = 144,983.

**Categorized project**: a project carrying an industry label. Projects without any label are reported as Uncategorized and are never folded into Other. The Use Case Map window is October 1, 2025 to August 31, 2026 (n = 173,048), extending the June window (which started October 2025 for the same categorization-quality reason).

**Industry**: the platform's category labels, which users choose in their own language (335 distinct labels across Korean, Japanese, Portuguese, Spanish, Thai, Hindi, Russian and other languages), are normalized to the June taxonomy of 19 industries plus Other by a published rule set. Eleven product categories that did not exist in the June taxonomy (Music, Kids & Family, History & Culture, Digital & IT, DIY, Art, Fashion, Audio, AI-generated, Plants & Gardening, miscellaneous) are folded into Other and listed in the data files. Zero labels are unmapped.

**Language**: base language name. With the April 29, 2026 export the platform's labels for three languages (English, Spanish, Portuguese) switched to regional variants (English (US), Spanish (Mexico), Portuguese (Brazil)); for those three, generic labels appear only before that date and variant labels only after it. All other languages keep a single label. Variants are collapsed to the base language for comparability with June, and the raw label counts are listed in `paid-language-minutes-2026.csv`.

**Active language pair**: a distinct source-to-target combination with at least one project, counting "Auto Detect" and "Other Languages" as sources, as in June. Cumulative n = 1,162.

**Plan tier** (Lens B), assigned per project in this order: (1) workspace under an enterprise contract during the contract period → Enterprise; (2) credit-ledger row → the ledger's plan tier, which is the plan at the time of use (for the 62 projects with ledger rows on more than one tier, the tier of the largest charge); (3) no ledger row, which is the case for lip-sync and multi-language child projects charged on the parent → the creator's most frequent ledger tier in the same month; (4) otherwise unknown (1.8% of window projects; excluded from the paid cohort and from denominators). Inherited rows are 35.5% of paid projects and 26.5% of paid minutes; Section 5.3 reports every headline without them.

**Creator tier** (tables by tier in Lens B): a creator is assigned the highest plan tier reached in the window, so each creator counts once. Project-level figures use the project's own tier.

**Within Perso Dubbing's data**: the scoping qualifier used throughout, as in June. Findings describe Perso Dubbing's cohorts and are not estimates for the AI dubbing market.

**Exclusions** (Lenses B and C): accounts on the platform's multi-account abuse list (2,636 accounts in the window; 410 paid-tier projects), internal and demo workspaces (15 plan names; 103 accounts), and cancelled projects.

**Dubbed minutes**: the translated-video length of a project. 96.0% of paid projects carry a duration. Audio-separation and transcription projects have no translated video and carry none (2,009 paid projects, of which 528 from December 2025 to March 6, 2026 have no recorded type and are classified by their missing duration); a further 643 dubbing and lip-sync projects lack a duration. Averages use only projects with a duration (n = 64,194); minute totals are sums over those projects.

**Credits**: the ledger's charged quota per project (charges minus rollbacks). Six paid projects with net-negative credits (refunds after failed jobs) are clipped to zero. Credits are a secondary metric and are not converted to currency, because promotional discounts differ by market.

**Billing country**: the country on the paying customer's payment record, matched through the creator's most recent customer ID. Enterprise contracts are invoiced outside the payment platform and carry no country. Country tables therefore cover self-serve plans only (90.7% of self-serve paying creators matched) and are shown against two denominators: matched self-serve minutes (211,381) and all paid minutes (303,241). Countries are shown individually where they have at least 10 paying creators and 300 dubbed minutes (35 countries); the remaining 72 are pooled. Billing country is not audience country.

**Countries with a paid subscription**: countries with at least one customer whose subscription is active, cancelled or past due (119 as of September 7, 2026); leads without a payment are excluded. 68 countries had an active subscription on that date. The June edition's "80+ countries" has no recoverable definition and is not compared.

**Share-link-enabled rate** (called "share rate" in the June edition): projects with a share link enabled, which was the platform default for every project until June 10, 2026. The data does not record whether a link was opened, sent or published. Published for the whole period in `share-rate-daily-2026.csv` as a descriptive statistic; no period is used as a finding, because the figure records the platform default on both sides of the June 11, 2026 change (Section 6.2).

---

## 4. The Use Case Map (cumulative and paid)

**Cumulative map** (Lens A): 19 industries plus Other (rows) by the 20 largest target languages (columns), cell value = share of the industry's categorized projects; n = 173,048, all statuses. This is the June construction extended to August 2026 with one change: the June downloadable files used active projects only (n = 42,046) while the June text used all statuses (112,797). v2.0 uses all statuses in both, and the June files are archived under `data/v1/`.

**Paid map** (Lens B): the same rows and columns, cell value = dubbed minutes; n = 66,846 projects. Cells with fewer than 300 dubbed minutes are flagged in the long-format file and not used for findings. Industry and language rows used for findings have at least 500 projects and 300 minutes.

---

## 5. Statistical Conventions

### 5.1 Confidence intervals

Shares of project counts carry 95% intervals from the normal approximation, CI = p ± 1.96 × √(p(1-p)/n), as in June. Shares of minutes are not binomial and carry no interval; they are reported with their n.

### 5.2 Concentration

Creator-level concentration (top 1%, top 10%) ranks paying creators by their total dubbed minutes in the window. Workspace concentration uses the same measure per workspace.

### 5.3 Sensitivity

`sensitivity-key-findings-2026.csv` reports the paid share of minutes, the Religion target mix, the largest source-to-target flow and the multi-language share under five scenarios: baseline; excluding inherited-tier projects; excluding December 2025; excluding the Enterprise tier; excluding the five largest workspaces. Numerators and denominators are filtered identically in each scenario. A finding is used in the text only if its direction holds in every scenario or the exception is stated next to it (as with the Korean-to-English flow, which ranks first overall and fifth among self-serve plans).

### 5.4 Non-additive creator counts

Creator counts in per-row tables (columns named `paid_creators_non_additive`) are not additive across rows: one creator can appear under several tiers, industries or countries. Distinct paying creators in the window: 2,902.

---

## 6. Limitations

### 6.1 User-acquisition mix

Target-language concentrations reflect where Perso Dubbing acquires customers as much as where demand is. The June edition flagged Hindi-target Animation and Film content and Korean-target Science & Tech content as cases where this applies; the paid re-test in Chapter M6 shows that the Korean-target ranking did not hold, which supports the June caution. Cross-platform data would be needed to separate acquisition from demand.

### 6.2 Share-link-enabled rate: the June behavioral reading is withdrawn

The June edition reported a 96% "share rate" and read it as evidence that dubbed videos were shared immediately. The metric is the share of projects with a share link enabled, and until June 10, 2026 that was the default state of every new project; the data does not record whether anyone opened, sent or published the link. The behavioral reading is therefore withdrawn. The figure is kept as a descriptive statistic: 95.9% of projects created between January 1, 2025 and June 10, 2026 had a share link enabled. On June 11, 2026 the platform changed the default; the daily rate was 97.3% on June 10, 57.8% on the day of the change, and 12.4% from June 12 to August 31, 2026 (13.0% for the rest of June, 13.3% in July, 11.1% in August; `share-rate-daily-2026.csv`, which carries daily rows from May 25 to August 31 and four period-summary rows). The rate after the change measures the new default. It is published, but it is not used as a finding and is not compared with the earlier period.

### 6.3 No growth rates

Usage-based pricing replaced unlimited plans on December 1, 2025. Monthly output fell from 206,110 dubbed minutes in November 2025 to 39,946 in January 2026 as a result. The June edition avoided platform-wide volume comparisons for a related reason; v2.0 reports no year-over-year rate of any kind. December 2025 is a transition month in which legacy balances were consumed; it holds 30.3% of paid minutes in the window and every headline is reported without it (Section 5.3). Monthly paid minutes from January to August 2026 are published in `paid-monthly-2026.csv` for context only.

### 6.4 June figures that do and do not reproduce

Re-running the June period through the v2.0 pipeline reproduces 316,856 projects, 112,797 categorized projects, 36 × 34 languages, 909 pairs and the 95.8% share-link-enabled rate exactly. Three June creator-level figures do not reproduce under the documented rule: professional creators 4,023 (v2.0 rule: 3,743), single-use creators 115,439 (114,573), professional projects 143,805 (145,596). All three derive from one per-account count, so a single undocumented June filter is the likely cause; the June pipeline was not retained, and the cause cannot be recovered. The June headline data file also listed 112,805 categorized projects where the June methodology said 112,797; v2.0 reproduces 112,797. The June statement "top 1% average 15 languages" referred to the cohort minimum (Section 0). v2.0 states its rules and the recomputed figures.

### 6.5 The June Religion figure and the free cohort

The June "Religion dual hub" (English 25.6%, Portuguese 25.2%) was computed on all projects, October 2025 to April 2026, without a plan split. v2.0 reports three things about it, each in `v1-findings-retest-2026.csv`. First, on paid Religion projects (December 2025 to August 2026) the targets are English 27.8%, Spanish 14.8%, Portuguese 4.6% (n = 6,823). Second, in the free cohort of the same period, 1,467 accounts created exactly one Portuguese-target Religion project each. Third, the June window can be split by plan only from December 1, 2025, when the credit ledger begins: in that part of the window, 924 of 1,632 free-tier Religion projects (56.6%) targeted Portuguese, each from an account with no other Portuguese-target Religion project (922 of the 924 accounts created no other project at all), against 8.6% of 2,529 paid-tier Religion projects; the 1,975 categorized Religion projects of October and November 2025 predate the ledger and are not split (their Portuguese share is 21.2%). The 1,467 figure therefore describes the December 2025 to August 2026 free cohort, and the explanation of the June figure is established for the five months of its window that can be tested (December 2025 to April 2026); October and November 2025 cannot be tested.

### 6.6 Contract concentration

Enterprise contracts are 23.5% of paid minutes from 111 accounts, and the largest single source-to-target flow (Korean to English, 50,892 minutes) is 76.6% contract volume. Contract flows are reported separately from self-serve behavior and are not generalized to a market trend.

### 6.7 Country

Billing country is the location of the payment method. 30.3% of paid minutes have no country (contracts and unmatched self-serve records) and are shown as explicit residual rows. Country shares of all paid minutes are lower bounds.

---

## 7. Editorial Framing

The June edition's four-layer framing of AI dubbing as a distribution-stage category is kept as editorial framing. The share-link-enabled rate that the June edition cited as support is not carried forward as a behavioral signal (Section 6.2). Country rows describe the billing country of the paying customer and the target languages of the minutes produced; they are not read as import, export or market-demand statements, because the data records neither the source market of the content nor its audience.

---

## 8. Data Files Released (CC BY 4.0)

At `perso.ai/research/state-of-ai-dubbing-2026/data/`. June files are archived unchanged under `data/v1/`.

**Cumulative (Lens A), regenerated for January 2025 to August 2026, June schema**: `headline-statistics-2026.csv`, `use-case-map-counts-2026.csv`, `use-case-map-pct-2026.csv`, `use-case-map-long-2026.csv`, `per-target-language-inverse-2026.csv`, `industry-deep-dive-2026.csv`, `per-language-deep-dive-2026.csv`, `multi-language-adoption-2026.csv`, `multi-language-adoption-cumulative-2026.csv`, `top1pct-cohort-anonymized-2026.csv`, `quarterly-trends-2026.csv` (advisory; a note column explains each column), `methodology-2026.md` (this document).

**Paid cohort (Lens B), new in v2.0**: `paid-headline-2026.csv`, `paid-vs-free-profile-2026.csv` (includes the free-plan 99th-percentile duration), `paid-concentration-2026.csv` (creator and workspace concentration), `paid-multi-language-by-tier-2026.csv`, `paid-language-pairs-by-tier-2026.csv`, `paid-largest-flow-composition-2026.csv`, `platform-monthly-minutes-2026.csv` (all-cohort monthly series across the pricing change), `share-rate-daily-2026.csv` (daily the share-link-enabled rate around June 11, 2026), `paid-new-languages-2026.csv`, `v1-period-recompute-2026.csv` (June figures re-run under the v2 rules), `methodology-counts-2026.csv` (the exclusion and normalization counts cited in this document), `paid-industry-minutes-2026.csv`, `paid-language-minutes-2026.csv`, `paid-usecase-map-minutes-2026.csv`, `paid-usecase-map-minutes-long-2026.csv`, `paid-tier-mix-by-industry-2026.csv`, `paid-country-profile-2026.csv`, `paid-country-language-long-2026.csv`, `paid-multi-language-adoption-2026.csv`, `paid-monthly-2026.csv`, `paid-language-pairs-2026.csv`, `paid-production-signals-by-industry-2026.csv`, `v1-findings-retest-2026.csv`, `v1-vs-v2-industry-share-2026.csv`, `sensitivity-key-findings-2026.csv`.

---

## 9. Reproducibility

Every published file is produced by three scripts run in order: a fact-table builder (joins the two exports with the ledger, subscription, contract, country and abuse records and assigns tiers), a table builder (writes the CSV files and runs 25 automated checks on sums, denominators and June reproduction), and a findings script (computes the figures quoted in the text with n and intervals). All ordering ties are broken deterministically; running the chain twice yields byte-identical files. Every figure quoted in the text and in this document appears in, or is a sum or difference of, values in the published files; the file that carries each figure is named under its chapter, and the exclusion and normalization counts cited here are in `methodology-counts-2026.csv`. Project-level data is not released.

---

## 10. Update Cadence

| Edition | Schedule |
|---|---|
| State of AI Dubbing 2026 (v1.0) | Published June 4, 2026 |
| Mid-Year Update (v2.0, this document) | September 2026 |
| State of AI Dubbing 2027 | June 2027 (annual cadence) |

---

## 11. Citation

**APA**:
> Kwon, T., & Perso Dubbing Data Team. (2026). *State of AI Dubbing 2026: A Multi-Vertical Analysis, Mid-Year Update (v2.0).* Perso Dubbing. https://perso.ai/research/state-of-ai-dubbing-2026/

**Methodology**:
> Kwon, T., & Perso Dubbing Data Team. (2026). *State of AI Dubbing 2026: Methodology Notes, v2.0.* https://perso.ai/research/state-of-ai-dubbing-2026/data/methodology-2026.md

---

## 12. Contact

- Press inquiries: press@perso.ai
- Data inquiries: data@perso.ai
- Press Kit: perso.ai/research/state-of-ai-dubbing-2026/press-kit/

*Released under CC BY 4.0. Free to share, cite, and re-use with attribution to Perso Dubbing.*
*Version 2.0 · September 2026 · Taeksoon Kwon and the Perso Dubbing Data Team*
