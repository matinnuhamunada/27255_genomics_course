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

> ## Discussion 01 - Prokka
> 
>
> > ## Solution
> >
> > TBD
> {: .solution}
>
{: .challenge}

## antiSMASH: 

> ## Discussion 02 - AntiSMASH
> 
>
> > ## Solution
> >
> > TBD
> {: .solution}
>
{: .challenge}

## Abricate 
ABRicate is a tool for the detection of antimicrobial and virulence genes. It is also available on Galaxy, so you don’t have to download your assembly for this. It uses different databases for example CARD to detect virulence genes in the genome. For more information: https://github.com/tseemann/abricate.  
See below an example of default parameters with CARD database selected, an explanation of the output table and an example output. 

> ## Discussion 02 - AntiSMASH
> 
>
> > ## Solution
> >
> > TBD
> {: .solution}
>
{: .challenge}

{% include links.md %}