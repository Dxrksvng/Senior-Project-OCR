Presentation Project1: [https://canva.link/2kb5cqji5elbsfc](https://canva.link/2kb5cqji5elbsfc)
Presentation Project2: [https://canva.link/qj231zk1nqbb44d](https://canva.link/qj231zk1nqbb44d)

# 🎓 Automated Verification of English Proficiency Test Scores Using OCR for Graduation Qualification

> **AI-powered OCR system for automatic validation of English proficiency test results.**
> This project streamlines the graduation qualification process by converting score report images (TOEIC, KMITL-TEP, IELTS) into structured, verifiable data using Optical Character Recognition (OCR) and rule-based verification.

---

## 🧠 Overview

The project eliminates the need for manual verification of English proficiency scores required for graduation. It leverages AI and OCR to detect, extract, and validate information from scanned documents, achieving 99% accuracy and significantly reducing staff workload.

---

## 🚀 Key Features

* Multi-OCR model integration: Tesseract, EasyOCR, TrOCR
* Automated image preprocessing (noise reduction, skew correction, contrast enhancement)
* Document classification (test type detection)
* Rule-based verification against graduation criteria
* Structured JSON output for downstream systems
* FastAPI-based web dashboard for uploads and verification

---

## 🧮 System Architecture

```
Uploaded Report → Pre-processing → OCR Engine → Data Parsing → Rule-based Verification → JSON Output → Web Dashboard
```

---

## 📊 Model Evaluation

| Model     | Approach | Accuracy (%) | WER (%) | CER (%) | F1-score (%) |
| --------- | -------- | ------------ | ------- | ------- | ------------ |
| EasyOCR   | Boxing   | 99.75        | 0.25    | 0.16    | 99.79        |
| EasyOCR   | Pure     | 77.17        | 22.83   | 22.71   | 86.30        |
| Tesseract | Boxing   | 99.77        | 0.23    | 0.17    | 99.82        |
| Tesseract | Pure     | 81.80        | 18.20   | 15.22   | 86.89        |
| TrOCR     | Boxing   | 99.63        | 0.37    | 0.18    | 99.67        |
| TrOCR     | Pure     | 0.00         | 100.00  | 100.00  | 0.00         |

---

## 🛠️ Tech Stack

* **Language:** Python 3.11
* **Framework:** FastAPI, Flask
* **Libraries:** OpenCV, Pytesseract, EasyOCR, Transformers
* **Database:** MySQL / SQLite
* **Evaluation:** jiwer, scikit-learn
* **Deployment:** XAMPP / Localhost / Cloud VM

---

## ⚙️ Setup Instructions

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/english-ocr-verification.git
   cd english-ocr-verification
   ```
2. **Create and activate a virtual environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # macOS/Linux
   venv\Scripts\activate     # Windows
   ```
3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```
4. **Run the server**

   ```bash
   uvicorn main:app --reload
   ```

Access the app at [http://127.0.0.1:8000](http://127.0.0.1:8000).

---

## 📈 Example Output

```json
{
  "test_type": "TOEIC",
  "candidate_name": "Nattakamon J.",
  "score": 785,
  "status": "PASS",
  "criteria": ">= 550",
  "verified_by": "OCR Automated System",
  "date_verified": "2025-11-12"
}
```

---

## 💡 Research Contributions

* Multi-OCR comparative evaluation pipeline
* Preprocessing optimization raising accuracy to 99%
* Rule-based validation adaptable to any institution
* FastAPI integration for real-time API usage
* Quantitative evaluation (Accuracy, F1, WER, CER)

---

## 🔹 Future Enhancements

* Extend support for IELTS, CU-TEP, TU-GET
* Add multilingual recognition (Thai/English)
* Integrate with Oracle DB and student systems
* Deploy using Docker or AWS Lambda

---

## 📓 Citation

> Jaimetha, N. (2025). *Automated Verification of English Proficiency Test Scores Using OCR for Graduation Qualification.*
> King Mongkut’s Institute of Technology Ladkrabang (KMITL), Faculty of Information Technology.

---

## 👨‍💻 Author

**Nattakamon Jaimetha (jdiih)**
Data Science & Business Analytics – KMITL
📧 [Email] (nattakamon0208@gmail.com)
🌐 [GitHub](https://github.com/Dxrksvng) | [LinkedIn](https://www.linkedin.com/in/nattakamon-jaimetha)

---

