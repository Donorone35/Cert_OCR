# OCR-Certificate-Extractor

This repository contains a **OCR framework** for **extracting structured data from academic certificates**.  
It uses **pytesseract OCR**, **OpenCV**, and **PDF/image preprocessing** to handle tasks like **text extraction, semester report parsing, and JSON output generation**.

## Key Features
- **Multi-Format Support:** Handles PDF, PNG, JPG, and GIF certificates.
- **Advanced Preprocessing:** Grayscale conversion, denoising, resizing, and adaptive thresholding to improve OCR accuracy.
- **Structured JSON Output:** Extracts student name, roll/registration numbers, programme, semester, courses, SGPA/CGPA, and remarks.
- **Hash & Metadata Tracking:** Computes SHA256 hash of certificate images and logs environment metadata.
- **Colab Compatible:** Fully functional in Google Colab.
- **Modular Design:** Easily extensible for new certificate formats.

## Technology Used
### Languages & Libraries
- Python 3.10+
- pytesseract (OCR engine)
- OpenCV (image preprocessing)
- Pillow (image handling)
- pdf2image (PDF → image conversion)
- numpy (numerical processing)
- requests (optional public IP metadata)
- python-dateutil (date parsing)

### OCR & Parsing
- **OCR Engine:** pytesseract
- **Preprocessing:** Grayscale, denoise, resize, adaptive thresholding
- **Parsing Rules:** KIIT-style semester grade reports

## Project Structure
```
Cert_OCR/
│── Examples/ # Sample inputs & JSON files
│ ├── SEM_6_Report_Card.pdf
│ ├── SEM_6_Report_Card_extracted.json
│ ├── SEM_6_Report_Card_page-0001.jpg
│ └── SEM_6_Report_Card_page-0001_extracted.json
│── Cert_OCR.py # Main OCR script
│── requirements.txt # Python dependencies
│── README.md # Project documentation
│── LICENSE # MIT License

```

## Installation & Usage
### Installation
1. **Clone the Repository**
```bash
git clone https://github.com/Donorone35/Cert_OCR.git
cd Cert_OCR
pip install -r requirements.txt
```

## **Contact**
- **Author:** Trayambak Rai
- **GitHub:** [Donorone35](https://github.com/Donorone35)
- **LinkedIn:** [Trayambak Rai](https://www.linkedin.com/in/trayambak-rai-314606278/)
