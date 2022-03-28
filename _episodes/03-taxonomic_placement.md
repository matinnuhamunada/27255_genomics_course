---
title: "Taxonomic Placement"
teaching: 10
exercises: 10
questions:
- "What is the taxonomic classification of my genome?"
objectives:
- "Assigning taxonomic classiffication to a newly assembled genomes using available tools."
keypoints:
- "Taxonomic placement of a newly assembled genome can be achieved by calculating nearest reference organism and placing the query genome into existing tree in the database. Such example of tools are autoMLST and GTDB."
---
## Downloading the assembled sequence
We now have an assembled genome that we can analyze. Before moving forward, we would like to determine the lineage or taxonomic classification of this newly assembled genome. For that, we will need to first download the genome from galaxy.

1. Find the `medaka consensus pipeline` - `Consensus` result and click the `Download` icon (first from left) to save it to your computer. **Hint:** The file should be in `.fasta` format.

## Taxonomic Placement with autoMLST
We will use [autoMLST](https://automlst.ziemertlab.com/analyze) to get an overview which gives us the most similar organisms. Unfortunately, it is not available in the Galaxy server, so we must do the analysis in the autoMLST webserver. 

1. Go to the [autoMLST webserver](https://automlst.ziemertlab.com/analyze)
2. Choose the `Placement (Fast) mode`
3. Upload your genome sequence
4. Enter your email to get your result back
5. Click `Submit job`

## Other tools to consider
### RefSeq_Masher
> Find what NCBI RefSeq genomes match or are contained within your sequence data using Mash MinHash with a Mash sketch database of 54,925 NCBI RefSeq Genomes.

### GTDB-tk
> a toolkit for assigning objective taxonomic classifications to bacterial and archaeal genomes.

> ## Discussion 01
> 
>
> > ## Solution
> >
> > TBD
> {: .solution}
>
{: .challenge}

{% include links.md %}

