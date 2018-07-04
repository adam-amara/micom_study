## Materials

This repository contains additional matrials for the following preprint:

> Micom: metagenome-scale modeling to infer metabolic interactions in the microbiota.
> Christian Diener and Osbaldo Resendis-Antonio
> https://doi.org/10.1101/361907

Project to study the approaches from micom in a metagenomic shotgun data set
of 186 individuals.

All scripts are provided as Python 3 code. libraries required to reproduce
figures and data processing csan be installed using the provided requirements
file:

```bash
pip install --user -r requirements.txt
```

### Subfolders

See each subfolder for detailed desription of contained files.

[*figures*](/figures)
Scripts to reproduce the figures in the publication.

[*results*](/results)
Intermediate results required for figures.

[*workflows*](/workflows)
Long running parallel analyses that produce the results provided in the
previous folder.

### Scripts

**genera.py**
Reads the genus-level abundances and combines them with the AGORA models
for each genus.
Output: `genera.csv`

**taxa_stats.py**
Counts the fraction of reads assigned to each taxonomic rank and the fraction
of reads that has at least one represenative in the AGORA models.
Output: a text table

### Files

**recent.csv**
Provides a list of samples and the corresponding [SRA](https://www.ncbi.nlm.nih.gov/sra) abundances.




