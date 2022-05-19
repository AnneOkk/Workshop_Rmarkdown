+++
title = "R Markdown Workshop - Preparation"
description = ""
tags = [
    "R Markdown",
    "workshop preparation",
]
date = "2022-05-18"
categories = [
    "Workshop",
    "R Markdown",
]
menu = "main"
+++


**~ 45 minutes**

## 1) Install R 

Please make sure that you have a [recent R version](https://cran.rstudio.com/) installed (>= 4.0.0 is recommended). 
You can check your R Version in the Console (in RStudio) by typing:


```R.version.string```

If you are using an older R version, please install the [newest R version](https://cran.rstudio.com/). 

## 2) Install R Studio 

Go to the [RStudio website](https://www.rstudio.com/) and download the newest version if you are using an older version of RStudio (if in doubt, better update!). Simply follow the download instructions. The new version will be available next time you open RStudio. 


## 3) Install necessary packages 

You need several R packages for the workshop. Please make sure to install these packages before the workshop. The easiest way to do so is by running this code in your R console or terminal: 

```tpl
cran_packs <- c("flexdashboard", "learnr", "bookdown",
                "officer", "rticles", "webshot",
                "tidyverse", "remotes", "magick", "stargazer",
                "kableExtra", "vtable", "devtools")
```

```tpl
install.packages(cran_packs, dependencies = TRUE)
```

```tpl
github_packs <- c('rstudio/blogdown',
                  'haozhu233/kableExtra', 'crsh/papaja')
```

```tpl
remotes::install_github(github_packs, dependencies = TRUE)
```

Once these packages are installed, you may use blogdown to install the Hugo package. Hugo is a static site generator that we will use to build blogdown paged. You may install Hugo using blogdown, like so: 

```tpl
blogdown::install_hugo()
```

You can check whether the installations were successful by running ```library(package_name)```. All installed packages must be loaded before we can use them during the workshop. 


## Set up Git and GitHub


To make the most out of the workshop, I highly encourage you to install Git and to create a GitHub account for version control. 
Follow the instructions from the [Happy Git with R Book](https://happygitwithr.com/) and the official [GitHub guides](https://docs.github.com/en/get-started/quickstart/set-up-git): 


1. [Register a GitHub account](https://happygitwithr.com/github-acct.html)

2. [Install Git](https://docs.github.com/en/get-started/quickstart/set-up-git). Follow the instructions under **Setting up Git** (do not use the Desktop client). For **Windows Users**: Follow the installation instructions for Git [here](https://www.computerhope.com/issues/ch001927.htm). 

### Once this is done, you are all set for the workshop! 🎉

## 4) Sign up on osf


Many social scientists use osf to store their data or code. It is possible to integrate your GitHub repositories into osf.
Please [sign up on osf](https://osf.io/) before the workshop. 


## 5) Install TeX

- Windows: [MikTeX](https://miktex.org/)
- Mac: [MacTeX](http://www.tug.org/mactex/)




