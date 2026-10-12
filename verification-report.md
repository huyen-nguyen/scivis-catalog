# Verification and size report

Checked: 8 October 2026 UTC. Input: scientific_visualization_catalog(3).xlsx and image(6).png.

The catalog includes all 93 input records and 11 LANL scientific collections, for 104 entries. No input workbook cells were modified. There is no verified exact total for all the scientific content represented by these sources.

## Download totals

| Selection | Entries | Exact RAW bytes | Rounded estimates | Unknown download entries | Known subtotal |
|---|---:|---:|---:|---:|---:|
| Open SciVis RAW volumes | 55 | 1,609,612,633,721 | 0 entries, ≈ 0.000000 TB | 0 | 1.609613 TB / 1.463934 TiB |
| Original spreadsheet selection | 75 | 1,609,612,633,721 | 20 entries, ≈ 0.184994 TB | 0 | ≈ 1.794607 TB / 1.632185 TiB |
| Default: spreadsheet selection + LANL | 86 | 1,609,612,633,721 | 29 entries, ≈ 3.803384 TB | 2 | ≈ 5.412997 TB / 4.923092 TiB |

Exact RAW payload: **1,609,612,633,721 bytes**. Formula: sum of width × height × depth × bytes per scalar over 55 published RAW paths. All 55 paths and scalar types match the publisher-maintained manifest. The result excludes detached NRRD headers. It is a calculated payload total, not a measurement of bytes transferred from the server.

The default known subtotal is approximately **5.413 TB (4.923 TiB), plus unknown sizes** for Bowtie round 3 and Asteroid Impact. Of the 86 selected entries, 55 have exact calculated RAW payloads and 29 use rounded download sizes. Approximate byte fields preserve the arithmetic conversion of displayed values, not byte-level measurement precision.

1 TB = 10^12 bytes. 1 TiB = 2^40 bytes. Publisher MB/GB labels are interpreted as decimal where no exact bytes are available. LANL Apache K/M/G/T listings are interpreted as binary; these are still rounded estimates. This assumption is visible in the individual rows.

## Problems in the input workbook

- `H98` uses `SUM(ScientificDatasets[Download GB])`, so its 4,672.687733721 GB sum ignores the Quantity column. It includes large entries whose quantity is zero.
- `I98` similarly sums all working-size values, producing 983,165.858311073 GB and mixing hosted database capacity with local storage. It is not the selected local working requirement.
- Missing-working formulas reference `#REF!`; missing-source formulas contain `#REF!` errors. They cannot support a verified/complete claim.
- Rounded source sizes were stored as numerical GB values, but formatting and many decimal places do not turn them into exact bytes.

## Representation and overlap decisions

- Kept one copy of each published RAW URL. No duplicate RAW URLs were found among the 55 entries.
- Retained Stanford Bunny CT (360 slices) and Open SciVis Bunny CT (361 slices) as distinct representations. Their underlying scan may overlap; no checksum-level equivalence is asserted.
- Retained MR Brain and MRI Woman separately; equal dimensions do not prove identical content.
- Retained the Miranda variants separately with their distinct scopes.
- HD(CP)² single-step and four-hour series cannot be selected simultaneously in the UI because the shorter product overlaps the longer scope.
- LANL archive files and their expanded directories are not both counted. Indexing `.db` files, PDFs, server configuration and ancillary metadata are excluded from the dataset download plan.
- HEAT selection is full CYL fp16 archive plus original PLI archive. The half-resolution and alternative expanded/fp16 representations are excluded. This is a defined download plan, not a full repository mirror.
- JHTDB hosted capacities, the four per-field/time climate payloads, and COVIS with unspecified extent are excluded from the default download plan. They remain discoverable in the catalog.

## LANL coverage

| Collection | Sized scope | Size evidence / remaining gap |
|---|---|---|
| Cloverleaf | One published archive | Listing: 172M; interpreted as ~172 MiB. |
| Monopoly steel XCT | Three published archives | Listing: 5.9G + 6.1G + 7.9G; interpreted as ~19.9 GiB. |
| Gray–Scott reaction diffusion | One published archive | Listing: 118M; interpreted as ~118 MiB. |
| Poisson electrostatics | One published archive | Listing: 40M; interpreted as ~40 MiB. |
| Heat equations | One published archive | Listing: 43M; interpreted as ~43 MiB. |
| HEAT shock simulations | CYL full fp16 + PLI original archives | 134G + 2.6T; interpreted as ~134 GiB + ~2.6 TiB. |
| Bowtie manufacturing, rounds 1 & 2 | One published archive | Listing: 2.2G; interpreted as ~2.2 GiB. |
| Bowtie manufacturing, round 3 | Five sample folders; multiple image views | Full collection bytes unknown. |
| FireTec wildfire simulations | 527 VTS files, seven simulations | 527 listed files × ~1.0 GiB per file. |
| Asteroid impact | Seven simulations; multiple resolutions | Full collection bytes unknown. |
| NIF fusion simulation | 20 HDF5 plot files | 898M + 970M + 22.2G; Apache units interpreted as binary. |

**FireTec:** counted the filenames actually listed across seven directories: backcurve40 70; backcurve80 75; backcurve320 74; headcurve40 72; headcurve80 90; headcurve320 73; valley_losAlamos 73. Total: **527 VTS files**. Missing timestep filenames were not fabricated. Each listing shows 1.0G, so the combined size is approximately 527 GiB. All 527 URLs are included as explicit file links.

