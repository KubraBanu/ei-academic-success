# Environment Setup Guide

## Prerequisites
- R 4.1+ (https://cran.r-project.org/)
- RStudio Desktop (free: https://posit.co/downloads/)

## R Environment Setup

### 1. Clone the repository
git clone https://github.com/KubraBanu/ei-academic-success.git
cd ei-academic-success

### 2. Open RStudio
- File → Open Project or open the .Rmd file directly

### 3. Install required R packages
Run in R console:
install.packages(c("rmarkdown", "knitr", "ggplot2", "dplyr", "tidyr",
                   "rpart", "rpart.plot", "caret", "MASS",
                   "tm", "SnowballC", "corrplot", "ggcorrplot",
                   "gridExtra", "readr", "readxl"))

## Dataset
The analysis uses the MacCann et al. (2020) meta-analytic dataset:
- File: `maccann2020.csv` (included in this repository)
- Source: MacCann, C. et al. (2020). Emotional intelligence predicts academic performance: A meta-analysis. Psychological Bulletin.

## Running the Analysis

### Option A — R Markdown (Recommended)
1. Open `20241212_STAT4600_Final_project_Code_EI_Measures_KB_JK_KS_AZ.Rmd` in RStudio
2. Click "Knit" to render the full analysis as HTML
3. The rendered output will open automatically

### Option B — View Pre-rendered Output
Open `20241212_STAT4600_Final_project_Code_EI_Measures_KB_JK_KS_AZ.html` directly in a browser — no R installation needed.

### Option C — Run R Script
1. Open the `.R` script in RStudio
2. Run line by line or Source the entire file

## Key Outputs
- Regression model summaries in `model_summary.txt` through `model6_summary.txt`
- R-squared summary in `grouped_r2_summary.csv`
- Decision tree visualizations (generated when running the analysis)

## NEDSI 2025 Conference
This research was presented at the Northeast Decision Sciences Institute (NEDSI) 2025 Academic Conference.
Presentation slides: `2025_Emotional_Intelligence_Clark_University_Presentation.pptx`
Conference poster: `2025_NEDSI_Poster_Emotional_Intelligence.pptx`
