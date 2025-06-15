Overview:
This project is a web application built with Streamlit that allows users to upload their resumes in PDF, DOCX, or TXT formats and automatically predicts the job category they belong to. It leverages natural language processing (NLP) techniques, including text cleaning, TF-IDF vectorization, and machine learning classifiers trained on categorized resume data.

Features
Upload resumes in PDF, DOCX, or TXT formats.
Extracts and displays the resume text.
Performs text preprocessing and cleaning.
Predicts the category/job sector of the resume using a trained classifier.
Easy-to-use interface with a clean layout.
Supports multiple classifiers (KNN, SVC, Random Forest) trained on resume datasets.
Fully customizable and extendable for other models or features.
Demo
Screenshot of app <!-- Optional: Add a screenshot here -->

Installation
Requirements
Python 3.8+
Streamlit
pandas
numpy
scikit-learn
PyPDF2
python-docx
matplotlib
seaborn
Setup
Clone the repository:
bash
git clone https://github.com/yourusername/resume-category-prediction.git
cd resume-category-prediction
Create a virtual environment (optional but recommended):
bash
python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate
Install dependencies:
bash
pip install -r requirements.txt
Make sure you have the pre-trained model files (clf_Final.pkl, tfidf_Final.pkl, encoder_Final.pkl) in the project directory.
Usage
Run the Streamlit app:

bash
streamlit run app.py
Open your browser and go to the URL provided by Streamlit (usually http://localhost:8501).

Upload a resume in PDF, DOCX, or TXT format, and the app will display the extracted text and predict the category automatically.

Files and Structure
app.py: Main Streamlit app for user interaction.
Pre-trained models:
clf_Final.pkl: The trained classifier model.
tfidf_Final.pkl: The TF-IDF vectorizer.
encoder_Final.pkl: Label encoder for categories.
Additional scripts/functions for text extraction and cleaning.
Dataset (UpdatedResumeDataSet.csv) used for training.
Notebook
Model.ipynb: Jupyter notebook demonstrating data analysis, feature engineering, model training, and evaluation.
Technologies Used
Python
Streamlit
scikit-learn
pandas
NumPy
matplotlib & seaborn
PyPDF2
python-docx
Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your improvements.

License
This project is licensed under the MIT License. See the LICENSE file for details.
