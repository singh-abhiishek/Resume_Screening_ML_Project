# Resume Screening App using Machine Learning

An end-to-end Resume Screening Web Application built using Python, Machine Learning, and Streamlit.  
This project classifies resumes into different job categories using Natural Language Processing (NLP) techniques.

---

## Project Overview

This application predicts the job category of a resume based on its textual content.  
It uses TF-IDF vectorization for feature extraction and a trained machine learning classification model for prediction.

The trained model, label encoder, and vectorizer are saved as serialized `.pkl` files and loaded inside the application for real-time inference.

---

## Features

- Resume classification using Machine Learning
- TF-IDF based text vectorization
- Label Encoding for category mapping
- Pre-trained ML model for prediction
- Web interface using Streamlit
- Docker support
- Easy to deploy

---

## Tech Stack

- Python
- Scikit-learn
- Pandas
- NumPy
- Streamlit
- Docker

---

## Project Structure

```
Resume_Screening/
│
├── app.py
├── clf.pkl
├── encoder.pkl
├── tfidf.pkl
├── UpdatedResumeDataSet.csv
├── requirements.txt
├── Dockerfile
├── Resume Screening with Python.ipynb
└── README.md
```

---

## How the System Works

1. User provides resume text as input.
2. Text is cleaned and processed.
3. TF-IDF vectorizer converts text into numerical features.
4. The trained classification model predicts the job category.
5. The predicted label is decoded using the label encoder.
6. Final result is displayed on the web interface.

---

# How to Run the Project (Without Docker)

## Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Resume_Screening.git
cd Resume_Screening
```

## Step 2: Create Virtual Environment (Recommended)

```bash
python -m venv venv
```

Activate virtual environment:

Windows:
```bash
venv\Scripts\activate
```

Mac/Linux:
```bash
source venv/bin/activate
```

## Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

## Step 4: Run the Application

If you are using Streamlit:

```bash
streamlit run app.py
```

After running the command, open the URL shown in the terminal (usually):

```
http://localhost:8501
```

---

# Run Using Docker

## Step 1: Build Docker Image

```bash
docker build -t resume-screening-app .
```

## Step 2: Run Docker Container

If using Streamlit:

```bash
docker run -p 8501:8501 resume-screening-app
```

Then open:

```
http://localhost:8501
```

---

# Model Training Details

The model was trained using:

- TF-IDF Vectorization for feature extraction
- Scikit-learn classification algorithm
- Label Encoding for output classes

Training notebook file:

```
Resume Screening with Python.ipynb
```

---

# Future Improvements

- Add PDF resume upload support
- Improve text preprocessing pipeline
- Compare multiple ML algorithms
- Deploy on cloud platform (AWS / Render / Railway)
- Add authentication and user history

---

# Author

Abhishek Singh  