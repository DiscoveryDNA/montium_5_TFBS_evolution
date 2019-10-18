## README.md

**Purpose**: To explore and analyze Transcription Factor Binding Sites (TFBS) data from the genomies from 24 species of Drosophila in the Montium Clade. 

We are starting with just mapping [Bicoid (bcd)](https://en.wikipedia.org/wiki/Bicoid_(gene)) TFBS.

## The Data Origin

Main Data Repo: [https://drive.google.com/drive/folders/1kAh9NPg0gin4KIYvdz2Czi1LCQ2Js06X](https://drive.google.com/drive/folders/1kAh9NPg0gin4KIYvdz2Czi1LCQ2Js06X)

The motif data used in this analysis was created from alignments of non-coding regions from the genomes from 24 species . 

1. Using Kvon et al., data as a reference. 3500 orthologous non-coding regions were extracted from the 24 species. 
2. This data was further preprocessed: [https://github.com/DiscoveryDNA/QC_kvon](https://github.com/DiscoveryDNA/QC_kvon). Creating alignments of all regions.
3. Raw sequences were scanned for TFBS and mapped to the lignments using [https://github.com/DiscoveryDNA/map_motif2](https://github.com/DiscoveryDNA/QC_kvon).
4. The mapped TFBS regions were then used to extract the "orthologous TFBS region" and the nucleotides

## The Data

This is the data after all the preprocessing 'all_data_bcd_2019_10_01.csv'.

## Analysis 

Part 1: Stats and Quality control of the intial dataset.


The motif data used in this analysis was created from alignments of non-coding regions from the genomes from 24 species . https://github.com/DiscoveryDNA/map_motif2

## Overall Questions

At this point there will be species that have this motif and those that do not. For those species that do, you can ask: How is this sequence different between them? Are these clade specific changes?  For those species that do not have the sequence, is this an instance of TFBS sequence decay?  How did this sequence decay?  It would be good to be able to identify, using the tree, what TFBS arose and which TFBS decayed. Still have to work out exactly how, but overall, we could use ancestral state reconstruction. 