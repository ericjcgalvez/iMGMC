# iMGMC - integrated Mouse Gut Metagenomic Catalog

![logo](/images/logo.png)

## Description

*Creation of an new mouse gut gene catalog with special features:*
  - more diverse samples from different studies (12 Vendors incl. wild mice and various gut locations)
  - clustering-free approach: all-in-one assembly, keeping track of each ORF to contigs to bins
  - higher taxonomic resolution and more accuracy by using contigs for annotation
  - 16S rRNA gene integration via linkage to bins
  - expansion by 20,927 MAGs from sample-wise assembly of 871 mouse gut metagenomic samples, representing 1,296 species

See our paper for details:

**An integrated metagenome catalog enables novel insights into the murine gut microbiome**  
Till R. Lesker, Abilash C. Durairaj, Eric. J.C. Gálvez, Ilias Lagkouvardos, John F. Baines, Thomas Clavel, Alexander Sczyrba, Alice C. McHardy, Till Strowig http://biorxiv.org/cgi/content/short/528737v1

### External studies providing data:
Xiao, Liang, et al. "A catalog of the mouse gut metagenome." Nature biotechnology 33.10 (2015): 1103-1108. http://doi.org/10.1038/nbt.3353

Wang, Jun, et al. "Dietary history contributes to enterotype-like clustering and functional metagenomic content in the intestinal microbiome of wild mice." Proceedings of the National Academy of Sciences 111.26 (2014): E2703-E2710. http://doi.org/10.1073/pnas.1402342111

Lagkouvardos, Ilias, et al. "The Mouse Intestinal Bacterial Collection (miBC) provides host-specific insight into cultured diversity and functional potential of the gut microbiota." Nature microbiology 1 (2016): 16131. http://doi.org/10.1038/nmicrobiol.2016.131


## Data:

| Description | Size | Link |
|--|--|--|
| Catalog ORF sequences | 1 GB | [iMGMC-GeneID.fasta.gz](https://onedrive.live.com/download?cid=36ADEB4B3D109F6F&resid=36ADEB4B3D109F6F%2133644&authkey=AD4pwU2r1mk4FHU) |
| Full assembly contigs | 1.3 GB | [iMGMC-ConitgID.fasta.gz](https://onedrive.live.com/download?cid=36ADEB4B3D109F6F&resid=36ADEB4B3D109F6F%2133647&authkey=AIM3mw3FbPE6b_M) |
| Mapping File (GeneID->ContigID->BinID) | 30 MB | [iMGMC-map-Gene-Contig-Bin.tab.gz](https://onedrive.live.com/download?cid=36ADEB4B3D109F6F&resid=36ADEB4B3D109F6F%2133646&authkey=AJM_z8-oLOlOO58) |
| Taxonomic annotations | 40 MB | [iMGMC_map_taxonomy.tar.gz](https://onedrive.live.com/download?cid=36ADEB4B3D109F6F&resid=36ADEB4B3D109F6F%2133736&authkey=AOjPxI-kDPJEpc8) |
| Functional annotations | 36 MB | [iMGMC_map_functionality.tar.gz](https://onedrive.live.com/download?cid=36ADEB4B3D109F6F&resid=36ADEB4B3D109F6F%2133738&authkey=APk09LufvLmUJN8) |
| 16S rRNA sequences | 2 MB | [iMGMC-16SrRNAgenes.fasta](https://onedrive.live.com/download?cid=36ADEB4B3D109F6F&resid=36ADEB4B3D109F6F%2133739&authkey=AAsGBvRCokrqALg) |
| integrated MAGs | 0.5 GB | [iMGMC_MAGs.tar.gz](https://onedrive.live.com/download?cid=36ADEB4B3D109F6F&resid=36ADEB4B3D109F6F%2134225&authkey=ABA7bpleGh606kI) |
| representave mMAGs (n=1296) | 1 GB | [iMGMC-mMAGs-dereplicated_genomes.tar.gz](https://onedrive.live.com/download?cid=36ADEB4B3D109F6F&resid=36ADEB4B3D109F6F%2137126&authkey=ADFYgL1YRjtb-Vo) | 
| representave hqMAGs (n=830) | 0.7 GB | [iMGMC-hqMAGs-dereplicated_genomes.tar.gz](https://onedrive.live.com/download?cid=36ADEB4B3D109F6F&resid=36ADEB4B3D109F6F%2137129&authkey=AFbfuXtd4Cm9kHQ) | 
| all mMAGs (n=20,927) | 15 GB | [iMGMC-mMAGs.tar.gz](https://onedrive.live.com/download?cid=36ADEB4B3D109F6F&resid=36ADEB4B3D109F6F%2137128&authkey=AFxAhkbg1uYWzhY) | 


Accession codes of the used gut metagenome sequences:
European Nucleotide Archive: [ERP008710](https://www.ebi.ac.uk/ena/data/view/ERP008710), [ERA473426](https://www.ebi.ac.uk/ena/data/view/ERA473426), [PRJEB32890](https://www.ebi.ac.uk/ena/data/view/PRJEB32890) and to the Metagenomics Rapid Genomes/Metagenomes (MG-RAST) with ID 4661127.3/ [mgp5130](https://www.mg-rast.org/linkin.cgi?project=mgp5130)



## Pipelines:

![pipeline](/images/pipeline.png)

We recommend the use of [Bioconda](http://bioconda.github.io/)

### Use of the gene catalog (mapping pipeline)

[Instruction to process your own WGS samples with iMGMC](/genecatalog-pipeline.md)

### PICRUSt (mouse gut specific)

[Instruction to process your own samples 16S rRNA amplicon samples with PICRUSt and iMGMC](/PICRUSt/README.md)

### IMNGS (resource of processed 16S rRNA microbial profiles)

[Instruction to work with iMGMC-IMNGS data](/IMNGS.md)

### Workflows to create the iMGMC Catalog

[Code for assembly, binning and 16S rRNA gene reconstruction](/creation-cataloge-pipeline.md)

[Code for linking 16S rRNA genes to bins](/linking/README.md)

### Workflows to create by sample MAGs (single wise)

[Code for the generation and clustering of single-wise assembly MAGs](/sMAG-pipeline.md)

[Code for the evaluation of single-wise assembly MAGs versus all-in-one assembly MAGs](/evaluation/README.md)

