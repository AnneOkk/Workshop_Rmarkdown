---
author: "Anne"
weight: 2
---

# Relevant R packages 

You need several R packages for the workshop. Please make sure to install these packages before the workshop. The easiest way to do so is by running this code in your R console or terminal: 

```{r}
cran_packs <- c("flexdashboard", "learnr", "bookdown",
                "officer", "rticles", "webshot",
                "tidyverse", "remotes", "magick")
```

```
install.packages(cran_packs, dependencies = TRUE)
```

```
github_packs <- c('rstudio/blogdown',
                  'haozhu233/kableExtra')
```

```
remotes::install_github(github_packs, dependencies = TRUE)
```

Once these packages are installed, you may use blogdown to install the Hugo package. Hugo is a static site generator that we will use to build blogdown paged. You may install Hugo using blogdown, like so: 

```
blogdown::install_hugo()
```

You can check whether the installations were successful by running ```library(package_name)```. All installed packages must be loaded before we can use them during the workshop. 


