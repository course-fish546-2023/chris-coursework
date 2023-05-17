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



d)  **Describe one subcommand of the BEDtools suite as well as a practical use case.**
