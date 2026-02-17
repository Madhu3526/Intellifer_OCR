# PDF Table Extraction using OpenCV and Tesseract

## Overview

This project extracts tables from PDF documents and converts them into structured CSV files using classical computer vision techniques.

It detects table structures using morphological operations and applies OCR to extract cell text.

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

## How to Run

Update:

PDF_PATH  
PAGE_INDEX  
TESSERACT_PATH  
POPPLER_PATH  

Then run:

python main.py

Extracted tables will be saved in:

extracted_output/

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
- LayoutLM integration
