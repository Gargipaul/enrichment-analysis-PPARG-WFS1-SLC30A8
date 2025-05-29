# Functional Annotation and Pathway Enrichment of Type 2 Diabetes-associated SNPs

## Abstract

Type 2 Diabetes (T2D) is a complex metabolic disease influenced by genetic factors regulating insulin sensitivity and β-cell function. This project investigates the expression and statistical significance of three consistently associated T2D genes—**PPARG**, **WFS1**, and **SLC30A8**—using genome-wide significant single nucleotide polymorphisms (SNPs) from the DIAGRAM GWAS dataset. Functional annotation was performed using g:Profiler, and gene-level differential expression was visualized via volcano plots using Python. Notably, **PPARG** and **WFS1** showed strong upregulation (log₂ fold change > 2.5, p < 0.001), while **SLC30A8** showed a modest but borderline significant signal. This integrative analysis highlights potential therapeutic targets and demonstrates the power of visualization in genomic data interpretation.

---

## Project Structure

📁 annotation/ # Jupyter notebook for annotating SNPs
📄 plotting.ipynb # Volcano plot visualization code
📄 cleaned_merged_gwas_diagram_annotations.xlsx # Merged GWAS and annotation data
📄 genome_wide_significant_snps.xlsx # Source GWAS SNPs
📄 high_impact_filtered_variants.xlsx # Filtered high-impact SNPs
📄 Final_GO.png # g:Profiler GO enrichment plot
📄 manhattan_plot_labeled.png # Optional labeled Manhattan plot
📜 LICENSE # MIT License

---

## Methodology

### 1. **Data Acquisition**
- GWAS SNPs associated with T2D (p < 5 × 10⁻⁸) were sourced from the [DIAGRAM v3.2012DEC17](https://diagram-consortium.org/downloads.html) study.
- SNPs were curated into `genome_wide_significant_snps.xlsx`.

### 2. **Functional Annotation**
- Functional profiling was performed using [g:Profiler](https://biit.cs.ut.ee/gprofiler/gost), generating gene ontologies and pathway enrichments.
- Genes PPARG, WFS1, and SLC30A8 were selected based on biological relevance and annotation output.

### 3. **Differential Expression Analysis**
- Gene-level log₂ fold change and p-values were compiled in `cleaned_merged_gwas_diagram_annotations.xlsx`.
- Threshold for significance: **p < 0.05**

### 4. **Visualization**
- Volcano plots were generated using `plotting.ipynb` with:
  - **X-axis:** log₂(fold change)
  - **Y-axis:** –log₁₀(p-value)
  - Interactive rendering using **Plotly**

---

## Results Summary

| Gene      | log₂ Fold Change | P-value  | Significance       |
|-----------|------------------|----------|--------------------|
| PPARG     | 3.0              | 0.0001   | **Highly significant** |
| WFS1      | 2.5              | 0.001    | **Highly significant** |
| SLC30A8   | 1.2              | 0.05     | Borderline         |

- **PPARG**: Upregulated, consistent with role in adipogenesis and insulin sensitivity.
- **WFS1**: Upregulated, involved in ER stress and β-cell function.
- **SLC30A8**: Marginal change, relevant to insulin granule formation.

---

## How to Reproduce

1. Clone the repository:

```bash
git clone https://github.com/Gargipaul/enrichment-analysis-PPARG-WFS1-SLC30A8.git
cd enrichment-analysis-PPARG-WFS1-SLC30A8
---

## Install required Python libraries

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
DIAGRAM Consortium for GWAS data

g:Profiler for functional annotation tools


