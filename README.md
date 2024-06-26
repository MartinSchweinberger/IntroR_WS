# Introduction to R for Social Science

Martin Schweinberger (University of Eastern Finland, 11-12 May, 2024)

## General Information

### Abstract


This beginner-friendly workshop, *Introduction to R for Social Science*, is designed to equip participants with the foundational skills necessary to use R and RStudio effectively for text-based social science research. Through hands-on exercises and guided instruction, attendees will learn how to navigate the RStudio environment, load, manage, manipulate, and visualize data, and perform basic text analytics. Key topics covered include the use of regular expressions for pattern matching, concordancing for textual analysis, and essential techniques in network analysis, sentiment and keyword analysis, and topic modeling. By the end of this workshop, participants will have a solid understanding of how to use R for text-based social science research, opening up new possibilities for data-driven insights in their field. No prior experience with R or programming is required. 

### Timeline

Here is what we have planned to cover in this workshop (2 days, 10am to 4pm):

**Tuesday, 11 June** 

* 10:00 - 10:15 Introduction to the workshop

* 10:15 - 10:45 Preparation and getting started

* 10:45 - 11:30 R and RStudio basics 

* **11:30 - 12:30 Lunch break**

* 12:30 - 12:45 Exercise 1: Text Processing

* 12:45 - 13:15 Working with text

* 13:15 - 14:00 Basic string processing 1

* **14:00 - 14:30 Coffee break**

* 14:30 - 15:15 Basic string processing 2

* 15:15 - 16:00 Advanced string processing

**Wednesday, 12 June** 

* 10:00 - 10:10 Recap

* 10:10 - 10:45 Basics of data visualization

* 10:45 - 11:00  Introduction to Text Analytics

* 11:00 - 11:30 Exercise 2: Sentiment Analysis and Keyword Analysis

* **11:30 - 12:30 Lunch break**

* 12:30 - 13:15 Sentiment Analysis and Keyword Analysis in R

* 13:15 - 14:00 Networks and Collocation Analysis

* **14:00 - 14:30 Coffee break**

* 14:30 - 15:00 Exercise 3: Topic modelling

* 15:00 - 15:50 Topic modelling in R

* 15:50 - 16:00 Going further and wrap-up

### Resources

All resources (including the data we will use and analyse, the link to the script for this workshop, and  links to more in-depth resources for further study) are available via this [GitHub repository](https://github.com/MartinSchweinberger/IntroR_WS).

To got beyond or review what are are doing in more detail, check out the R [Basics](https://ladal.edu.au/tutorials.html#2_R_Basics) and [Text Analysis](https://ladal.edu.au/tutorials.html#5_Text_Analytics) tutorials offered by the [*Language Technology and Data Analysis Laboratory* (LADAL).](https://ladal.edu.au)

### Audience

The intended audience for this workshop is beginner-level, with no previous experience using R. However, the workshop will also be useful for intermediate and advanced users of R if they do not have substantive experience in analyzing text data with R. Thus, no prior knowledge of R is required.

If you want to know more, would like to get some more practice, or would like to have another approach to R, please feel free to check out on eof the various online resources available to learn R (you can check out a very recommendable introduction [here](https://uvastatlab.github.io/phdplus/intror.html)). 

### What to do before the workshop

In this workshop you will learn  (basic) R skills and (basic) knowledge of how to work with R and RStudio to perform basic text analytics. If you have no or little experience with this, you *can* (but *do not need or have to*) prepare or refresh your R skills by having a look at these tutorials:

* [Getting started with R](https://slcladal.github.io/intror.html)

* [Handling tables in R](https://slcladal.github.io/table.html)

Before attending the workshop, you could also install the following packages in RStudio:

* `here` (for easy pathing)
* `ggplot2`  (for general data visualization)
* `dplyr` (for data processing)
* `tsne` (for t-SNE)
* `knitr` (for knitting R Notebooks)
* `markdown` (for rendering Rmd files)
* `rmarkdown`  (for R Markdown formatting)
* `installr` (for updating R)


You can update R and install these packages by clicking on `packages` on the top of the lower right pane in RStudio or you can execute the following code in the lower left, `Console` pane of RStudio. 

```{r install, eval = F, message=F, warning=F}
# update R
#install.packages("installr")
#library(installr)
#updateR()
# install required packages
install.packages(c("here", "readxl", "dplyr", "stringr", "ggplot2", "knitr", "markdown", "rmarkdown", "devtools"), dependencies = T)
```


You can follow this workshop in different ways - you can sit back and watch it like a lecture or take a more active role - that said, the intention for this workshop is clearly to be practical so that I show something and then you do it on you computer and we have exercises where you can try out what you have just learned. Choose which option suits you best and then go with it. 


### Getting started

For everything to work, please do the following either before the workshop or at the beginning of the workshop (I will guide you if you want to do this at the begining of the workshop):

**GitHub**

* Check your GitHub log in details or create a new GitHub account

**Folder set up**

* Create a folder for this workshop somewhere on your computer, e.g. called *IntroR_WS*

* In that folder, create two subfolders called *data* and *images*

* Open RStudio, go to File > New Project > Existing Directory (Browse to project folder) > Create (and hit Enter)

This will then create an R Project in the project folder.

**Data and files**

* The data is ready for download in the data folder of the [GitHub repository for this workshop](https://github.com/MartinSchweinberger/IntroR_WS) but I will bring a USB stick with the required  data sets - please store/save them in the folder called *data* in the folder called *IntroR_WS*.


