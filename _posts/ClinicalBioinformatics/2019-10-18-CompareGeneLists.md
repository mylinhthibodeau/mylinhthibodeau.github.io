---
layout: post
title: Compare lists of genes
excerpt:
categories: ClinicalBioinformatics
tags: ["Clinical Bioinformatics", "SaveTime", "Automation"]
published: true
comments: true
share: true
---

### How to rapidly compare lists of genes?

#### Use online resources

There are multiple websites to compare lists of genes.

I personally like the [MolBioTools](http://www.molbiotools.com/listcompare.html) multiple list comparator and therefore, I will give you an example of how to use this tool to save time.

#### Arthrogryposis Panels

We will compare two company gene panels with a list of genes that we want to include: we will compare 3 lists together.

**Step 1.** Google "arthrogyposis panel" (today being 19-10-2019), there a numerous gene panels coming up. I selected 2 companies with large panels:

* Blueprint Genetics - Arthrogryposes [Panel]((https://blueprintgenetics.com/tests/panels/malformations/arthrogryposes-panel/) (78 genes)
* GeneDx - Arthrogryposis Multiple [Panel](https://www.genedx.com/test-catalog/disorders/arthrogryposis-multiplex-congenita/) (90 genes)

**Step 2.** Establish your expert-reviewed list of genes

Say I have my personal list of genes to include from the literature as follow: CATSAL, CATSHL, CHRNG, CHRND, CHRNA1,  DOK7, ECEL1, FBN2, GLE1, ERBB3, IRF6, LCCS3, MAGEL2, MYBPC1, MYH3, MYH8, PAFAHIBI, PIEZ02, PIP5KIC, RELN, RIPK4, RASPSN,  TARP, TNN12, TNNT3, TPM2, UBA1

**Step 2.** Go to comparator website

Click [here](http://www.molbiotools.com/listcompare.html) and you will see:

![molbiocomparator_raw](https://raw.githubusercontent.com/mylinhthibodeau/mylinhthibodeau.github.io/master/images/molbiocomparator_raw.png)

**Step 3.** Get the 3 lists of genes

For **Blueprint Genetics**, you need an extra step to isolated the list of genes from their website.

* Select the list of genes and copy-paste the list into an excel table as follow:

![BlueprintArthrogryposis_CopyList](https://raw.githubusercontent.com/mylinhthibodeau/mylinhthibodeau.github.io/master/images/BlueprintArthrogryposis_CopyList.png).

* In your excel sheet, select the first column (genes), copy and paste the list of genes in the first box of the comparator website.

For **GeneDx**, it's much simpler. Click on the Arthrogryposes Panel [Info Sheet](https://www.genedx.com/wp-content/uploads/2019/09/Comprehensive-Arthrogryposis-Info-Sheet.pdf) and simply select, copy and paste the list of genes in the second box of the comparator website.

For your **personal list of genes**, you can simply select, copy and paste in the third box.

It should look like:

![Arthrogryposis_CompareLists](https://raw.githubusercontent.com/mylinhthibodeau/mylinhthibodeau.github.io/master/images/ArthrogryposisCompare_3lists.png).

**Step 4.** Click compare *et voilà!!*

Now, you can simply look and click on the Venn Diagram to explore the overlaps.

![Arthrogryposis_ResultComparator_Lists](https://raw.githubusercontent.com/mylinhthibodeau/mylinhthibodeau.github.io/master/images/Arthrogryposis_ResultComparator_Lists.png).

At the quick glance, I see that compare to my personal list of genes to include:

* 14 genes are in both panels
* 1 gene is only in the Blueprint panel
* 12 genes are missing from either panels

> This is especially useful when customizing panels and identifying which genes are missing. For doing so, you just need to compare your personal list of genes with the company list of genes.

I hope this will help you save time :)

My Linh Thibodeau
