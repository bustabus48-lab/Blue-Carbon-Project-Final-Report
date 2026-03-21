# PDF Normalization Notes

## Scope
Normalized Markdown extraction was completed for:
- `source_reports/draft_inception_report_rev2.pdf`
- `source_reports/Ecosystem Health report draft.pdf`

Outputs:
- `normalized/inception_report.md`
- `normalized/ecosystem_health_report_draft.md`

## Extraction quality observations
1. **Character spacing artifacts** are present in several sections (e.g., letters split by spaces).
2. **Duplicated blocks** appear in some table-of-contents and tabular sections.
3. **Table structure loss** is visible where columns were flattened into prose-like sequences.
4. **Pagination/header carry-over** text appears in running content and should be ignored during evidence citation.

## Usage guidance
- Treat normalized files as **pre-processing artifacts**, not citation-grade sources.
- For citation-critical claims, confirm against original PDFs.
- Use chapter-level extraction and manual correction before final synthesis where tables are involved.

## Pending QA actions
- [ ] Remove duplicated ToC segments in `normalized/inception_report.md`.
- [ ] Reconstruct critical tables needed for methods and site evidence.
- [ ] Build a section index keyed to original PDF page numbers.
