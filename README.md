# Scientific visualization catalog

https://huyen-nguyen.github.io/scivis-catalog/

The catalog contains 103 entries. 

## Download totals

The default known subtotal is approximately **5.413 TB (4.923 TiB), plus unknown sizes** for Bowtie round 3 and Asteroid Impact. Of the 86 selected entries, 55 have exact calculated RAW payloads and 29 use rounded download sizes. Approximate byte fields preserve the arithmetic conversion of displayed values, not byte-level measurement precision.

1 TB = 10^12 bytes. 1 TiB = 2^40 bytes. Publisher MB/GB labels are interpreted as decimal where no exact bytes are available. LANL Apache K/M/G/T listings are interpreted as binary; these are still rounded estimates. This assumption is visible in the individual rows.

## Coverage Examples

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

## Source index

(Draft version - needs editing)

- [HACC metadata](https://g-d0cd3f.fd635.8443.data.globus.org/raw-data/EXASKY/HACC/EXASKY-HACC-data-medium-size-template_data.txt)
- [NYX metadata](https://g-d0cd3f.fd635.8443.data.globus.org/raw-data/EXASKY/NYX/template_data.txt)
- [Miranda metadata](https://g-d0cd3f.fd635.8443.data.globus.org/raw-data/Miranda/template_data-miranda-3072x3072x3072.txt)
- [S3D metadata](https://g-d0cd3f.fd635.8443.data.globus.org/raw-data/S3D/template.txt)
- [SCALE_LETKF metadata](https://g-d0cd3f.fd635.8443.data.globus.org/raw-data/SCALE_LETKF/template_data.txt)
- [Open-scivis RAW manifest](https://github.com/sci-visus/open-scivis-datasets/blob/main/test.py)
- [Stanford metadata](https://graphics.stanford.edu/data/voldata/)
- [SciVis2020 metadata](https://kaust-vislab.github.io/SciVis2020/data.html)
- [Open SciVis public catalog (retrieval unavailable)](https://klacansky.com/open-scivis-datasets/)
- [LANL collection index](https://oceans11.lanl.gov/)
- [bowtie_1_2 archive listing](https://oceans11.lanl.gov/bowtie_1_2/data/LA-UR-25-28525-bowtie/)
- [bowtie_3 file listing](https://oceans11.lanl.gov/bowtie_3/data/)
- [cloverleaf file listing](https://oceans11.lanl.gov/cloverleaf/data/)
- [deepwaterimpact file listing](https://oceans11.lanl.gov/deepwaterimpact/data/)
- [electrostaticEquations file listing](https://oceans11.lanl.gov/electrostaticEquations/data/)
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
- [LANL heatEquations file listing](https://oceans11.lanl.gov/heatEquations/data/)
- [LANL monopoly archive listing](https://oceans11.lanl.gov/monopoly/data/LA-UR-25-28633_Monopoly_Hotel_Data/)
- [LANL plot-file listing](https://oceans11.lanl.gov/nif/data/N210201-001_3D_r2/)
- [scivis2017 metadata](https://scivis2017.dkrz.de/data.html)
- [scivis2021 metadata](https://scivis2021.netlify.app/data/)
- [sciviscontest2024 metadata](https://sciviscontest2024.github.io/data/)
- [sciviscontest2026 metadata](https://sciviscontest2026.github.io/data/home)
- [sdrbench metadata](https://sdrbench.github.io/datasets.html)
- [turbulence metadata](https://turbulence.idies.jhu.edu/home)
- [Voreen metadata](https://www.uni-muenster.de/Voreen/download/workspaces_and_data_sets.html)
- [Publisher metadata](https://zenodo.org/records/10519411)
- [Publisher metadata](https://zenodo.org/records/15189444)