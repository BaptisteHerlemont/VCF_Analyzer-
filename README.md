# VCF File Analyzer

This project provides a script for analyzing Variant Call Format (VCF) files to extract detailed information by sites and genotypes. It leverages a Python script embedded within a Quarto (R) script to examine the VCF file, generate output files, and then analyze these files to create an HTML report featuring various statistics, tables, and figures.

## Features

- **VCF File Analysis:** Utilizes `cyvcf2` to read and analyze VCF data.
- **Report Generation:** Produces HTML reports including statistics, tables, and figures based on the analysis.
- **Python and R Integration:** Combines Python's analysis capabilities with R's visualization and reporting tools.

## Prerequisites

To use this project, you will need the following installed on your system:

(Versions of the programs used during development)

- Python 3.10.13
- R 4.1.2 
- Quarto (RStudio)
- The Python package `cyvcf2`
- Necessary R libraries for data processing and report generation

## Installation

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/BaptisteHerlemont/VCF_Analyzer-.git
    ```

2. Install Python dependencies:

    ```bash
    pip3 install cyvcf2
    ```

3. Ensure you have the required R dependencies installed.


The analysis relies on various R libraries. You can install these libraries by running the following commands in your R console or RStudio:

```r
install.packages("ggplot2")
install.packages("dplyr")
install.packages("knitr")
install.packages("MetBrewer")
install.packages("tidyr")
install.packages("plotly")
install.packages("viridis")
install.packages("reticulate") 
```
If you encounter no errors, you're ready to proceed with the analysis.


## Usage

To start the analysis and generate the report, follow these steps:

1. Ensure the Quarto script is in the same directory as your VCF file.
2. Open the Quarto script in RStudio. You can modify the names of the input and output files within the script as shown below:

    ```r
    {r setup, include=FALSE}
    input_vcf_file <- "YourInputFileName.vcf.gz"  # Change "YourInputFileName.vcf.gz" to the name of your VCF file
    output_csv_file_bySite <- "OutputFileNameBySite.csv"  # Change "OutputFileNameBySite.csv" to your desired output file name for site data
    output_csv_file_byGeno <- "OutputFileNameByGeno.csv"  # Change "OutputFileNameByGeno.csv" to your desired output file name for genotype data
    ```

    Replace `YourInputFileName.vcf.gz`, `OutputFileNameBySite.csv`, and `OutputFileNameByGeno.csv` with the actual names of your files.

3. After setting up the file names, run the Quarto script to perform the analysis. The generated HTML report and CSV files will be available in the output directory.

*Note: All figures generated in the report are colorblind friendly, ensuring accessibility for all users.*


## Contributing

Contributions to this project are welcome. If you wish to contribute, please fork the repository, create a branch for your changes, and submit a pull request.


## Contact

For any questions or suggestions, feel free to open an issue in the GitHub repository.
