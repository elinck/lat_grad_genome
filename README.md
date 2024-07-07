## A latitidunal gradient of reference genomes?

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

...insects:

```
datasets summary genome taxon insecta --reference --as-json-lines | dataformat tsv genome --fields accession,assminfo-name,annotinfo-name,annotinfo-release-date,organism-name > insects.tsv
```


...flowering plants: 

```
datasets summary genome taxon mesangiospermae --reference --as-json-lines | dataformat tsv genome --fields accession,assminfo-name,annotinfo-name,annotinfo-release-date,organism-name > flowers.tsv
```

...ray-finned fish: 

```
datasets summary genome taxon Actinopterygii --reference --as-json-lines | dataformat tsv genome --fields accession,assminfo-name,annotinfo-name,annotinfo-release-date,organism-name > actinopterygii.tsv
```

...and amphibians:

```
datasets summary genome taxon amphibia --reference --as-json-lines | dataformat tsv genome --fields accession,assminfo-name,annotinfo-name,annotinfo-release-date,organism-name > amphibia.tsv
```