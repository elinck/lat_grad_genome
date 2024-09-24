## NCBI downloads

We first downloaded metadata for all avian referemce genomes on the NCBI databases using  NCBI Datasets command-line tools:

```
datasets summary genome taxon aves --reference --as-json-lines | dataformat tsv genome --fields accession,assminfo-name,annotinfo-name,annotinfo-release-date,organism-name > birds.tsv
```

We'll repeat this for mammals: 

```
datasets summary genome taxon mammalia --reference --as-json-lines | dataformat tsv genome --fields accession,assminfo-name,annotinfo-name,annotinfo-release-date,organism-name > mammals.tsv
```

...and for squamates:

```
datasets summary genome taxon squamata --reference --as-json-lines | dataformat tsv genome --fields accession,assminfo-name,annotinfo-name,annotinfo-release-date,organism-name > squamates.tsv
```

...amphibians:

```
datasets summary genome taxon amphibia --reference --as-json-lines | dataformat tsv genome --fields accession,assminfo-name,annotinfo-name,annotinfo-release-date,organism-name > amphibia.tsv
```


...turtles: 

```
datasets summary genome taxon testudine --reference --as-json-lines | dataformat tsv genome --fields accession,assminfo-name,annotinfo-name,annotinfo-release-date,organism-name > testudines.tsv
```

...crocodiles: 

```
datasets summary genome taxon crocodylia --reference --as-json-lines | dataformat tsv genome --fields accession,assminfo-name,annotinfo-name,annotinfo-release-date,organism-name > crocodylia.tsv
```

...and tuataras: 

```
datasets summary genome taxon tuatara --reference --as-json-lines | dataformat tsv genome --fields accession,assminfo-name,annotinfo-name,annotinfo-release-date,organism-name > tuatara.tsv
```