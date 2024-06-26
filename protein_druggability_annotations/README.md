# ChEMBL, DrugBank and FDA Annotations

## About 
UniProt accessions were collected from proteins with available ChEMBL and DrugBank UniProt annotations (2401_release). Data from the Human Protein Atlas (HPA) version 22.0 was downloaded and parsed to obtain genes targeted by FDA approved drugs. Protein accessions provided by HPA were mapped to UniProtKB accessions to collect proteins targeted by FDA approved drugs. 

## Setup
Download most recent version of UniProtKB proteins with associated keywords & HPA FDA annotations. Place downloaded files into the data folder.
```
pip3 install venn
```

### UniProtKB
[https://rest.uniprot.org/uniprotkb/search?fields=accession%2Creviewed%2Cid%2Cprotein_name%2Cgene_names%2Corganism_name%2Clength%2Cgene_primary%2Cgene_synonym%2Ckeyword&format=xlsx&query=%28Human%29+AND+%28model_organism%3A9606%29+AND+%28reviewed%3Atrue%29&size=500](https://www.uniprot.org/uniprotkb?facets=model_organism%3A9606%2Creviewed%3Atrue&fields=accession%2Cid%2Cgene_names%2Cgene_primary%2Cgene_synonym%2Cprotein_name%2Cxref_hpa%2Cxref_chembl%2Cxref_drugbank&query=human&view=table)

### Human Protein Atlas (HPA)
https://www.proteinatlas.org/about/download

## Usage
Input file, such as <uniprotkb_Human_AND_model_organism_9606_2024_06_25.xlsx>, with protein, gene names and keyword columns are required. Input file, such as <proteinatlas.tsv>, with protein and FDA approved drug target columns are required.

### Citataion
Boatner LM, Palafox MF, Schweppe DK, Backus KM. CysDB: a human cysteine database based on experimental quantitative chemoproteomics. Cell Chem Biol. 2023 Jun 15;30(6):683-698.e3. doi: 10.1016/j.chembiol.2023.04.004. Epub 2023 Apr 28. PMID: 37119813; PMCID: PMC10510411.
