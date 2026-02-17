# PDF Table Extraction using OpenCV and Tesseract

## Overview

A rule-based PDF table extraction pipeline built using computer vision and OCR.
This project detects tables from PDF documents, extracts structured cell content, and exports the results as CSV files.
It is designed to demonstrate how table extraction works internally using classical image processing techniques instead of deep learning-based document AI models.

---

## Features

- Converts PDF pages to images
- Detects table structure using morphological operations
- Extracts cell bounding boxes
- Groups cells into rows and tables
- Performs OCR on each cell using Tesseract
- Cleans noisy OCR output
- Exports each table as a CSV file
- Supports multiple tables per page

---

## Technologies Used

- OpenCV
- Tesseract OCR
- pdf2image + Poppler
- Pandas
- NumPy

---

## Installation

### 1. Install Python dependencies

pip install -r requirements.txt

### 2. Install Tesseract OCR

Download:
https://github.com/UB-Mannheim/tesseract/wiki

Update path in main.py

### 3. Install Poppler

Download:
https://github.com/oschwartz10612/poppler-windows/releases

Update poppler_path in main.py

---

## Limitations

- Borderless tables not supported
- Complex merged cells partially supported
- OCR accuracy depends on scan quality

---

## Future Improvements

- Borderless detection
- Header detection
- Multi-page automation
