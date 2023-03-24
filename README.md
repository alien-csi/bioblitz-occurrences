## Rationale

This repository contains the functionality to standardize the Bioblitz dataset of the AlienCSI project []() to a [Darwin Core Archive](https://ipt.gbif.org/manual/en/ipt/2.5/dwca-guide) that can be harvested by a [GBIF IPT](https://ipt.gbif.org/manual/en/ipt/2.5/).

## Workflow

[source data](https://github.com/...) → Darwin Core [mapping script](https://github.com/...) → generated [Darwin Core files](https://github.com/...)


## Published dataset

* [Dataset on the IPT]()
* [Dataset on GBIF]()

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/) and the [Checklist recipe](https://github.com/trias-project/checklist-recipe). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── README.md              : Description of this repository
├── LICENSE                : Repository license
├── bioblitz-occurrences.Rproj : RStudio project file
├── .gitignore             : Files and directories to be ignored by git
├── src
│   ├── dwc_mapping.Rmd    : Darwin Core mapping script
└── data
│   ├── raw                : Fetched data
│   └── processed          : Darwin Core output of mapping script GENERATED
```

## Installation

1. Clone this repository to your computer
2. Open the RStudio project file
3. Run `install_packages.R` to install any required packages
4. Open `fetch_data.Rmd` [R Markdown file](https://rmarkdown.rstudio.com/) in RStudio to fetch data manually
5. Open the `dwc_mapping.Rmd` [R Markdown file](https://rmarkdown.rstudio.com/) in RStudio to map data to DwC manually
6. Click `Run > Run All` to generate the processed data

## License

[MIT License](LICENSE) for the code and documentation in this repository. The included data is released under another license.
