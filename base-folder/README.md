# TOPSIS Ranking Tool  
### By Karanveer Singh (Roll No: 102303670)

This command-line tool applies the TOPSIS (Technique for Order Preference by Similarity to Ideal Solution) method to rank alternatives based on multiple quantitative criteria.

---

## Installation

pip install Topsis-Karanveer-102303670

---

## Input Data Format

The input must be a CSV file with the following structure:

Column 1: Alternatives  
Column 2 onwards: Numerical criteria values

Example:

| City | AirQuality | Cost | Transport | Safety |
|------|------------|------|-----------|--------|
| C1 | 72 | 32000 | 7 | 8 |
| C2 | 88 | 47000 | 9 | 6 |
| C3 | 65 | 28000 | 6 | 9 |
| C4 | 80 | 36000 | 8 | 8 |

---

## Weights and Impacts

Weights (comma separated):

0.30,0.20,0.25,0.25

Impacts (comma separated):

+,-,+,+

---

## Usage

topsis <input_file.csv> <weights> <impacts> <output_file.csv>

Example:

topsis city.csv "0.30,0.20,0.25,0.25" "+,-,+,+" ranks.csv

---

## Output Format

The output CSV will contain:

City, Score, Rank

Example:

C1, 0.51, 3  
C2, 0.56, 2  
C3, 0.44, 4  
C4, 0.67, 1

Higher score means better rank.

---

## Error Handling

The program checks for:

Incorrect number of arguments  
Non-numeric values in criteria columns  
Invalid impact symbols (+ or - only)  
Incorrect CSV format

Appropriate error messages are displayed for invalid input.

---

## Conclusion

This tool helps in decision making by converting multiple evaluation criteria into a single composite score using the TOPSIS method.



# TOPSIS Project (Complete Submission)
### By Karanveer Singh (Roll No: 102303670, Group: 3C45)

This repository contains the complete TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution) project submission.

In this project, we have done **three major parts**:

✅ **1) TOPSIS Implementation Notebook (Colab/Jupyter)**  
✅ **2) TOPSIS Python Package Deployment on PyPI**  
✅ **3) TOPSIS Web Service Deployment Online (Website)**  

All detailed explanation and working screenshots/results are already provided in the **above `.md` file(s)** in this repository.

---

## ✅ Project Overview

TOPSIS is a popular Multi-Criteria Decision Making (MCDM) technique used to rank multiple alternatives based on multiple criteria.

This project helps to:
- Take a dataset (CSV)
- Take weights and impacts
- Compute TOPSIS score for each alternative
- Generate a ranked output CSV
- Provide results through a web interface
- Send output CSV to the user using email

---

# ✅ Part 1: Notebook Submission

A complete notebook solution is included in this repository.
It contains:
- Dataset loading
- Weight & impact processing
- TOPSIS calculations
- Final ranking output generation
- Example runs and output demonstration

📌 Notebook file available inside:  
`/notebook/`

---

# ✅ Part 2: PyPI Package Deployment

We also deployed our TOPSIS logic as a Python package on **PyPI**.

### ✅ Package Installation
pip install Topsis-Karanveer-102303670

✅PyPI Link
🔗 (Paste your PyPI project link here):
https://pypi.org/project/Topsis-Karanveer-102303670/

Part 3: Web Service Deployment (Online)

We also developed and deployed a TOPSIS Web Service where the user can upload the input file, provide weights, impacts and email.

✅ Website Features

Upload CSV file
Enter weights and impacts
Enter correct email id
Get output CSV via email
Validations included:
CSV file required
numeric columns validation
weight & impacts count match
impacts must contain only + or -

✅ Live Website Link

🔗 (Paste your Render live website link here):
https://topsis-webservice-l1tm.onrender.com


topsis-assignment/
│
├── README.md
│
├── notebook/
│ ├── TOPSIS_Project.ipynb
│ └── (optional) Report.pdf
│
├── pypi_package/
│ ├── setup.py
│ ├── README.md
│ ├── libname/
│ │ ├── init.py
│ │ └── topsis.py
│ └── dist/
│ ├── (optional, not compulsory to upload)
│
├── webservice/
│ ├── app.py
│ ├── requirements.txt
│ ├── templates/
│ │ └── index.html
│ ├── uploads/
│ │ └── (empty folder or .gitkeep)
│ ├── outputs/
│ │ └── (empty folder or .gitkeep)
│ └── .gitignore
│
├── sample_files/
│ ├── 102303670-data.csv
│ └── 102303670-result.csv
│
└── screenshots/
├── pypi_page.png
├── render_deploy.png
└── web_output.png
