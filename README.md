# Identification of Adult Sepsis Events 

## Objective

Identify adult sepsis events using the [CDC Adult Sepsis Event Toolkit](https://www.cdc.gov/sepsis/pdfs/sepsis-surveillance-toolkit-mar-2018_508.pdf) criteria using the [Common Longitudinal Intensive Format (CLIF) 2.0](https://clif-consortium.github.io/website/) data structure. 

## Required CLIF tables and fields

Please refer to the online [CLIF data dictionary](https://clif-consortium.github.io/website/data-dictionary.html), [ETL tools](https://github.com/clif-consortium/CLIF/tree/main/etl-to-clif-resources), and specific [table contacts](https://github.com/clif-consortium/CLIF) for more information on constructing the required tables and fields.

### To identify hospitalizations:
- **`patient`**
- **`hospitalization`**

### To identify presumed infection
-  **`microbiology_culture`**
-  **`microbiology_antibiotic`**

### To identify organ dysfunction
- **`labs`**
- **`vitals`**
- **`medication_admin_continuous`**
- **`respiratory_support`**

## Dependencies

The following R packages are required for this project:

- [`knitr`](https://cran.r-project.org/package=knitr): A general-purpose tool for dynamic report generation in R.
- [`here`](https://cran.r-project.org/package=here): A simple way to find files in R projects, relative to the project root.
- [`tidyverse`](https://cran.r-project.org/package=tidyverse): A collection of R packages for data science, including `ggplot2`, `dplyr`, `readr`, and more.
- [`arrow`](https://cran.r-project.org/package=arrow): A package for reading and writing Apache Arrow data, including Parquet files.
- [`gtsummary`](https://cran.r-project.org/package=gtsummary): A package for creating beautiful summary tables in R, often used in clinical research.

You can install all dependencies with the following command:
```r
install.packages(c("knitr", "here", "tidyverse", "arrow", "gtsummary"))
```
