---
layout: post
title: Compare lists of genes
excerpt:
categories: ClinicalBioinformatics
tags: ["Clinical Bioinformatics", "Introduction", "Resources"]
published: true
comments: true
share: true
---

### How to rapidly compare lists of genes?

#### Use online resources

There are multiple websites to compare lists of genes.

I personally like the [MolBioTools](http://www.molbiotools.com/listcompare.html) multiple list comparator and therefore, I will give you an example of how to use this tool to save time.

#### Arthrogryposis Panels

**Step 1.** Google "arthrogyposis panel" (today being 19-10-2019), there a numerous gene panels coming up. I selected 2 companies with large panels:

* Blueprint Genetics - Arthrogryposes [Panel]((https://blueprintgenetics.com/tests/panels/malformations/arthrogryposes-panel/)
* GeneDx - Arthrogryposis Multiple [Panel](https://www.genedx.com/test-catalog/disorders/arthrogryposis-multiplex-congenita/)

**Step 2.** Go to comparator website

Click [here](http://www.molbiotools.com/listcompare.html) and you will see:

![molbiocomparator_raw](https://raw.githubusercontent.com/mylinhthibodeau/mylinhthibodeau.github.io/master/images/molbiocomparator_raw.png)


#### What will this post cover?

This blog post is a work in progress. I will be providing an overview of some bioinformatics genomics skills and resources based on my personal training experience.

This post will also be followed by "workshop posts" containing some applied/hands-on simple exercises/examples, which will also be made available on [my personal github](https://github.com/mylinhthibodeau/Genomics101-Workshop).

### First of all, register your accounts

The very first step on your journey is to be able to retrieve genomic data from the Web. My personal advice would be to register accounts for these resources:

* [UCSC](https://genome.ucsc.edu/cgi-bin/hgSession?hgS_doMainPage=1)
* [Ensembl](http://uswest.ensembl.org/index.html)
* Genomic Oligoarray and SNP array evaluation tool v3.0 - [University of Miami CMA tool](http://firefly.ccs.miami.edu/cgi-bin/ROH/ROH_analysis_tool.cgi). This has been a popular tool in clinical practice, but there are other useful tools that perform similar tasks in my opinion (e.g. [NCBI Bulk Conversion](Databases and Web Tools for Cancer Genomics Study) or [Ensembl BioMart](ensembl.org/biomart/martview))
* [COSMIC](https://cancer.sanger.ac.uk/cosmic/register). If you are working with families with hereditary cancer, I suggest you also register a COSMIC account.

If you are planning to acquire intermediate-to-advanced coding skill, you can also register for this:

* OMIM API [access request](https://www.omim.org/api).

### Overview

#### 100% useful clinical bioinformatics skills

While coding is a powerful tool, it can also have a steep learning curve at the beginning. There are many tools you can use which require no coding at all. So rather than starting from scratch you can benefit from those that have come before and focus on the more pertinent part of that data analysis

If you are a clinical trainee with a limited amount of time available, the best avenue for you is likely to learn how to make the most out of GUI (Graphical User Interface) resources.

Don't be quick to dismiss GUI websites/resources as they are often underused resources and most clinicians (and even researchers) are not using them to their full potential. For example, although most people know how to punch genomic coordinates in the UCSC (University of California Santa Cruz) [Genome Browser](https://genome.ucsc.edu/) or [BLAT](https://genome.ucsc.edu/cgi-bin/hgBlat) a sequence (which is performing targeted alignment), most people do not know how to add custom tracks of genomic coordinates (e.g. BED file format) to visualize contigs (assembled *de novo* or with alignment from sequencing data) or splicing junctions (e.g. transcriptome data). I am providing you with some instructions on how to do this below.

Clinical genetics training should provide you with the opportunity to learn the basic uses for these resources (see below), but note that for most of these individual GUI resources, there are 1-4 days workshops available to learn the intricasies of their workings, so even though you might already know the basics, I believe taking it further could be useful for clinical and research applications.

#### Genome browsers

**UCSC [Genome Browser](https://genome.ucsc.edu/)**

As mentioned previously, the UCSC [Genome Browser](https://genome.ucsc.edu/) can be used for diverse tasks.

* Basic uses: Query genomic position and retrieve databases annotations.
* Additional uses: (see [Exercises](https://github.com/mylinhthibodeau/Genomics101-Workshop/tree/master/UCSC/UCSC_exercises.md))
  - Upload custom genomic coordinates text or BED file data to UCSC to visualize genomic contigs.
  - Visualize transcriptome splicing events


I have personally used UCSC to visualize and characterize somatic splicing abnormalities. If you are working with assembly data, this UCSC feature could be extremly useful for you. It would allow you to visualize genomic events at the same time than the genomic annotations (gene transcripts, databases entries like ClinVar, dbSNP, DECIPHER, etc.).  

**[Ensembl](https://uswest.ensembl.org/Homo_sapiens/Info/Index)**

* Basic use: search for gene/variant/transcript annotations  
* Additional uses: (see [Exercises](https://github.com/mylinhthibodeau/Genomics101-Workshop/tree/master/Ensembl/Ensembl_exercises.md))
  - Use [BioMart](http://grch37.ensembl.org/biomart/martview/903c1d51f3db4ab09ae86c4184ac84b6) for data query and extensive annotations
  - Convert genomic coordinates between assemblies

**[Remap](https://www.ncbi.nlm.nih.gov/genome/tools/remap)**

* Basic use: [Remap](https://www.ncbi.nlm.nih.gov/genome/tools/remap) converts genomic coordinates from one assembly to another (e.g. from GRCh37 to GRCh38). Note that this task can also be accomplished with the [Ensembl Assembly Converter](http://www.ensembl.org/Homo_sapiens/Tools/AssemblyConverter) or [UCSC LiftOver](https://genome.ucsc.edu/cgi-bin/hgLiftOver) tool.

See [exercise](https://github.com/mylinhthibodeau/Genomics101-Workshop/tree/master/Remap/Remap_exercises.md) for an example.

#### Population Databases

**ExAc and gnomAD**

See [example](http://exac.broadinstitute.org/variant/20-10620522-C-T) for IGV.js visualization. The sequencing reads for each individual can be visualized at the bottom as ExAc is using the visualization [IGV.js](https://github.com/igvteam/igv.js) tool.

**[dbSNP](https://www.ncbi.nlm.nih.gov/projects/SNP/)**

If you are searching more than 2-3 SNPs repetitively, it would be more time efficient to submit a batch query. Unfortunately, the [batch query tool](https://www.ncbi.nlm.nih.gov/projects/SNP/batchquery.html) is becoming deprecated, but I think it is a still useful exercise to try.

See [exercise](https://github.com/mylinhthibodeau/Genomics101-Workshop/tree/master/dbSNP/dbSNP_exercises.md) for an example.


#### Phenotypic resources

**[Phenomizer](http://compbio.charite.de/phenomizer/)**

This is a tool from the Human Phenotype Ontology (HPO).

#### Likely useful coding skills

In order to acquire coding skills, it takes approximately 4 months of full time dedicated and intensive work. Why 4 months? Oh well, because it is approximately the amount of time it took me. Although I was performing some research work at the same time, I also have completed one year of mechanical engineering before medical school and I had learned basic coding skills. Therefore, all things considered, I am pretty confident that 4 months would be the minimum amount of time required to learn sufficient coding skils in order to apply them to real clinical or research problems.

Unfortunately, there aren't any curriculum for clinical bioinformatics yet. Moreover, in order to reach a coding skill level that will allow you to use coding for clinical data, you will most likely need to learn some genomics research coding as a baseline, then you will be able to build on this skill set with more complex clinical questions.

**Learn coding skills mainly useful for research**

Introductory curriculum:

Individual Genomic Tools: Other workshops such as the ones provided at conferences can be a good introduction. I highly recommend to seek and attend such workshops when available, especially at clinical conferences since these sessions will provide a snapshot overview of a genomic tool. For example, the [American Society of Human Genetics](http://www.ashg.org/) [Annual Meeting 2017](http://www.ashg.org/meetings/index.shtml) had several interactive invited workshops, including "Accessing the Breadth of Data in Ensembl: A Worked Clinical Example" and "Overview and Interpretation of GTEx Resources: eQTLs and Gene Expression".

Basic coding/bioinformatics: The [Canadian Bioinformatics Workshops](https://bioinformatics.ca/workshops/) can provide a "crash course-like" curriculum. Although some of more advanced workshop require a letter of support from a person in the field of Bioinformatics (ideally from a known leader in the field), these workshops are meant to be introductory and might be suitable for a keen clinical trainee.

More comprehensive "coding oriented" curriculum:

- R coding: STAT545/STAT547
- Python: self-learning > CPSC 301 Computing for Life Sciences (UBC)
  - Other possibility: Workshops (UBC and SFU)
- Bash (Linux/Unix) terminal: No real "medical/biological" formal curriculum available on online platforms or at nearby teaching institutions (pending review).

**Learn clinically useful coding skills**

Here are some examples of useful skills to acquire and the language(s) that would allow to complete them.

* R coding or Python:
  - Comparing lists of genes
  - Using an API (Application Programming Interface). For example, the OMIM API, to retrieve genetic and phenotypic data.
* Bash:
  - Learn how to use the terminal to query txt files (.txt, .tsv, .csv) or a VCF file

***

### Perhaps less useful coding skills, except if you have a lot of time available and are an independent learner

This section is meant for the motivated individual who wants to acquire bioinformatics skills independently in a self-learning process.

#### Step 1. Download some datasets (intermediate-to-advanced)

This also only apply to you if are planning to acquire intermediate-to-advanced coding skill. If it is the case, I would advise is to download useful datasets to your computer:

* DECIPHER The Development Disorder Genotype - Phenotype Database ([DDG2P database](https://decipher.sanger.ac.uk/ddd#ddgenes)).
* Catalogue of Somatic Mutations in Cancer/[COSMIC gene census](https://cancer.sanger.ac.uk/census). You need to have registered an account to download the file to your computer (otherwise, you are stuck with browsing the data on the web). I find that the COSMIC cancer gene census encompass almost all hereditary cancer predisposition genes and therefore, can be useful as a reference list.
* [Orphadata](http://www.orphadata.org/cgi-bin/index.php/) from Orphanet. This resource could potentially be very useful to a clinician as it contains a lot of phenotypic data, but its use is limited by the difficulty to query the XML format data (e.g. [Phenotypes associated with rare disorders](http://www.orphadata.org/cgi-bin/inc/product4.inc.php)) and the inconsistencies of the tree structure. Using this resource will require a lot of patience, time and hard work, and will most likely require intermediate Python coding skills, so I would classify it as "Advanced".

#### Step 2. Learn the basics

Although less useful in the short run, starting with learning basic computer science skills would teach underlying workings and function of very simple algorithms using if/else/or statements.

* Basics of R (3-4 weeks): Online [Technical Foundations of Informatics](https://info201-s17.github.io/book/index.html). Specifically, Introduction to Git and Github, Introduction to R.
  - Pros: If a limited amount of time is available, learning how to employ "ready to use" functions in R is more appropriate. The time to reach usefullness is shorter. Applications to biological (and clinical) questions/problems is easier.
  - Cons: This coding language was not meant for building algorithms and instead, was meant as a statistical tool for research. Therefore, it is less flexible and it contains several incohenrences. Error messages are difficult to troubleshoort.  
* Basics in Python (3-4 weeks): Online [Code Academy Learn Python](https://www.codecademy.com/learn/learn-python). Python is a more coherent coding language.
* Basics of terminal/bash commands: Unfortunately, terminal use (bash Linus/Unix) is not as intuitive as R or Python languages, and therefore, I believe that "self-learning" might be a difficult approach. It is why I would recommend a more formal training avenue.
  - The University of British Columbia- West Grid/Compute Canada [Introduction to Genomic Analysis](https://arc.ubc.ca/introduction-genomic-analysis-workshop-series-june-5-9) is a [workshop series](https://phillip-a-richmond.github.io/Introduction-to-Genomic-Analysis/) initially meant for Canadian researchers using Compute Canada resources, but the curriculum seem to cover the most important basic terminal use/bash skills required for bioinformatics and therefore, appears to be a good option for genetics/genomics clinical trainees.
