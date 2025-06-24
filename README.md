# 🧠 Toxic Comment Detection from Images

This AI project performs **multi-label classification** of text extracted from images to identify toxic content such as `toxic`, `severe_toxic`, `obscene`, `threat`, `insult`, and `identity_hate`. It combines **OCR**, **NLP**, **grammar correction**, and **machine learning** into a single workflow.


## 🚀 Features

- 📷 Extracts text from uploaded images using `pytesseract`
- ✍️ Cleans and corrects grammar using a transformer model (`vennify/t5-base-grammar-correction`)
- 📊 Classifies text into multiple toxicity categories using SVM
- 📈 Trained on the Jigsaw Toxic Comment dataset with TF-IDF features


## 🔧 Technologies Used

- Python, Tesseract OCR, Transformers (HuggingFace), Scikit-learn
- Preprocessing with PIL, OpenCV
- Model training with SVM (OneVsRestClassifier)
- Deployment-ready with Flask/Streamlit (optional)


## 🛠 Installation

```bash
pip install pytesseract transformers scikit-learn joblib opencv-python-headless
```
📝 How it Works
1-Upload an image (.jpg, .jpeg, .png)
2-OCR extracts the text
3-Grammar corrected using a Transformer
4-TF-IDF vectorization
5-SVM predicts the labels


📊 Results
Multi-label accuracy: 91%
Handles blurry or unclear images with preprocessing
Useful in moderation tools, comment filtering, or educational platforms
