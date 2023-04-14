#### Week 03 Questions

a)  **An R Markdown file is plain text file that contains what 3 important types of content?**\
    The file contains the (1) YAML header that sets the the format options of the document, (2) the code chunks that allow you to do work utilizing most coding languages and a simple document-specific style of syntax, and (3) the ability to manipulate the output format via 'knitting' without forcing you to adjust every other aspect of the document.

b)  **What is a chunk and how do you add them? of the many chunk options which one do you think you will use the most and why? How is inline code different than code chunks?**\
    A code chunk is where you place the code in your Markdown document. It is the place where the work of your project is created to render your analyses or visualization in the document. Pulling from the [reading](https://r4ds.had.co.nz/r-markdown.html), you can add a code chunk via the following methods:

    -   Typing "Cmd/Ctrl + Alt + I"
    -   'Inserting' from the icons on the toolbar
    -   Typing the chunk indicators of the three hashes to start your code block {your code language goes here} your ending three hashes.

c)  **What's gone wrong with this code? Why are the points not blue?**

    Utilizing 'ChatGPT in Source' Addin, I was able to find the answer

```         
ggplot(data = mpg) + 
  geom_point(mapping = aes(x = displ, y = hwy, color = "blue"))
```

The points are not blue because the color "blue" is being passed as a string instead of as a color code. To specify the color blue, you just need to remove the quotes around "blue".

The corrected code below shows the separation of the color parameter from the actual mapping of the points.

```         
ggplot(data = mpg) + 
  geom_point(mapping = aes(x = displ, y = hwy), color = "blue")
```

![plot](https://d33wubrfki0l68.cloudfront.net/fda836ccf904bda73f021f4802803bc134145ffa/0c9a7/visualize_files/figure-html/unnamed-chunk-11-1.png)

d)  **Of the many things we have done in class the past two weeks, what is one aspect you would like to revisit and spend more time on?**

    I am going to spend more time on pulling in and manipulating large data so that I can use it. I continue to stumble in code as well as in understanding of how the reference databases are being compared to the data in questions when I'm still unclear on what the code chunks are doing.
