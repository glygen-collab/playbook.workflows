**Workflow 1: RNA Seq Centric Workflow**

**Goal:** User compares their own RNA Seq data to a gene list set from a published study.

**Motivation:** This is an easy way to identify DEGs and phenotypes associated with them as well as compare the outputs to what has been found in the literature.

**RNA Seq data:**

LPS stimulated (0 vs 30 minutes) immortalized mouse macrophages (IMM’s).

*Lipopolysaccharide regulates the Macrophage RNA-Binding Proteome.*

DOI: [10.1021/acs.jproteome.3c00838](https://doi.org/10.1021/acs.jproteome.3c00838)

**Gene list publication data:** 

*Resident and elicited murine macrophages differ in their expression of their glycomes and glycan-binding proteins.*

DOI: [10.1016/j.chembiol.2020.12.005](https://doi.org/10.1016%2Fj.chembiol.2020.12.005)

**Schematic of Workflow 1:**

![](Aspose.Words.8e75bfd3-a81f-4117-b16a-4082383b1c94.001.png)

**Description of Steps:**

1) User inputs a RNA Seq counts matrix and metadata. 
1) Resolved into AnnData matrix.
1) Limma-Voom to calculate differentially expressed genes (DEGs).
1) Subset up, down, and highest scored DEGs.
1) ENRICHR analysis of each subset and highlights connected genes
1) Extract the enriched glycans representative of the counts data.
1) Get glycoenzyme data for glycans of interest.
1) ENRICHR analysis of glycoenzymes data and extract enriched pathways.
1) Upload a literature based gene list from a published study.
1) ` `ENRICHR analysis of published gene list.
1) ` `Compare enriched pathways between the different arms of the workflow.

**Input:** RNA Seq counts, metadata, and a gene list from the literature to compare with.

**Output:** Enriched pathways for the RNA Seq counts, implicated glycosylation enzymes, enriched pathways for the literature based gene list.

**Shortcomings:** All shortcomings were documented on the github ticket reporting system, this particular project had issues with the WikiPathway / STRING nodes, metadata matrix upload, and RNA Seq counts matrix upload process.




\*This workflow allows the user to upload their own RNA seq experiments and compare the generated DEGs and subsequent pathway analysis data to published studies. A powerful and quick to use tool to compare lab generated data to the existing literature.\*



