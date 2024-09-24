
This archive includes data and code from Linck & Cadena In press, *Molecular Ecology*.  

### Files:

`*.tsv`: Metadata for available reference genomes from NCBI's Genome Browser.

`*.zip`: Zipped GBIF occurence datasets (DOIs for each are referenced in the manuscript) for different taxonomic groups and species lists. 

`congen_lit_review.csv`: A comma-delimited table of summarizing the study's literature review. 

### Scripts: 

`01_analysis.Rmd`: Rmarkdown notebook to run all analyses and produce Figure 1. 

`ncbi.md`: Shell commands to download metadata associated with reference genomes from NCBI's command-line tools (generates up-to-date versions of all `.tsv` files). 

### Instructions:

To replicate analyses in Linck & Cadena, download the contents of the archive and place in a local directory titled `lat_grad_genome`. Within this folder, create a second directory titled `data`, and place all `.tsv`, `.csv`, and `.zip` files within it. Knit `01_analysis.Rmd`. 