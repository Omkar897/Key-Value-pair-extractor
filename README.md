# Key-Value Pair Extractor

## Overview
The **Key-Value Pair Extractor** is a Python-based tool designed to extract structured key-value pairs from text documents, specifically from medical prescriptions and invoices. It leverages **PyTesseract (OCR)** and **OpenCV** for text extraction and utilizes **custom NLP techniques** to parse and organize the extracted data into meaningful pairs.

## Features
✅ **Optical Character Recognition (OCR)** using PyTesseract  
✅ **Preprocessing** (Noise removal, Thresholding, Contour detection)  
✅ **Custom NLP-based Key-Value Matching**  
✅ **Export Data to Excel or JSON**  
✅ **Handles Noisy and Unstructured Data**  

## Tech Stack
- **Python**
- **OpenCV** (Image preprocessing)
- **PyTesseract** (OCR engine)
- **NLTK / spaCy** (For text processing)
- **Pandas** (Data handling and export)
- **Streamlit** (Optional - for UI)

## Installation
```bash
# Clone the repository
git clone https://github.com/Omkar897/key-value-pair-extractor.git
cd key-value-extractor

# Create a virtual environment (optional)
python -m venv venv
source venv/bin/activate  # On Windows use 'venv\Scripts\activate'

# Install dependencies
pip install -r requirements.txt
```

## Usage
1. **Run the script**
   ```bash
   python extractor.py --input sample_image.jpg --output result.json
   ```
2. **Optional: Run with UI (Streamlit)**
   ```bash
   streamlit run app.py
   ```
3. The extracted key-value pairs will be saved in JSON or Excel format.

## Example Output
```json
{
    "Patient Name": "John Doe",
    "Age": "45",
    "Prescription Date": "2024-02-06",
    "Medicine": "Paracetamol 500mg"
}
```

## Future Improvements
- Improve NLP-based key-value detection
- Add support for more document formats (PDF, Scanned Docs)
- Deploy as a web-based API for remote processing

## Contributing
Feel free to fork the repository and submit pull requests for improvements!

## License
This project is licensed under the **MIT License**.

