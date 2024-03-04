# VCF File Analyzer

This project provides a script for analyzing Variant Call Format (VCF) files to extract detailed information by sites and genotypes. It leverages a Python script embedded within a Quarto (R) script to examine the VCF file, generate output files, and then analyze these files to create an HTML report featuring various statistics, tables, and figures.

## Features

- **VCF File Analysis:** Utilizes `cyvcf2` to read and analyze VCF data.
- **Report Generation:** Produces HTML reports including statistics, tables, and figures based on the analysis.
- **Python and R Integration:** Combines Python's analysis capabilities with R's visualization and reporting tools.

## Prerequisites

To use this project, you will need the following installed on your system:

- Python 3.x
- R
- Quarto
- The Python package `cyvcf2`
- Necessary R libraries for data processing and report generation

## Installation

1. Clone the repository to your local machine:

    ```bash
    git clone https://yourrepository.github.com/vcf-analyzer.git
    ```

2. Install Python dependencies:

    ```bash
    pip install cyvcf2
    ```

3. Ensure you have the required R dependencies installed.

## Usage

To start the analysis and generate the report:

1. Place your VCF file in the appropriate directory.
2. Run the main script (add specific commands here).
3. The generated HTML report will be available in the output directory.

## Project Structure

- `script.py`: Python script for the initial analysis of the VCF file.
- `report.qmd`: Quarto (R) script for report generation.
- `/data`: Directory for input VCF files.
- `/output`: Directory for output files and generated reports.

## Contributing

Contributions to this project are welcome. If you wish to contribute, please fork the repository, create a branch for your changes, and submit a pull request.

## License

This project is distributed under the MIT License. See the `LICENSE` file for more details.

## Contact

For any questions or suggestions, feel free to open an issue in the GitHub repository or contact me directly (add your contact information).
