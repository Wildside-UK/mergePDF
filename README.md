# PDF Merge Tool

A simple Python utility for merging PDF files using [PyPDF2](https://pypi.org/project/PyPDF2/). This tool provides two modes:

## Features

### 🔁 Interleave Mode (`I`)
Merges pages from `odd.pdf` and `even.pdf` in alternating sequence (reconstruct double-sided scans split into odd and even pages).

**Required input files:**
- `odd.pdf`
- `even.pdf`

**Result:**
- `merged.pdf` with interleaved pages (odd-even-odd-even...)

---

### ➕ Append Mode (`M`)
Appends all pages of `append.pdf` to the end of `original.pdf`.

**Required input files:**
- `original.pdf`
- `append.pdf`

**Result:**
- `merged.pdf` containing `original.pdf` followed by `append.pdf`

---

## Requirements
-  Python 3.6+ (Coded and tested using Python 3.13 but expected to work with 3.6).
-  PyPDF2

---

## Usage
1. Ensure the relevant PDF files are named as required (see above).
2. Run the script:

```bash
python merge_pdf.py
