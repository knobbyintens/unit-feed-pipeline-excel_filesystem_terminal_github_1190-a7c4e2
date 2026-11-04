# Aurora Retail Group — Unit Feed Pipeline

Category operations repository for the monthly unit feed.

- Source export archive: `data/warehouse_unit_export.xlsx.b64` (base64-encoded
  workbook; decode it to obtain `warehouse_unit_export.xlsx`, worksheet `LegacyExport`)
- Published feed: `feeds/unit_feed_2020_2024.csv`
- Tracker: see the open `Monthly unit feed — pipeline tracker` issue

The source workbook is a legacy WMS export: wide multi-block layout, newest
rows first, includes forecast rows, blank year separators and pre-window
history. Only actual monthly figures for the 2020-01 through 2024-12 window
belong in the feed.
