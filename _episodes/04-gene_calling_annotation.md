---
title: "Genome Annotation"
teaching: 10
exercises: 30
questions:
- "What genes are contained in my genome?"
objectives:
- "Assigning gene calls to sequence and annotate them with the known databases"
keypoints:
- "Genome annotation starts by identifying genes and other functional elements (rRNA, tRNA, etc.) within the nucleotides. This is followed by comparison with databases of interest to predict the functions encoded in the genes."
---
## Importing and editing Annotation workflow
Import genome annotation workflow:
1. In a new tab, open this link: [https://usegalaxy.eu/u/matinnu/w/03annotation](https://usegalaxy.eu/u/matinnu/w/03annotation){:target="_blank"}
2. On the top-right corner, click the `+` button (import workflow) 
3. Click `start` using this workflow
4. Click on the name of the newly imported workflow (`imported: 03_Annotation`) and click `Edit`
5. Explore the workflow and make changes if necessary

When you are contempt with the workflow, click save. Next, we will run the analysis on the newly assembled genome (sample_02)
1. Click the _"play"_ button on the top-right corner (`Run Workflow`)
2. If the workflow does not show in detailed view, click `Expand to full workflow form`
3. Set `Send results to a new history` to `yes`. 
4. Change the history name to _"03_Annotation_2021_sample02"_.
5. On the `1: input dataset`, select `medaka consensus` as the input.
6. Click `Run Workflow` on the top panel.

## Prokka: rapid prokaryotic genome annotation
Prokka is a software tool to annotate bacterial, archaeal and viral genomes quickly and produce standards-compliant output files.

> ## Discussion 01 - Prokka
> 1. What kind of output do you get from Prokka?
> 2. Which outputs can be used for subsequent analysis?
>
> > ## Solution
> >
> > TBD
> {: .solution}
>
{: .challenge}

## Busco: 
Busco is a functional quality control based on evolutionarily-informed expectations of gene content of near-universal single-copy orthologs
> ## Discussion 02 - Busco
> 1. What kind of output do you get from Busco?
> 2. How do you know if your genome is contaminated or incomplete?
> 3. What other tools can we use for quality checking our genome completeness and contamination?
>
> > ## Solution
> >
> > TBD
> {: .solution}
>
{: .challenge}

{% include links.md %}