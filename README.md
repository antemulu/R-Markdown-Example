# R-Markdown-Example
title: "R Markdown Example"
author: "AM"
date: "4/11/2022"
output: html_document
---


#Introduction
#Create your own Markdown file and post the code on GitHub and your reflection on the process of Markdown in your blog.
Importing the inbuilt dataset "mtcars" 

```{r}

data(mtcars)

head(mtcars)

```

#mean of the variable 'mpg' in the 'mtcars' dataset


```{r}
mean(mtcars$mpg)
```

#median of the variable 'qsec' in 'mtcars' dataset

```{r}
median(mtcars$qsec)
```

#Descriptive statistics for 'disp' variable

```{r}
summary(mtcars$disp)
```

#Scatter plot between 'disp' and 'wt'


```{r}
scatter.smooth(x=mtcars$disp, y=mtcars$wt, main="disp ~ wt")
```
I created documents with R Markdown which starts with an .Rmd file that contains a combination of markdown (content with simple text formatting) and R code chunks. The .Rmd file is fed to knitr, which executes all the R code chunks and creates a new markdown (.md) document which includes the R code and its output. 
R Markdown presents your code alongside its output (graphs, tables, etc.) with conventional text to explain it, a bit like a notebook. 
I converted my R Markdown document to .html file type to display the headers, images etc.   
At the top of any RMarkdown script is a YAML header section enclosed by ---. By default, this includes a title, author, date and the file type you want to output to. 
I used regular markdown rules in my R Markdown document. Once I knitted my document, to be used by another person the output displayed text formatted HTML. 
Code Chunks: YAML header is the space where you will write your code, accompanying explanation and any outputs.  


