Cite the source report: Kwon, T., and Perso Dubbing Data Team (2026). *State of AI Dubbing 2026: A Multi-Vertical Analysis, Mid-Year Update (v2.0)*. https://perso.ai/research/state-of-ai-dubbing-2026/ Data supplement: https://doi.org/10.5281/zenodo.23338581.

# State of AI Dubbing 2026: public data supplement (v2.0)

This supplement preserves the 36 public CSV files and accompanying methodology from Perso Dubbing's September 2026 report, retrieved on October 13, 2026. Files in `data/` are unchanged copies of the published sources. The tables include aggregate statistics and a published anonymized creator/workspace cohort summary. Project-level exports, account identities, audio and video are not included.

## Scope and units

| Population | Window | Interpretation |
|---|---|---|
| All platform projects | January 1, 2025 to August 31, 2026 | 386,068 projects of every type and status, including transcription, audio separation and canceled projects. This is not a count of completed dubbed videos. |
| Paid cohort | December 1, 2025 to August 31, 2026 | 66,846 paid-plan projects after the published exclusions, 2,902 paying creators and 303,241 dubbed minutes. Minute totals use projects with recorded translated-video duration. |
| Categorized Use Case Map | October 1, 2025 to August 31, 2026 | 173,048 categorized projects. Check each table's denominator before comparing it with paid-cohort tables. |

The 68 target languages and 1,162 active language pairs describe the all-platform window. The paid cohort used 55 target languages and 617 pairs. Observed usage is distinct from the product's supported-language count.

## Files and reuse

See `FILE_INDEX.md` for every CSV's row count and column names. Each table retains its own schema; files must not be concatenated into one table. Percentage columns and creator counts can have different denominators or be non-additive. Read each table's headers and the [methodology](data/methodology-2026.md).

Use these tables to cite or inspect the report's descriptive findings. They do not establish global market share, audience geography, causal effects or changes in demand. Billing country is the payment location. Project counts across the December 1, 2025 pricing change are not a consistent growth series. Plan-tier differences in multilingual use are associations.

## Source clarification

The preserved methodology contains wording that Section 5.3 reports "every headline" without inherited-tier projects and that all headline findings survive a sensitivity check. The published sensitivity CSV covers selected metrics, not every headline figure or every industry/language share. Reuse only the comparisons actually present in `sensitivity-key-findings-2026.csv`. This note clarifies the scope; the source files remain unchanged. For corrections after this snapshot, consult the [living report](https://perso.ai/research/state-of-ai-dubbing-2026/).

## Provenance and license

`SOURCE_MANIFEST.json` records source URLs and SHA-256 hashes. `SHA256SUMS.txt` covers the source data files. The source report releases these public findings and data tables under [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/). Attribute Perso Dubbing, retain the source citation and license link, and identify any changes you make. No independent peer review is claimed.

Authors of the source report: Taeksoon Kwon and Perso Dubbing Data Team. Publisher: Perso Dubbing. This supplement was prepared for distribution by Perso Dubbing; the uploader is not substituted for the report's authors.

## Citation

```bibtex
@misc{persodubbing2026midyear,
  author = {Kwon, Taeksoon and {Perso Dubbing Data Team}},
  title = {State of AI Dubbing 2026: A Multi-Vertical Analysis, Mid-Year Update (v2.0)},
  year = {2026},
  publisher = {Perso Dubbing},
  note = {Originally published June 4, 2026; updated September 2026},
  url = {https://perso.ai/research/state-of-ai-dubbing-2026/}
}
```

The published data supplement is available at https://doi.org/10.5281/zenodo.23338581. This DOI identifies the data supplement; the source report remains at its original URL.

## Preparation tools

OpenAI Codex assisted with drafting the distribution README, dataset card and deposit description, and with packaging and file checks. The 36 source CSVs and accompanying methodology were copied unchanged from the published report; no new research observations or data values were generated for this supplement.
