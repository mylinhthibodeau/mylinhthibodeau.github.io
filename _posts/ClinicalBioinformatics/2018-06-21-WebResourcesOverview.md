---
layout: post
title: Web Resources Overview for Clinical Bioinformatics
excerpt:
categories: ClinicalBioinformatics
tags: ["Genomics", "Clinical Bioinformatics" , "Introduction", "Resources", "Web"]
published: true
comments: true
share: true
---

Essentials of web resources !

### Essentials - Websites

#### Phenotype

For a clinical data entry phenotypic tool, you can explore the [Phenotips](https://phenotips.org/) (Girdea et al, 2013)[1] as an option for your centre/department.

The [Monarch](https://monarchinitiative.org/phenotype) initiative can be useful for integrating both phenotypic and genomic data from diverse sources, such as OMIM and NCBI gene identifiers. It also contains pathogenic variants from the ClinVar databases. The web Analyze tool allows for determining "semantic similarities", which allows to obtain phenotypic similarities scores for associating genes and diseases. It also provides genotype-phenotype associations in diverse organisms, including Human and Mouse (frequent model organism for studying human diseases). You can also export the results of your search (e.g. ClinVar variants and Phenotypes results as tsv files)

There are many tools for phenotypic entries, and it is better to prioritize tools that have these features:

* Easy to use: Select web-application tools that are intuitive and fast to use. When you start using such tools, it might take you 10 minutes to figure out the way to perform a data query, but as you become more familiar, it shouldn't take more than 5 minutes to understand the basics of how to use a tool. If it takes more time, you might consider assessing other tools that are faster for you to get a handle on.
* Data export is available: You should prioritize web tools that allows you to export the results of your search as text files (tsv, txt or csv formats). This will allow you to store the information for later use, and also, will avoid the need for typing or writing down the results of your search. As complexity of genotype-phenotype searches is increasing, saving time at each step is important ! Moreover, downloading the file will allow you to keep track of the source of the data so that you can reference it later.
* Clinically used: Ideally, we would like to prioritize tools that have been clinically validated, but at this time, there is no information or review comparing these tools and how helpful they are for clinicians. Therefore, prioritize tools that have proven useful at in research and have been used successfully in the literature and until we gather more information on web-applications, we will need to make up our own mind about which tool is best suited for genetics practice.
* Uniformity if possible: If at all possible when working in a group, it would be ideal for the group to work with the same tools. Therefore, the search/query output will be reproducible and also, compatible for data aggregation. This may seem trivial, but building a department/local (and eventually perhaps ?national ?international) knowledge database can be very useful in accelerating diagnostic accuracy and making the group benefit from the experience of individual clinicians.

### American College of Medical Genetics - Variant Classification

I have mentioned some of the ACMG web-based tools in a [previous post](https://mylinhthibodeau.github.io//genomics101/WebResourcesOverview/), which include [InterVar](http://wintervar.wglab.org/), the [University of Maryland tool](http://www.medschool.umaryland.edu/Genetic_Variant_Interpretation_Tool1.html/), but if you are performing a lot of variant classification work, you might consider using a software package such as [ANNOVAR](http://annovar.openbioinformatics.org/en/latest/user-guide/download/), which performs variant annotation as well and can be integrated with an [python-based InterVar](https://github.com/WGLab/InterVar) script. You will need to register in order to use ANNOVAR, while the [InterVar](http://wintervar.wglab.org/) web-application can be used directly.

***

#### References

[1] Girdea, M., Dumitriu, S., Fiume, M., Bowdin, S., Boycott, K. M., Chénier, S., Chitayat, D., Faghfoury, H., Meyn, M. S., Ray, P. N., So, J., Stavropoulos, D. J. and Brudno, M. (2013), PhenoTips: Patient Phenotyping Software for Clinical and Research Use. Hum. Mutat., 34: 1057–1065. doi: 10.1002/humu.22347
