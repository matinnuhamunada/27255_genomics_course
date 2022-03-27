---
title: "Introduction"
teaching: 15
exercises: 15
questions:
- "How do I start working with my sequence data?"
objectives:
- "Understand the data format and make a decision on how to process MinION data"
keypoints:
- "First key point. Brief Answer to questions. (FIXME)"
---
## Introduction
For the bioinformatics analysis of your genomes, we will be working in Galaxy. 

There are two main online galaxy platforms; the global server: [https://usegalaxy.org/](https://usegalaxy.org/){:target="_blank"} and the European server: [https://usegalaxy.eu/](https://usegalaxy.eu/){:target="_blank"}. The global version has a slightly larger set of programs than the European version. However, the European version runs in general slightly faster, and therefore you are recommended using the European version. 

## Overview of Genome Assembly Processes

<div style="width: 640px; height: 120px; margin: 10px; position: relative;"><iframe allowfullscreen frameborder="0" style="width:640px; height:120px" src="https://lucid.app/documents/embeddedchart/2d2d642d-65ea-4f1b-a1e0-329c5ee118e9" id="J954-Kp1sEdf"></iframe></div>

## Importing Data into Galaxy
There are several ways we can input our data into Galaxy. **We will inform you how to fetch your raw sequencing data when it is ready**. In the meantime, we can exercise our analysis using the data from **last year**.

The data from previous year is available in Aileen's (previous TA) history. Let's login to Galaxy and import this data into our history:
1. Go to [https://usegalaxy.eu/](https://usegalaxy.eu/){:target="_blank"}
2. Click `Login or Register`. Create an account and activate (if you hadn’t so)
3. Go to Aileen's history at: [https://usegalaxy.eu/u/aileen/h/nanoporesequencesmastercourse](https://usegalaxy.eu/u/aileen/h/nanoporesequencesmastercourse){:target="_blank"}
4. Import the data by pressing the `+` button on the upper right corner and click `import`. _Note that this only works if you are on the same server._
5. Rename the history to "27255_raw_2021"

> ## Discussion
> Each item in the history are the samples raw reads that has been demultiplexed. 
> - How many gigabytes of data are there?
> - How much data was generated for an average sample?
> - Why do we have uneven distribution of data yield? Is that normal?
{: .challenge}

## Importing and editing a published workflow
We have prepared a template workflow that you can edit and use in your genome assembly and annotation. The workflow will be split into different steps with several measures to check quality in between. 

Follow this step to import and run initial QC workflow in your history:
1. In a new tab, open this link: [https://usegalaxy.eu/u/matinnu/w/01rawqc](https://usegalaxy.eu/u/matinnu/w/01rawqc){:target="_blank"}
2. On the top-right corner, click the `+` button (import workflow) 
3. Click `start` using this workflow
4. Click on the name of the newly imported workflow (`imported: 01_Raw_QC`) and click `Edit`
5. Explore the workflow and make changes if necessary
> ## Discussion
> - What are the purpose of the two main tools in the workflow?
> - Do you think [Kraken2](https://ccb.jhu.edu/software/kraken2/) is suited for long-read sequences?
{: .challenge}

When you are contempt with the workflow, click save. Next, we will run `barcode02.fastq` (the smallest dataset) with the workflow.
1. Click the "play" button on the top-right corner (`Run Workflow`)
2. If the workflow does not show in detailed view, click `Expand to full workflow form`
3. Set `Send results to a new history` to `yes`. 
4. Change to the history name to "01_Raw_QC_sample02_2021".
5. On the `1: input dataset`, select `2: barcode02.fastq` as the input.
6. Click `Run Workflow` on the top panel.

<iframe src="https://drive.google.com/file/d/11oVVgxtFSqbGPfaS0JNYckiyXYZmV_-Y/preview" width="640" height="480" allow="autoplay"></iframe>

## Adding more analysis in your workflow
As you can see, the workflow only has three parts:
- QC & Filtering
- Assembly
- Polishing

Next, we would like to add more analysis in the workflow:
- Gene Calling & Annotation

{% include links.md %}

