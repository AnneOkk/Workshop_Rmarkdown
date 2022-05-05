---
author: "Anne"
---

# Preparation


{{< tabs "prep" >}}
{{< tab "Install R and RStudio" >}}
# Install R and Rstudio 

**~ 10 minutes**

## Install R 

Please make sure that you have a [recent R version](https://cran.rstudio.com/) installed (>= 4.0.0 is recommended). 
You can check your R Version in the Console (in RStudio) by typing:


```R.version.string```

If you are using an older R version, please install the newest R version. 


## Install RStudio 

You may install RStudio [here](https://www.rstudio.com/products/rstudio/download/#download). If you already have Rstudio installed, check your RStudio version like this (on a Mac):

<img src="/docs/R_Markdown_Workshop/before/first-page_files/RStudioVersion.png" alt="" width="45%"/>

Go to the [RStudio website](https://www.rstudio.com/) and download the newest version if you are still using an older version of RStudio. Simply follow the download instructions. The new version will be available next time you open RStudio. 

{{< /tab >}}

{{< tab "Install necessary packages" >}}


# Install necessary packages 

**~ 10 minutes**

You need several R packages for the workshop. Please make sure to install these packages before the workshop. The easiest way to do so is by running this code in your R console or terminal: 

```tpl
cran_packs <- c("flexdashboard", "learnr", "bookdown",
                "officer", "rticles", "webshot",
                "tidyverse", "remotes", "magick")
```

```tpl
install.packages(cran_packs, dependencies = TRUE)
```

```tpl
github_packs <- c('rstudio/blogdown',
                  'haozhu233/kableExtra')
```

```tpl
remotes::install_github(github_packs, dependencies = TRUE)
```

Once these packages are installed, you may use blogdown to install the Hugo package. Hugo is a static site generator that we will use to build blogdown paged. You may install Hugo using blogdown, like so: 

```tpl
blogdown::install_hugo()
```

You can check whether the installations were successful by running ```library(package_name)```. All installed packages must be loaded before we can use them during the workshop. 

{{< /tab >}}

{{< tab "Git and GitHub" >}}

# Git and GitHub

**~ 30 minutes**

To make the most out of the workshop, I highly encourage you to install Git and to create a GitHub account for version control. 
Follow the instructions from the [Happy Git with R Book](https://happygitwithr.com/) and the official [GitHub guides](https://docs.github.com/en/get-started/quickstart/set-up-git): 


1. [Register a GitHub account](https://happygitwithr.com/github-acct.html)

2. [Install Git](https://docs.github.com/en/get-started/quickstart/set-up-git). Follow the instructions under **Setting up Git** (do not use the Desktop client).

Once this is done, you are all set for the workshop! We will not delve into all the possibilities offered by Git and GitHub, but we will learn how to fork a repository to use someone else's project as a starting point for your own idea. 


{{< /tab >}}

{{< tab "osf" >}}

# Sign Up on osf

**~ 5 minutes**

Many social scientists use osf to store their data or code. It is possible to integrate your GitHub repositories into osf, so you no longer have to take care of multiple online repositories. 
Please [sign up on osf](https://osf.io/) before the workshop. 


{{< /tab >}}
{{< /tabs >}}

