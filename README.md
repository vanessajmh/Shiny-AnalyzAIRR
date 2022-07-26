# Shiny-AnalyzAIRR

**Shiny-AnalyzAIRR** is a Shiny web application developed for the [AnalyzAIRR package](https://github.com/vanessajmh/AnalyzAIRR), making it user-friendly for biologists with little or no background in bioinformatics.

The application can be either download from the Github repository or directly used at this [link](https://analyzairr.shinyapps.io/shiny-analyzairr/).


# Package installation

The latest release of **AnalyzAIRR** can be installed from Github using devtools:

```
# Install package dependencies
#Package Dependencies installation
list.pkgs <- c("shiny", "shinydashboard", "shinysky", "shinyjs", "shinythemes", "shinyWidgets", "rmarkdown","markdown", "BiocStyle","devtools")
pkgs <- list.pkgs[!(list.pkgs %in% installed.packages()[,"Package"])] if(length(pkgs)>0)
install.packages(pkgs)

# AnalyzAIRR installation
devtools::install_github("vanessajmh/AnalyzAIRR")

```

**Shiny-AnalyzAIRR** should be cloned as follow:
```
# Clone the repository in commande line:
git clone https://github.com/vanessajmh/Shiny-AnalyzAIRR
```


# Getting started

**Shiny-AnalyzAIRR** can be launched from the terminal:
```
# Go to the Shiny-AnalyzAIRR folder
cd Shiny-AnalyzAIRR
# Launch R and shiny
R -e 'shiny::runApp("./")'
```

Alternatively, it can be run through Rstudio:
```
# Open global.R and run
shiny::runApp("./")
```
The interface can be opened in a web browser using the displayed hyper link address.

# Data loading

**Shiny-AnalyzAIRR** proposes two different data loading processes.

**1. Upload a RepSeqExperiment object**

A **RepSeqExperiment** object generated using the **AnalyzAIRR** R package and saved in an rds format can be used.

**2. Upload alignment files in AnalyzAIRR-compliant formats**

More details on how to prepare the input data can be found [here](https://vanessajmh.github.io/AnalyzAIRR.github.io/)
