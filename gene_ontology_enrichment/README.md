# Gene Set Enrichment Analysis

## About
Enrichment of X gene set library terms were performed using the Enrichr package. UniProt protein identifiers were mapped to Entrez gene symbols as input for Enrichr. Custom background gene sets were established using all experimentally detected proteins. P-values were computed from Fisher’s exact test to determine the significance of each enriched term. The negative log of these p-values were calculated using R. 

## Set Up
```
pip3 install gseapy
```

## Usage
Input file, such as <compiled_proteins.csv>, with protein and gene names columns are required. Additional quantitative columns, such as Log2 ratios, can be used for further analysis.

### Citataion
Yan T, Julio AR, Villanueva M, Jones AE, Ball AB, Boatner LM, Turmon AC, Nguyễn KB, Yen SL, Desai HS, Divakaruni AS, Backus KM. Proximity-labeling chemoproteomics defines the subcellular cysteinome and inflammation-responsive mitochondrial redoxome. Cell Chem Biol. 2023 Jul 20;30(7):811-827.e7. doi: 10.1016/j.chembiol.2023.06.008. Epub 2023 Jul 6. PMID: 37419112; PMCID: PMC10510412.
