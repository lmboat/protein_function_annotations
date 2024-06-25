# protein_function_annotations

## About
Protein functions are based on annotations in the UniProtKB/Swiss-Prot database (ex. 2401-release), Human Protein Atlas (ex. version 22.0) and the ScaPD database. UniProt keywords were parsed to classify proteins into five broad functional categories: chaperones/transporter/channel/receptor, enzyme, nucleic acid and small molecule binding, scaffolding/modulator/adaptor, transcription factor/regulator and uncategorized. Transcription factors, channels and transporters were also found using protein class descriptions from the HPA. In addition, examples of experimentally validated scaffolding proteins were collected from the ScaPD database. For proteins in more than one category, annotations were prioritized based on the following: enzyme > chaperones/transporter/channel/receptor > scaffolding/modulator/adaptor > transcription factor/regulator > nucleic acid and small molecule binding.

## Setup
Download most recent version of UniProtKB proteins with associated keywords & HPA FDA annotations. Place downloaded files into the data folder.

### UniProtKB
https://rest.uniprot.org/uniprotkb/search?fields=accession%2Creviewed%2Cid%2Cprotein_name%2Cgene_names%2Corganism_name%2Clength%2Cgene_primary%2Cgene_synonym%2Ckeyword&format=xlsx&query=%28Human%29+AND+%28model_organism%3A9606%29+AND+%28reviewed%3Atrue%29&size=500

### Human Protein Atlas (HPA)
https://www.proteinatlas.org/about/download

## Usage
Input file, such as <uniprotkb_Human_AND_model_organism_9606_2024_06_25.xlsx>, with protein, gene names and keyword columns are required. Input file, such as <proteinatlas.tsv>, with protein and FDA approved drug target columns are required.

### Citataion
Boatner LM, Palafox MF, Schweppe DK, Backus KM. CysDB: a human cysteine database based on experimental quantitative chemoproteomics. Cell Chem Biol. 2023 Jun 15;30(6):683-698.e3. doi: 10.1016/j.chembiol.2023.04.004. Epub 2023 Apr 28. PMID: 37119813; PMCID: PMC10510411.
