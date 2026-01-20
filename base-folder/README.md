# TOPSIS-102303670

**for:** Project-1 (UCS633)  
**submitted by:** Karanveer Singh  
**Roll No:** 102303670  
**Group:** 3C45  

`topsispackage1.1.1` is a Python library for solving **Multiple Criteria Decision Making (MCDM)** problems using the  
**Technique for Order of Preference by Similarity to Ideal Solution (TOPSIS).**

---

## Installation

Use the package manager **pip** to install this package:

```bash
pip install topsispackage1.1.1


## usage

This package takes a CSV file as input, along with weights and impacts, and generates a result CSV file
containing Topsis Score and Rank.

Input Rules

The dataset must be a .csv file

The first column should contain names/IDs (non-numeric)

All columns from 2nd onwards must be numeric

The file must contain at least 3 columns

Number of weights and impacts must match the number of numeric columns

Impacts must contain only + or -


Python Function Usage

from topsis import topsis

topsis(
    "102303670-data.csv",
    "1,1,1,1,2",
    "+,+,-,+,+",
    "102303670-result.csv"
)