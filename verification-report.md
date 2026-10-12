# Verification and size report

The current catalog contains **103 entries**. The two HD(CP)² input records are represented by one dataset row with two download options. The full four-hour series is the default option; only the active option is counted.

## Reported size coverage

| Evidence | Entries |
|---|---:|
| Reported download size | 81 |
| Reported component or per-file sizes | 6 |
| Reported hosted capacity (excluded from downloads) | 9 |
| No matching source total | 7 |

Source labels remain rounded where the source is rounded. A green badge indicates source provenance, not byte-exact precision. Open SciVis and LANL listings use the documented binary unit basis; other conversions use the recorded basis. No new download or checksum verification is asserted.

## Download totals (initial selections)

| Selection | Entries | Estimated download bytes | Entries without a fixed download size |
|---|---:|---:|---:|
| Default selection | 86 | 5,414,124,600,099 | 1 |
| Original spreadsheet selection | 75 | 1,794,558,825,659 | 0 |
| Open SciVis | 55 | 1,609,564,725,659 | 0 |
| LANL collections | 11 | 3,619,565,774,440 | 1 |

## HD(CP)² options

| Option | Source-reported components | Estimated download bytes |
|---|---|---:|
| Four-hour series (full dataset) | 96 GB + 2.6 TB | 2,696,000,000,000 |
| One time step (smaller subset) | 81 MB + 12 GB | 12,081,000,000 |

Both options use the existing [publisher metadata](https://scivis2017.dkrz.de/data.html) and registered download location. These are alternative scopes of one dataset.

## Interface changes

- One HD(CP)² row; selecting every visible row can now select all 103 entries.
- The expanded option selector updates the row, download totals, and exported record.
- Parentheses replace em-dash separators; an empty selection displays 0 B.
- Forced uppercase styling is removed. Scientific acronyms and source unit labels retain their meaningful case.
- The uploaded heading, description, table labels, and Helvetica/Arial styling are preserved.
- The catalog uses one download-size summary and visible-row selection controls.

## Validation

Validated all 103 record IDs, both HD(CP)² options, their exact effect on numeric totals, visible-row bulk selection, and the empty-selection state. All other 102 records and initial selection totals are unchanged. The scripts initialize without missing control references. No em-dash characters or forced-uppercase CSS remain.
