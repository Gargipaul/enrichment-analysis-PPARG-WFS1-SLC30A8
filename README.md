# 🧬 Functional Annotation and Pathway Enrichment of Type 2 Diabetes-associated SNPs

## 📌 Abstract

Type 2 Diabetes (T2D) is a complex metabolic disease influenced by genetic factors regulating insulin sensitivity and β-cell function. This project investigates the expression and statistical significance of three consistently associated T2D genes—**PPARG**, **WFS1**, and **SLC30A8**—using genome-wide significant single nucleotide polymorphisms (SNPs) from the DIAGRAM GWAS dataset. Functional annotation was performed using g:Profiler, and gene-level differential expression was visualized via volcano plots using Python. Notably, **PPARG** and **WFS1** showed strong upregulation (log₂ fold change > 2.5, p < 0.001), while **SLC30A8** showed a modest but borderline significant signal. This integrative analysis highlights potential therapeutic targets and demonstrates the power of visualization in genomic data interpretation.

---

## 🗂️ Project Structure
## 📁 annotation/ 
### Jupyter notebook for SNP annotation

📄 plotting.ipynb 
### Volcano plot visualization code

📄 cleaned_merged_gwas_diagram_annotations.xlsx
### Merged GWAS and annotation data

📄 genome_wide_significant_snps.xlsx 
### Source GWAS SNPs

📄 high_impact_filtered_variants.xlsx 
### Filtered high-impact SNPs

📄 Final_GO.png 
### g:Profiler GO enrichment plot

📄 manhattan_plot_labeled.png 
### Optional labeled Manhattan plot

---

## 🔬 Data and Methods

### 📊 Data Source
- **GWAS Dataset**: *DIAGRAMv3.2012DEC17*  
  Genome-wide significant SNPs (p < 5×10⁻⁸)

### 🧰 Functional Annotation
- **Tool**: [g:Profiler](https://biit.cs.ut.ee/gprofiler/)
- **Output**: Enriched Gene Ontologies (GO) and pathway annotations

### 🧬 Genes of Interest
- **PPARG** – Nuclear receptor influencing adipogenesis and insulin sensitivity
- **WFS1** – Regulates ER stress and pancreatic β-cell function
- **SLC30A8** – Zinc transporter important for insulin granule formation

### 📐 Statistical Thresholds
- **Significance**: p < 0.05
- **Visualization**: Volcano plot  
  - X-axis: log₂ fold change  
  - Y-axis: –log₁₀ p-value
---

## Results Summary

| Gene      | log₂ Fold Change | P-value  | Significance       |
|-----------|------------------|----------|--------------------|
| PPARG     | 3.0              | 0.0001   | ✅ Highly significant |
| WFS1      | 2.5              | 0.001    | ✅ Highly significant |
| SLC30A8   | 1.2              | 0.05     | ⚠️ Borderline significance |

---

## 🚀 How to Reproduce

1. Clone this repository:
   ```
   git clone https://github.com/Gargipaul/enrichment-analysis-PPARG-WFS1-SLC30A8.git
   cd enrichment-analysis-PPARG-WFS1-SLC30A8

## 📄 License
This project is open-source under the MIT License.

## 🙏 Acknowledgments
- DIAGRAM Consortium for providing GWAS meta-analysis data

- g:Profiler for gene ontology and functional annotation tools

- Python ecosystem – including pandas, seaborn, and matplotlib for visualization

### 💡 *For academic collaboration or questions, feel free to reach out via [GitHub](https://github.com/Gargipaul).*


