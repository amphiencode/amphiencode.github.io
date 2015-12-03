---
layout: page
title: Data
---

<div class="message">
  <b><u>Disclaimer:</u> This data is made available to the members of the european amphioxus genome consortium as collaborative material. These datasets are not to be used for whole genome analyses unless otherwise agreed for, and not to be redistributed to anybody outside the consortium without prior arrangements.</b></div>

## Datasets

The genome of the european amphioxus *Branchiostoma lancealatum* was generated from 150x Illumina coverage sequenced by [Génoscope](http://www.genoscope.cns.fr). In the Bl71nemr assembly, haplotypes were reconcilied using haplomerger. 

This assembly spans 495.3Mb (N50: 1.29Mb) split in 10,247 scaffolds with 4% of residual gaps. Masked regions are represented with lowercase characters (soft-masking); gaps in the assembly are represented with Ns.

The genome was annotated using both EVM/PASA pipeline and cufflinks/transdecoder. Both these annotation have their strength. Cufflinks provides a better representation of transcript diversity, limits and TSSs positions. Conversely, EVM generates more robust predicted proteins, especially in regard to frameshifts, etc... A final annotation with unified IDs (BL00000) was subsequently built by merging the two annotations with a suffix indicative of their origin (BL00000_evm0 or BL00000_cuff0). All three annotations are available as GTFs. 

|File   |Dataset   | Format |
|---|---|---|
| **[Bl71nemr.fa](https://www.dropbox.com/s/hoor1hcv90c2la7/Bl71nemr.fa.gz?dl=1)**  | Genome assembly  | fasta |
| **[Bla_annot-final_v4.gtf](https://www.dropbox.com/s/a9605ohtf8ydxy8/Bla_annot-final_v4.gtf.gz?dl=1)** | Final merged annotation (EVM/PASA+cufflinks)  | GTF | 
| **[Bla_annot_evm.gtf](https://www.dropbox.com/s/sc4r43dy5gl38g2/Bla_annot_evm.gtf.gz?dl=1)**| EVM/PASA annotation | GTF |
| **[Bla_annot_cuff_v4.gtf](https://www.dropbox.com/s/mwxqtyxso9ds0oy/Bla_annot_cuff_v4.gtf.gz?dl=1)** | Cufflinks annotation | GTF |
| **[Bla_annot-final_v4_refTr.fa](https://www.dropbox.com/s/p5mnsdru1bxkq4s/Bla_annot-final_v4_refTr.fa.gz?dl=1)**| Reference transcripts* | fasta |
| **[Bla_annot-final_v4_refAa.fa](https://www.dropbox.com/s/rx29l9swyruj5kk/Bla_annot-final_v4_refAa.fa.gz?dl=1)**| Reference proteins** | fasta |

*(\*) most expressed transcript for each locus; (\*\*) longest protein for each locus*

## Blast server

A **[blast server](http://zoo-animalia.zoo.ox.ac.uk/blastseq04)** makes it possible to search the assembly, the reference transcripts and proteins. 

## Genome browser

The european amphioxus genome assembly and annotation are available as a [UCSC track hub](https://genome.ucsc.edu/goldenPath/help/hgTrackHubHelp.html). The RNA-seq, ATAC-seq and Chip-seq available in the browser is not part of the bulk of genome data provided to the consortium and is a courtesy of JL Skarmeta's lab. To enable access, you can either: 

- Use the [following UCSC session](http://genome-euro.ucsc.edu/cgi-bin/hgTracks?hgS_doOtherUser=submit&hgS_otherUserName=fmarletaz&hgS_otherUserSessionName=basic_braLan1) which includes gene models, RNAseq signal and methylation data. 

- set up the hub by adding the hub address `http://zoo-animalia.zoo.ox.ac.uk/braLan/hub.txt` to `My Data > Track Hubs > My hubs` in UCSC menu. 





