---
layout: default
title: Home
---

# DoRothEA

## Overview
DoRothEA (Discriminant Regulon Expression Analysis) is a manually curated human regulon to estimate single sample transcription factor (TF) activities from gene expression data and consensus TF-target DNA binding networks. The approach assumes that the activity of a TF can be estimated from the mRNA levels of its direct target genes. We provide two versions of DoRothEA.
### DoRothEA (v1)
The first version of DoRothEA consists of 127 TFs targeting in total 7,445 genes. If you use this regulon please cite

>Garcia-Alonso, L., Iorio, F., Matchan, A., Fonseca, N., Jaaks, P., Peat, G., Pignatelli, M., Falcone, F., Benes, CH., Dunham, I., Bignell, GR., McDade, S., Garnett, MJ., Saez-Rodriguez, J. (2018). [Transcription Factor Activities Enhance Markers of Drug Sensitivity in Cancer.](http://cancerres.aacrjournals.org/content/early/2017/12/09/0008-5472.CAN-17-1679) Cancer Research, 78(3), 769–780.

```
@article{GarciaAlonso2018,
  doi = {10.1158/0008-5472.can-17-1679},
  url = {https://doi.org/10.1158/0008-5472.can-17-1679},
  year  = {2018},
  month = {feb},
  publisher = {American Association for Cancer Research ({AACR})},
  volume = {78},
  number = {3},
  pages = {769--780},
  author = {Luz Garcia-Alonso and Francesco Iorio and Angela Matchan and Nuno Fonseca and Patricia Jaaks and Gareth Peat and Miguel Pignatelli and Fiammetta Falcone and Cyril H. Benes and Ian Dunham and Graham Bignell and Simon S. McDade and Mathew J. Garnett and Julio Saez-Rodriguez},
  title = {Transcription Factor Activities Enhance Markers of Drug Sensitivity in Cancer},
  journal = {Cancer Research}
}
```
### DoRothEA (v2)
This new version of DoRothEA provides updated TF regulons derived from a broader collection of resources and strategies. The new TF regulons are signed (to account for activation/repression), when possible, and each TF-target interaction has been assigned a confidence score, ranging from A-E, being A the most confident interactions (see table below). You can find the regulons [here](https://github.com/saezlab/dorothea/tree/master/data/TFregulons/consensus/Robjects_VIPERformat/normal) 

| Confidence score  | #Interactions |
| ----------------- | ----- | 
| A                 |  5,869         |
| B                 |  8,991         |
| C                 |  17,519         | 
| D                 |  281,632        |
| E                 |  763,110       |
| Total             |  1,077,121       |

 You can find the preprint of the publication on [bioRxiv](https://www.biorxiv.org/content/early/2018/06/03/337915).

>Garcia-Alonso, L., Ibrahim, MM., Turei, D., Saez-Rodriguez, J. (2018). [Benchmark and integration of resources for the estimation of human transcription factor activities.](https://www.biorxiv.org/content/early/2018/06/03/337915) BioRxiv.

#### COMBAT vs nonCOMBAT
Before infering regulons from GTEx data we corrected for batch effects using COMBAT. If you are interested in regulons inferred from non-batch corrected GTEx data, we provide the data [here](https://github.com/saezlab/dorothea/tree/master/data/TFregulons/advanced_single_evidences/Robjects_VIPERformat/inferred_ARACNe/normal_GTEx_non_batch_corrected/tissue_specific).

#### GTEx vs TCGA
The default regulons contain among the other resources regulons derived from GTEx data using ARACNe. For users more interested in cancer specific applications we also provide DoRothEA with regulons infered from TCGA. Please find the consensus regulon [here](https://github.com/saezlab/dorothea/tree/master/data/TFregulons/consensus/Robjects_VIPERformat/pancancer)

```
@article{garcia2018benchmark,
  doi = {10.1101/337915},
  url = {https://www.biorxiv.org/content/early/2018/06/03/337915},
  year  = {2018},
  month = {jun},
  publisher = {},
  volume = {},
  number = {},
  pages = {},
  title={Benchmark and integration of resources for the estimation of human transcription factor activities},
  author={Garcia-Alonso, Luz and Ibrahim, MM and Turei, D and Saez-Rodriguez, J}
  journal={bioRxiv}
```
## Outlook
Currently we are trying to infer mouse regulons from the human regulons. [Drop us a line](mailto:cholland2408@gmail.com) if you are interested in the progress. More information coming soon...
