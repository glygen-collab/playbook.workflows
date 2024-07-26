**Workflow 2: Biomarker Drug Discovery Integrated with Glycomics Data**

**Goal:** User has a biomarker (experimentally validated or a candidate), identified median tissue expression, FDA approved drugs specific to that tissue type, pulls information from GlyGEN on the gene / protein product regarding glycoforms. Glycosylation related enzymes are then assessed as potential drug candidates. List of tissue specific and glycosylation enzyme drugs are compared in excel.

**Motivation:** To check if there are tissue and glycosylation enzyme specific drug targets that are similar for a given biomarker.

**Biomarker: CA-125**

This biomarker was chosen due to its historical use as a biomarker in ovarian cancer. The gene which encodes this glycoprotein is MUC16 and it is highly glycosylated (Both N- and O- linked). MUC16 is highly expressed in fallopian tube tissue indicative of its biological underpinnings in ovarian cancer.

DOI: [10.1016/j.bbcan.2021.188503](https://doi.org/10.1016/j.bbcan.2021.188503)


**Schematic of Workflow 2:**

![](Aspose.Words.e17c7528-9304-4244-bd46-743652da8787.001.png)

**Description of steps:**

1) Biomarker is chosen by the user (CA-125), the corresponding gene becomes the first input (MUC16).
1) Median tissue expression is assessed using GTEx.
1) Tissues are Z-scored and plotted with horizontal bar plot.
1) One particular tissue type is then chosen for further analysis (Fallopian tube).
1) Tissue-Drug co-mentions in PubMed are assessed using DrugRif.
1) Top scored drugs are listed  by Z-score.
1) FDA approved drugs are extracted from the scored list for that particular tissue.
1) Based on the gene input, GlyGEN is searched to assess protein products. 
1) GlyGEN is then searched to assess glycosylation sites and lists the known glycans.
1) Out of the list of glycans, some are chosen for further analysis by searching GlyGEN for glycan information based on associated GlyToucan ID’s.
1) Using GlyGEN, information regarding the construction of each glycan (glyco-enzymes) is extracted and a list of enzymes is generated.
1) Some of those enzymes are chosen for further analysis, and their corresponding genes are inputted.
1) Pubmed is then searched according to Drug-gene co-mentions using AutoRif.
1) FDA approved drugs are then extracted from the drug lists and compared to the tissue specific drug list generated earlier to see if there are any matches via Excel.

**Input:** A gene which encodes a biomarker of interest.

**Output:** A list of drugs specific to the tissue type of interest and glycosylation related enzymes enriched for that biomarker.

**Shortcomings:** All documented within the Github ticket reporting system.


\*This workflow allows the user to assess a biomarker’s median tissue expression and examine tissue specific drugs. Glycosylation data is gathered for the biomarker and glycans are profiled to examine glycosylation enzymes which can be potential drug targets. The list of FDA approved drugs for both the tissue specific and glycosylation enzymes are compared to elucidate potential therapeutic interventions relevant to a particular phenotype.\*




