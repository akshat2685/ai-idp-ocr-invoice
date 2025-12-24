# AI-Based Intelligent Document Processing (IDP)

This project demonstrates a basic end-to-end pipeline for **Intelligent Document Processing (IDP)** using **OCR, Python, and NLP concepts**. The objective is to extract structured information from unstructured document images.

---

## 📄 Document Type
**Invoice**

A sample invoice image is used to demonstrate text extraction and key-field identification.

---

## 🛠️ Tools & Technologies Used

- **Python**
- **Tesseract OCR** – for text extraction
- **OpenCV** – image preprocessing
- **Regex** – rule-based information extraction
- **JSON** – structured output format
- **Google Colab** – development environment

---

## 🧠 Approach

1. **Document Input**  
   An invoice image is uploaded to the system.

2. **Image Preprocessing**  
   The image is converted to grayscale and thresholding is applied to improve OCR accuracy.

3. **Text Extraction (OCR)**  
   Tesseract OCR is used to extract raw textual content from the processed image.

4. **Key Field Identification**  
   Important fields such as:
   - Invoice Number  
   - Invoice Date  
   - Total Amount  
   are extracted using regular expressions.

5. **Structured Output**  
   The extracted fields are organized into a clean **JSON format**, making the data suitable for downstream applications.

---

## 📊 Sample Output (JSON)

```json
{
    "invoice_number": "INV-1023",
    "date": "12-08-2024",
    "total_amount": "12450"
}
