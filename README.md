# Resume ATS Score Calculator  

## 📌 Project Overview  
This project is a **Flask-based web application** that calculates the **ATS (Applicant Tracking System) score** of a resume based on a given job description. It uses **NLP-based sentence embeddings** to measure the similarity between a resume and a job posting.  

## 🚀 Features  
- Upload a **PDF resume**.  
- Enter a **job description**.  
- Calculate the **similarity score** between the resume and job description.  
- **Web-based UI** for easy interaction.  

## 🛠️ Technologies Used  
- **Flask** (Web Framework)  
- **Sentence Transformers** (NLP Model for Similarity)  
- **PyMuPDF (fitz)** (Extract Text from PDF)  
- **Scikit-Learn** (Cosine Similarity Calculation)  

## 💂️️ Project Structure  
```
resume-score/
│── uploads/                # Folder to store uploaded resumes
│── templates/
│   ├── index.html          # HTML template for UI
│── app.py                  # Main Flask application
│── pyproject.toml          # Project dependencies (Poetry)
│── poetry.lock             # Package lock file
│── README.md               # Project documentation
```

## ⚙️ Installation  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/your-username/resume-score.git
cd resume-score
```

### 2️⃣ Set up a Virtual Environment  
```bash
python -m venv venv
source venv/bin/activate   # On macOS/Linux
venv\Scripts\activate      # On Windows
```

### 3️⃣ Install Dependencies  
Using **Poetry** (recommended):
```bash
poetry install
```
Or using **pip**:
```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Application  
```bash
python app.py
```
The app will run on **http://127.0.0.1:5000/**.  

## 📝 Usage  
1. Open the web application.  
2. Upload a **PDF resume**.  
3. Enter the **job description**.  
4. Click "Submit" to get the **ATS match score**.  

## 🤖 How It Works  
1. **Extracts text** from the uploaded PDF resume.  
2. **Encodes** both the resume text and job description using **Sentence Transformers**.  
3. **Computes similarity** using **cosine similarity**.  
4. Returns a **percentage score**, showing how well the resume matches the job description.  

## 🐜 License  
This project is **open-source** and free to use.
