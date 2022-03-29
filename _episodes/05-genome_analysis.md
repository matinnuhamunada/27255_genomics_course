---
title: "Tools for analysing genomes"
teaching: 15
exercises: 45
questions:
- "How do I analyse my genome?"
objectives:
- "Assigning gene calls to sequence and annotate them with the known databases"
keypoints:
- "Genome annotation starts by identifying genes and other functional elements (rRNA, tRNA, etc.) within the nucleotides. This is followed by comparison with databases of interest to predict the functions encoded in the genes."
---
The next steps are then to actually analyse the assembled genome. Dependent on your research questions and what you want to investigate, is a range of different tools that can help with the analysis. Here is a list of suggestions that might be of interest to you. You don’t have to do them all, choose the ones you find suitable to answer your research questions. 

## antiSMASH: 
AnitSMASH stands for Antibiotics and Secondary Metabolites Analysis Shell and is used for the detection of secondary metabolites. To use AntiSMASH you first have to download your polished genome assembly from galaxy and then upload it to the AntiSMASH website. (https://antismash.secondarymetabolites.org/#!/start). After the it has finished the analysis job you will first be presented with a list of all detected secondary metabolite gene clusters, denoted as Region 1, Region 2 etc (labelled as number 5 in image). It will also tell you for each gene cluster the most similar known cluster detected in the MiBiG database, and the Similarity to that cluster. The Similarity is the percentage of genes within most similar known compound that have a significant BLAST hit to genes within the current region. So, the Similarity is NOT the same as the percentage identity that is an output of a Blast search. 
For more information on each Region, click on the number in the top (labeled as 2 in image). 
If you have experimental data on for example the bioactivity of your strain, try to match that to the potential compounds detected by AntiSMASH. 
For more information: 
- https://docs.antismash.secondarymetabolites.org/understanding_output
- https://docs.antismash.secondarymetabolites.org/
- https://academic.oup.com/nar/article/39/suppl_2/W339/2507123
- https://academic.oup.com/nar/article/47/W1/W81/5481154

> ## Discussion 01 - AntiSMASH
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

> ## Discussion 02 - Abricate
> 
>
> > ## Solution
> >
> > TBD
> {: .solution}
>
{: .challenge}

## Blast
Lastly, you can also simply blast genes of interest against your assembled genome. For that you will first have to download the nucleotide or amino acid sequence of your gene of interest from NCBI (https://www.ncbi.nlm.nih.gov/). Then you can use nucleotide Blast or tblastn (dependent if you have the nt or aa of your gene of interest). Use the option align two or more sequences. Below an example for finding a gene of interest in your assembled genome. 

{% include links.md %}