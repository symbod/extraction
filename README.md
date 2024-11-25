# Extraction

This repository contains the code and result images accompanying the paper:

**Systematic Comparison of Bone Proteome Extraction Methods to Allow for Integrated Proteomics-Metabolomics-Correlation**

## Overview
- **Result Images**: The `results` directory contains the figures and supplementary images generated for the paper.
- **R Markdown File**: The `.Rmd` file (`Workflow.Rmd`) allows you to run the code used in the analysis and recreate the result images.
- **Environment**: The corresponding computational environment required to run the code can be found as a Docker image on Docker Hub.

## Running the Analysis
To recreate the result images:
1. Ensure you have R and the required environment configured. Using the Docker image is recommended for reproducibility.
2. Run the `Workflow.Rmd` file in your R setup or RStudio.

### Docker Environment
The computational environment for running the code is available on Docker Hub:

- Docker Hub Repository: [kadam0/extraction_prot](https://hub.docker.com/repository/docker/kadam0/extraction_prot)
- Tags:
  - `rstudio`: Provides a GUI-based environment with RStudio.
  - `r`: Allows running the code in a terminal-based R environment.

### Using the Docker Environment
1. Pull the Docker image:
   ```bash
   docker pull kadam0/extraction_prot:rstudio
   ```
2. Run the container:
   ```bash
   docker run -p 8787:8787 -e PASSWORD=yourpassword kadam0/extraction_prot:rstudio
   ```
3. Access RStudio in your browser at `http://localhost:8787` and run `Workflow.Rmd`.

## Citation
If you use this repository or the Docker environment, please cite the associated paper:

**Systematic Comparison of Bone Proteome Extraction Methods to Allow for Integrated Proteomics-Metabolomics-Correlation.**

---
For any issues or questions, feel free to contact the repository maintainers or refer to the paper for detailed
