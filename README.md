## Downloading NCBI SRA metadata using Geofetch vs SRA Run Selector 

### Tools 

- [geofetch](http://geofetch.databio.org/en/latest/)
- [NCBI SRA Run Selector](https://www-ncbi-nlm-nih-gov.ezproxy.u-pec.fr/Traces/study/?)


### Installing geofetch  

```bash
pip install geofetch # Installation 

geofetch --help # Manual 
```


### Downloading GSE157852 metadata

1. via **geofetch** 
- Commend (if you want to download a subset of samples, see [this](http://geofetch.databio.org/en/latest/file-specification/))

```bash
geofetch -i GSE157852 --just-metadata
```

- Output files

  - [GSE157852/GSE157852_annodation.csv](https://github.com/Mira0507/sra_metadata/blob/master/GSE157852/GSE157852_annotation.csv): PEP sample table 
  - [GSE157852/GSE157852_config.yaml](https://github.com/Mira0507/sra_metadata/blob/master/GSE157852/GSE157852_config.yaml): PEP project config file
  - [GSE157852/GSE157852_GSE.soft](https://github.com/Mira0507/sra_metadata/blob/master/GSE157852/GSE157852_GSE.soft) 
  - [GSE157852/GSE157852_GSM.soft](https://github.com/Mira0507/sra_metadata/blob/master/GSE157852/GSE157852_GSM.soft) 
  - [GSE157852/GSE157852_SRA.csv](https://github.com/Mira0507/sra_metadata/blob/master/GSE157852/GSE157852_SRA.csv)
  - [GSE157852/GSE157852_SRA_filt.csv](https://github.com/Mira0507/sra_metadata/blob/master/GSE157852/GSE157852_SRA_filt.csv)


2. via **NCBI SRA Run Selector**

- Manually downloading metadata (see [tutorial video](https://www.youtube.com/watch?v=Ww_OTe3M_94))
- Output file: [SraRunTable.txt](https://github.com/Mira0507/sra_metadata/blob/master/SraRunTable.txt)