**NIF:** 20 plot-file entries: 898M + 970M + 22.2G, interpreted as approximately 24.02421875 GiB. The arithmetic is exact on rounded inputs; actual bytes remain unmeasured.

## Working-size limits

The default calculated working-payload subtotal is 1,731,528,798,873 bytes, plus rounded working values of approximately 591.881 GB; 15 selected entries have unknown working size. Do not interpret this as a complete unpacked, peak disk, RAM, or cache requirement. RAW payload is counted once, rather than adding identical download and working values. Archives and containers need separate unpacked inventories.

HACC Dataset2 and the large 3072³ Miranda package retain the input values in provenance fields, but their specific particle-count/type metadata could not be retrieved. Their input working calculations are excluded from the verified working subtotal. S3D remains unknown at whole-package level: a per-snapshot calculation cannot establish all archive contents.

## Verification limits

Primary publisher pages were checked through web retrieval. The Open SciVis homepage and several binary/Globus/registration endpoints could not be retrieved. All 55 Open SciVis file specifications were therefore cross-checked against the publisher repository. Some web results are cached; their retrieval is metadata evidence, not a live file-service availability guarantee.

A direct HEAD probe of the Aneurism RAW URL returned HTTP 403 in this environment. Binary bodies, HTTP Content-Length values and checksums were not verified. Every record states this distinction; no file link is labeled as a successful live transfer. The supplied HEAD verifier can record actual lengths from a network with access, without downloading large datasets.

Bowtie round 3 and Asteroid Impact require complete recursive inventories and representation choices to produce full download totals. Exact transfer lengths are also needed for every rounded package. This delivery does not claim that adding directory display sizes produces a correct byte-exact grand total.

## Source index

- [Publisher metadata](https://g-d0cd3f.fd635.8443.data.globus.org/raw-data/EXASKY/HACC/EXASKY-HACC-data-medium-size-template_data.txt)
- [Publisher metadata](https://g-d0cd3f.fd635.8443.data.globus.org/raw-data/EXASKY/NYX/template_data.txt)
- [Publisher metadata](https://g-d0cd3f.fd635.8443.data.globus.org/raw-data/Miranda/template_data-miranda-3072x3072x3072.txt)
- [Publisher metadata](https://g-d0cd3f.fd635.8443.data.globus.org/raw-data/S3D/template.txt)
- [Publisher metadata](https://g-d0cd3f.fd635.8443.data.globus.org/raw-data/SCALE_LETKF/template_data.txt)
- [Publisher RAW manifest](https://github.com/sci-visus/open-scivis-datasets/blob/main/test.py)
- [Publisher metadata](https://graphics.stanford.edu/data/voldata/)
- [Publisher metadata](https://kaust-vislab.github.io/SciVis2020/data.html)
- [Open SciVis public catalog (retrieval unavailable)](https://klacansky.com/open-scivis-datasets/)
- [LANL collection index](https://oceans11.lanl.gov/)
- [LANL archive listing](https://oceans11.lanl.gov/bowtie_1_2/data/LA-UR-25-28525-bowtie/)
- [LANL file listing](https://oceans11.lanl.gov/bowtie_3/data/)
- [LANL file listing](https://oceans11.lanl.gov/cloverleaf/data/)
- [LANL file listing](https://oceans11.lanl.gov/deepwaterimpact/data/)
- [LANL file listing](https://oceans11.lanl.gov/electrostaticEquations/data/)
- [mountain_backcurve320: 74 files](https://oceans11.lanl.gov/firetec/data/mountain_backcurve320/)
- [mountain_backcurve40: 70 files](https://oceans11.lanl.gov/firetec/data/mountain_backcurve40/)
- [mountain_backcurve80: 75 files](https://oceans11.lanl.gov/firetec/data/mountain_backcurve80/)
- [mountain_headcurve320: 73 files](https://oceans11.lanl.gov/firetec/data/mountain_headcurve320/)
- [mountain_headcurve40: 72 files](https://oceans11.lanl.gov/firetec/data/mountain_headcurve40/)
- [mountain_headcurve80: 90 files](https://oceans11.lanl.gov/firetec/data/mountain_headcurve80/)
- [valley_losAlamos: 73 files](https://oceans11.lanl.gov/firetec/data/valley_losAlamos/)
- [LANL file listing](https://oceans11.lanl.gov/grayScottSimulation/data/)
- [CYL listing](https://oceans11.lanl.gov/heat/data/cyl/)
- [PLI listing](https://oceans11.lanl.gov/heat/data/pli/)
- [LANL file listing](https://oceans11.lanl.gov/heatEquations/data/)
- [LANL archive listing](https://oceans11.lanl.gov/monopoly/data/LA-UR-25-28633_Monopoly_Hotel_Data/)
- [LANL plot-file listing](https://oceans11.lanl.gov/nif/data/N210201-001_3D_r2/)
- [Publisher metadata](https://scivis2017.dkrz.de/data.html)
- [Publisher metadata](https://scivis2021.netlify.app/data/)
- [Publisher metadata](https://sciviscontest2024.github.io/data/)
- [Publisher metadata](https://sciviscontest2026.github.io/data/home)
- [Publisher metadata](https://sdrbench.github.io/datasets.html)
- [Publisher metadata](https://turbulence.idies.jhu.edu/home)
- [Publisher metadata](https://www.uni-muenster.de/Voreen/download/workspaces_and_data_sets.html)
- [Publisher metadata](https://zenodo.org/records/10519411)
- [Publisher metadata](https://zenodo.org/records/15189444)
