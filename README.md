# Dataset of User Reviews for Low-Rated Amazon Appstore Applications


## Overview

This repository contains a dataset of 79,821 user reviews from 64 low-rated software applications sourced from the Amazon Appstore. In the literature, more emphasis has been given to high-rating and popular applications, while low-rating apps have been largely ignored. This dataset was created to address this gap, providing a concentrated resource for systematically studying the root causes of user dissatisfaction and software failure. It is intended for researchers, developers, and practitioners interested in software quality, requirements engineering, and user experience analysis.

## Dataset Details

### File Description

* **File:** `low_rated_app_reviews.csv`
* **Format:** Comma-Separated Values (CSV)
* **Encoding:** UTF-8
* **Rows:** 79,821
* **Columns:** 3

### Data Schema

The dataset consists of three primary columns:

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `Stars` | Text | The quantitative star rating assigned by the user (e.g., "1.0 out of 5 stars"). |
| `Title_of_Review` | Text | The headline or summary of the review provided by the user. |
| `Base_Review` | Text | The full, detailed text of the user's feedback, describing their experience. |

### Steps to Reproduce
The dataset was created by following a systematic process of application selection, data extraction, and data cleaning. The workflow can be reproduced using the steps outlined below:

1. Application Identification and Selection
- Identify a pool of applications on the Amazon Appstore.
- Apply specific filtering criteria to select the final applications for inclusion. The criteria used for this dataset were:
    - A user rating of 3.0 stars (out of 5) or lower.
    - A minimum of 350 individual user reviews.
- Compile a final list of applications that meet these requirements. For this dataset, 64 applications were selected.

2. Data Extraction
- Utilize an automated web scraping tool. This dataset was created using the "Instant Data Scraper" Google Chrome extension.
- For each selected application, navigate to its user reviews pages on the Amazon Appstore.
- Configure the scraping tool to extract the following data fields for each individual review: the user's star rating (`Stars`), the title of the review (`Title_of_Review`), and the full review text (`Base_Review`).
- Export the scraped data into a spreadsheet format, such as CSV or XLSX.

3. Data Verification and Cleaning
- Manually cross-check a sample of the extracted data against the live Amazon Appstore listings to verify accuracy.
- Consolidate the data scraped from all applications into a single master dataset.
- Process the dataset to remove any duplicate entries, formatting inconsistencies, or irrelevant artifacts from the scraping process.

4. Manual Categorization
- Manually review the primary function of each of the 64 selected software applications.
- Assign each application to one of the 14 predefined functional categories outlined in the associated data paper.

The final output of this reproducible process is the single, cleaned CSV file contained in this repository.

### How to Cite
Nek Dil Khan (2025), "Dataset of User Reviews from 64 Low-Rated Applications on the Amazon Appstore", Mendeley Data, V1, doi: 10.17632/zztwrn36n8.1

@data{khan_2025_dataset,
  author = {Khan, Nek Dil},
  title = {Dataset of User Reviews for Low-Rated Applications on the Amazon Appstore},
  year = {2025},
  publisher = {Mendeley Data},
  version = {V1},
  doi = {10.17632/zztwrn36n8.1}
}


###Authors
Nek Dil Khan
(nekdil2003@gmail.com)


