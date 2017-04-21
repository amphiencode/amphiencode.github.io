---
layout: page
title: Data
---

<div class="message">
  <b><u>Disclaimer:</u> This dataset is made available to the members of the European amphioxus genome consortium as collaborative material. These datasets are not to be used for whole genome analyses unless otherwise agreed for, and not to be redistributed to anybody outside the consortium without prior arrangements. The functional genomics data (ATAC-seq, Chip-seq, Methylation, RNA-seq) included in the browser are provided as a courtesy by several participant labs and remain their property (see contacts).</b></div>

## Datasets

The genome of the European amphioxus *Branchiostoma lancealatum* was generated from 150x Illumina coverage sequenced by [Genoscope](http://www.genoscope.cns.fr). In the Bl71nemr assembly, haplotypes were reconcilied using haplomerger.

This assembly spans 495.3Mb (N50: 1.29Mb) split in 10,247 scaffolds with 4% of residual gaps. Masked regions are represented with lowercase characters (soft-masking); gaps in the assembly are represented with Ns.

The genome was annotated using both EVM/PASA pipeline and cufflinks/transdecoder. Both these annotation have their strength. Cufflinks provides a better representation of transcript diversity, limits and TSSs positions. Conversely, EVM generates more robust predicted proteins, especially in regard to frameshifts, etc... A final annotation with unified IDs (BL00000) was subsequently built by merging the two annotations with a suffix indicative of their origin (BL00000_evm0 or BL00000_cuff0). All three annotations are available as GTFs.

|File   |Dataset   | Format |
|---|---|---|
| **[Bl71nemr.fa](https://www.dropbox.com/s/r9s9wd3osyf6zud/Bl71nemr.fa.gz?dl=1)**  | Genome assembly  | fasta |
| **[Bla_annot_final.gtf](https://www.dropbox.com/s/d4fqnoa8gdix3pa/Bla_annot_final.gtf.gz?dl=1)** | Final merged annotation (EVM/PASA+cufflinks)  | GTF |
| **[Bla_annot_evm.gtf](https://www.dropbox.com/s/d4fqnoa8gdix3pa/Bla_annot_final.gtf.gz?dl=1)**| EVM/PASA annotation | GTF |
| **[Bla_annot_cuff.gtf](https://www.dropbox.com/s/ow1v90mfflk070b/Bla_annot_cuff.gtf.gz?dl=1)** | Cufflinks annotation | GTF |
| **[Bla_annot_final_v4.fa](https://www.dropbox.com/s/3an2j8vd7ljwm47/Bla_annot_final_v4.fa.gz?dl=1)** | All full transcripts (coding and non-coding) | fasta |
| **[Bla_annot_v4_best_Aac.fa](https://www.dropbox.com/s/8853oz3c977nxdn/Bla_annot_v4_best_Aac.fa.gz?dl=1)**| Reference protein*  | fasta |
| **[Bla_annot_v4_best_Cds.fa](https://www.dropbox.com/s/tkzkuo4gq25v11g/Bla_annot_v4_best_Cds.fa.gz?dl=1)**| Reference CDS*  | fasta |
| **[Bla_annot_v4_best_Tra.fa](https://www.dropbox.com/s/6by9yx915jyba7a/Bla_annot_v4_best_Tra.fa.gz?dl=1)**| Reference transcripts*  | fasta |

*(\*) most highly expressed transcript for each coding locus (35961)

## Blast server

A **[blast server](http://zoo-animalia.zoo.ox.ac.uk/blastseq04)** makes it possible to search the assembly, the reference transcripts and proteins.

## Genome browser

The European amphioxus genome assembly and annotation are available as a [UCSC track hub](https://genome.ucsc.edu/goldenPath/help/hgTrackHubHelp.html). The assembly should be searchable using BLAT. To enable access, you can either:

- Use the [following UCSC session](http://genome-euro.ucsc.edu/cgi-bin/hgTracks?hgS_doOtherUser=submit&hgS_otherUserName=fmarletaz&hgS_otherUserSessionName=basic_braLan1)
- set up the hub by adding the hub address `http://zoo-animalia.zoo.ox.ac.uk/BraLan/hub.txt` to `My Data > Track Hubs > My hubs` in UCSC menu.
