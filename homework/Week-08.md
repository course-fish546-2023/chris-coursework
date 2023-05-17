---
title: "Week 08 Questions"

format:
  html:
    code-fold: false
    code-tools: true
    code-copy: true
    highlight-style: github
    code-overflow: wrap
---

a)  **What is a genomic range and what 3 types of information do you need for a range?**  
Genomic ranges are a way to represent the features of a genome in a specific region and require the user to identify the chromosome of interest, and the start and stop positions of the feature of interest within that chromosome.

b)  **What does 0-based and 1-based refer to? What are the advantages and disadvantages of each?**  
Both the 0-based and 1-based reference are to a coordinate system that denotes if the sequence starts at one or zero. The most common use in biological science is the 1-based system whereas the most common in computer sciences is the 0-based system. I've gotta say the number one disadvantage to them both is the ease in which a mistake can be made via wrong annnotation - a bracket versus a parenthesis can be the basis for an 'one-off' error all the way down the line. The advantage to using the 0-based system is that packages and programming languages are built with it, so data manipulation and interpretation are 'intuitive' to the machine, whereas the 1-based system could result in error is data isn't properly prepated to work within the system. 

c)  **What is the value of BEDtools over the bioconductor package GenomicRange?**  
It seems that BEDtools may be more efficient and slightly easier to use its base functions than GenomicRange. BEDtools is used in command line versus GenomicRange which is used in R, but that is a moot point since Markdown is a thing *except* that it could be indicative of the power of the tool. R is a great tool, but command line interface lets me guess that the power of BEDtools is greater than GenomicRange. In practical use, there are no package issues or program issues in BEDtools that we may expect to see in GenomicRange.

d)  **Describe one subcommand of the BEDtools suite as well as a practical use case.**  
Merge seems like a really interesting way to view and interpret your data; it is the BEDtools function that allows the user to combine overlapping intervals . Merging overlapping or adjacent intervals can provide a clearer and more interpretable representation of genomic features. Instead of dealing with a large number of individual intervals, merging helps identify and highlight larger genomic regions with shared characteristics or functional significance. For mt project, I could anticipate using Merge to clarify which genomic ranges are most impacted across all contaminants, or I could use it to help boost my statistical power with fewer sequences since I am relying on existing data.
