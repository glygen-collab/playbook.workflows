# Workflow 2: Biomarker Drug Discovery Integrated with Glycomics Data

## Goal
User has a biomarker (experimentally validated or a candidate), identified median tissue expression, FDA approved drugs specific to that tissue type, pulls information from GlyGEN on the gene/protein product regarding glycoforms. Glycosylation-related enzymes are then assessed as potential drug candidates. List of tissue-specific and glycosylation enzyme drugs are compared in Excel.

### Biomarker: CA-125
This biomarker was chosen due to its historical use as a biomarker in ovarian cancer. The gene which encodes this glycoprotein is MUC16, and it is highly glycosylated (both N- and O- linked). MUC16 is highly expressed in fallopian tube tissue, indicative of its biological underpinnings in ovarian cancer.
DOI: [10.1016/j.bbcan.2021.188503](https://doi.org/10.1016/j.bbcan.2021.188503)

## Schematic of Workflow 2

### Schematic in Words:
1. Biomarker is chosen by the user (CA-125), the corresponding gene becomes the first input (MUC16).
2. Median tissue expression is assessed using GTEx.
3. Tissues are Z-scored and plotted with a horizontal bar plot.
4. One particular tissue type is then chosen for further analysis (Fallopian tube).
5. Tissue-drug co-mentions in PubMed are assessed using DrugRif.
6. Top scored drugs are listed by Z-score.
7. FDA approved drugs are extracted from the scored list for that particular tissue.
8. Based on the gene input, GlyGEN is searched to assess protein products.
9. GlyGEN is then searched to assess glycosylation sites and lists the known glycans.
10. Out of the list of glycans, some are chosen for further analysis by searching GlyGEN for glycan information based on associated GlyToucan IDs.
11. Using GlyGEN, information regarding the construction of each glycan (glyco-enzymes) is extracted and a list of enzymes is generated.
12. Some of those enzymes are chosen for further analysis, and their corresponding genes are inputted.
13. PubMed is then searched according to drug-gene co-mentions using AutoRif.
14. FDA approved drugs are then extracted from the drug lists and compared to the tissue-specific drug list generated earlier to see if there are any matches via Excel.

*This workflow allows the user to assess a biomarker’s median tissue expression and examine tissue-specific drugs. Glycosylation data is gathered for the biomarker, and glycans are profiled to examine glycosylation enzymes which can be potential drug targets. The list of FDA-approved drugs for both the tissue-specific and glycosylation enzymes are compared to elucidate potential therapeutic interventions relevant to a particular phenotype.*
