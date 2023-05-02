---
title: "Week 06 Questions"

format:
  html:
    code-fold: false
    code-tools: true
    code-copy: true
    highlight-style: github
    code-overflow: wrap
---

a)  **What are SAM/BAM files? What is the difference between to the two?**  
SAM files (sequence alignment/ map) and BAM files (binary alignment/ map) are the standard data alignment formats used to store sequencing reads mapped to a reference. SAM files are readable and contain the metadata associated with the file, whereas BAM files are the samller, 'unreadable', and compressed binary version of SAM files.  

b)  **`samtools`is a popular program for working with alignment data. What are three common tasks that this software is used for?**  
samtools is used for viewing, manipulating, and summarizing your BAM files for analysis.  

c)  **Why might you want to visualize alignment data and what are two program that can be used for this?**  
Visualizing data gives us a first look (literally) at where our data aligns on chromosomes, where it doesn't , etc. You can visualize small portions of your sequence data in samtools, but IGV is the preferred visualization platform.

d)  **Describe what VCF file is?**  
A VCF file is a 3-part tab-delineated file that includes metadata, headers with sequence sample ID, and sequence data for each varient at a particular position. This file is created by 'calling' for varints in samtools and saving them.
