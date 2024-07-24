# Workflow 1: RNA Seq Centric Workflow

## Goal
User compares their own RNA Seq data to a gene list set from a published study.

## RNA Seq data:
- LPS stimulated (0 vs 30 minutes) immortalized mouse macrophages (IMM’s).
- Lipopolysaccharide regulates the Macrophage RNA-Binding Proteome.
- DOI: [10.1021/acs.jproteome.3c00838](https://doi.org/10.1021/acs.jproteome.3c00838)

## Gene list publication data: 
- Resident and elicited murine macrophages differ in their expression of their glycomes and glycan-binding proteins.
- DOI: [10.1016/j.chembiol.2020.12.005](https://doi.org/10.1016/j.chembiol.2020.12.005)

## Schematic of Workflow 1:

### Schematic in Words:
1. User inputs a RNA Seq counts matrix and metadata.
2. Resolved into AnnData matrix.
3. Limma-Voom to calculate differentially expressed genes (DEGs).
4. Subset up, down, and highest scored DEGs.
5. ENRICHR analysis of each subset and highlights connected genes.
6. Extract the enriched glycans representative of the counts data.
7. Get glycoenzyme data for glycans of interest.
8. ENRICHR analysis of glycoenzymes data and extract enriched pathways.
9. Upload a literature based gene list from a published study.
10. ENRICHR analysis of published gene list.
11. Compare enriched pathways between the different arms of the workflow.

*This workflow allows the user to upload their own RNA seq experiments and compare the generated DEGs and subsequent pathway analysis data to published studies. A powerful and quick to use tool to compare lab generated data to the existing literature.*
