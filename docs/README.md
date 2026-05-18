# Chronic RAAS Suppression Drives Hypoxic Metabolic Reprogramming and Vascular Remodeling in the Kidney

Included here are the steps to analyze and product figures related to sequencing data from ["Chronic RAAS Suppression Drives Hypoxic Metabolic Reprogramming and Vascular Remodeling in the Kidney"](https://www.biorxiv.org/content/10.1101/2025.07.09.663881v1).

| ![graphical_abstract.png](img/graphical_abstract.png) |
|:--:|
| Chronic inhibition of the renin-angiotensin-aldosterone system (RAAS), a cornerstone of antihypertensive therapy, drives concentric arterial and arteriolar hypertrophy (CAAH), a progressive renal vascular disease whose molecular and metabolic basis remained undefined. Structural injury precedes detectable kidney function decline, creating a window during which disease advances silently. Three-dimensional vascular imaging reveals the extent of this remodeling, with luminal narrowing spanning the renal arterial tree. In mouse models of genetic and pharmacologic RAAS suppression, fate-mapping shows that renin cells and their smooth muscle descendants adopt inflammatory, fibrotic, and secretory states accompanying progressive vessel wall thickening. Integrating single-cell transcriptomics, proteomics, and metabolomics, we identify a conserved hypoxia-associated metabolic program marked by glycolytic shift and impaired mitochondrial function. This analysis also yields a 10-gene molecular signature of CAAH validated in independent human kidney disease cohorts. Candidate urinary biomarkers establish a framework for non-invasive detection of this incompletely understood vascular pathology. |

## Requirements

**Operating system:** Linux x86-64

**Estimated runtime:** approximately 48-72 hours end-to-end (raw data processing through figure generation)

**Key software:**

| Package | Version | Use |
|---|---|---|
| R | 4.4.1 | Primary analysis language |
| Python | 3.12.4 | KPMP Census data extraction |
| Seurat | 5.2.1 | scRNA-seq processing, clustering, visualization |
| Signac | 1.14.0 | Multiome (ATAC+RNA) processing |
| harmony | 1.2.0 | Batch integration |
| Monocle 3 | 1.3.7 | Trajectory inference |
| cicero | 1.3.9 | Co-accessibility analysis |
| Pando | 1.1.1 | Regulatory network inference |
| IReNA | 0.99.0 | GRN construction |
| GENIE3 | 1.26.0 | GRN construction |
| UCell | 2.8.0 | Gene signature scoring |
| SCPA | 1.6.2 | Pathway activity scoring |
| SiPSiC | 1.4.3 | Single-cell pathway scoring |
| edgeR | 4.4.0 | Differential expression |
| limma | 3.62.1 | Microarray differential expression (ERCB validation) |
| fgsea | 1.32.2 | Gene set enrichment analysis |

The complete reproducible environment specification (conda `environment.yml`) is in [Create Analysis Environment](2.Create_Analysis_Environment.md).

