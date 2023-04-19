---
title: "Extra"
teaching: 15
exercises: 0
questions:
- "Using Command Line Tools for Bioinformatic Analysis"
objectives:
- "Getting a gist command line tools for a more flexibility in bioinformatic analysis"
keypoints:
- "Galaxy might not have all the tools and version required to run your analysis. Having a skill to work with command line tools and other programming language give you flexibility in your research."
---

## Where to start
A full genome assembly requires many curation steps, which is nicely summarized in the [Genome Assembly Guide](https://github.com/rrwick/Trycycler/wiki/Guide-to-bacterial-genome-assembly). When you have a nanopore only dataset, you can use trycycler to have a decent quality genomes through consensus approach. Nevertheless, the steps and tools can be complicated. Here, we wrap and simplifies the Trycycler into three steps using Snakemake.

## Example: Semi-automated Trycycler Assembly via Snakemake
For Nanopore only assembly, Trycycler offer a better accuracy to generate consensus assembly (combining multiple assemblies of the same isolate). Rather than only using one assembler like we do (Flye), Trycycler can subsample our reads and build multiple assemblies using different algorithms, then make a consensus out of it. You can also find Trycycler in galaxy.eu toolbox, but as it is quite intensive, I prefer to run it on a local machine / server.

Installing and running a command line tools for a newcomer might seems daunting. Nevertheless, there are two popular workflow manager: Snakemake and Nextflow, which makes running various pipelines and installing dependencies easier. We have tried to make a prototype to semi-automate run Trycycler via Snakemake here: [https://github.com/matinnuhamunada/trycycler_snakemake_wrapper](https://github.com/matinnuhamunada/trycycler_snakemake_wrapper). 

The TAs will run it for you, but it is also quite easy to run it on your own when you have the time (and resources).

{% include links.md %}