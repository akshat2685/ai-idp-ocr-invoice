# 📄 AI-Based Intelligent Document Processing (IDP)

This repository demonstrates a simple end-to-end Intelligent Document Processing (IDP) pipeline using OCR (Optical Character Recognition) and basic NLP techniques in Python. It extracts text from an invoice image, identifies important fields, and structures them in JSON format.

---

## 🧾 Document Type
**Invoice**

We use a sample invoice image to extract:
- Invoice Number
- Date
- Total Amount

---

## 🛠️ Tools & Technologies

**Languages & Libraries**
- Python
- Google Colab

**OCR & Image Processing**
- Tesseract OCR (`pytesseract`)
- OpenCV for preprocessing

**Text Processing**
- Regular Expressions (Regex)
- JSON for output formatting

---

## 🚀 Approach

1. **Image Upload:**  
   Upload a scanned invoice image to Colab.

2. **Image Preprocessing:**  
   Convert the image to grayscale and apply thresholding to improve OCR accuracy.

3. **Text Extraction:**  
   Use Tesseract OCR to extract text from the processed invoice image.

4. **Field Extraction:**  
   Parse the OCR text using regex to extract key fields like invoice number, date, and totals.

5. **Structured Output:**  
   Output the extracted information in clean **JSON format**.

---

## 🧪 Sample Output

```json
{
    "invoice_number": "INV-1023",
    "date": "12-08-2024",
    "total_amount": "12450"
}
