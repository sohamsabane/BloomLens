
# BloomLens – NLP & Generative AI Question Intelligence Platform

## Project Overview

BloomLens is an AI-powered educational question analysis platform developed using Natural Language Processing (NLP), Machine Learning, and Generative AI.

The application analyzes educational questions based on Bloom's Taxonomy, performs text preprocessing, sentiment analysis, information extraction, topic modelling, multilingual translation, and generates questions using Large Language Models (LLMs).

BloomLens helps educators analyze cognitive learning levels and create educational assessments.

## Team Members

| Name | PRN |
|------|-----|
| Soham Sabane | 202401110070 |
| Saumyajeet Sing Bhati | 202401110065 |

## Key Features

### 1. Text Extraction and Preprocessing
- Extract questions from text and PDF documents.
- Clean and normalize unstructured text.
- Tokenization and text preprocessing.
- TF-IDF vectorization.
- Bloom's Taxonomy classification using rule-based and SVM approaches.

### 2. Sentiment Analysis and Information Extraction
- Sentiment analysis using VADER.
- Positive, negative, and neutral classification.
- Extraction of Bloom's Taxonomy action verbs.
- Extraction of important concepts.
- Visualization of sentiment distribution.

### 3. Topic Modelling and Multilingual NLP
- Topic modelling using Latent Dirichlet Allocation (LDA).
- Identification of common topics in educational questions.
- English-to-Hindi translation.
- Groq API-based cloud translation.
- Local translation using Helsinki-NLP models.

### 4. Generative AI and LLM Integration
- Integration with Groq API.
- Question generation based on Bloom's Taxonomy.
- Zero-shot and few-shot prompting.
- Step-by-step prompting.
- Automatic Bloom-level classification.
- Question rewriting to higher cognitive levels.

## Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Backend programming |
| Streamlit | Web application interface |
| Pandas | Data processing |
| Scikit-learn | TF-IDF and SVM classification |
| NLTK | Natural language preprocessing |
| spaCy | NLP processing |
| VADER | Sentiment analysis |
| Gensim | LDA topic modelling |
| Transformers | Pretrained NLP models |
| Groq API | LLM integration |
| Matplotlib | Data visualization |

## Project Structure

```text
Bloomlens-main/
├── app.py
├── requirements.txt
├── README.md
├── .env.example
├── .gitignore
├── src/
│   ├── preprocess.py
│   ├── classify.py
│   ├── sentiment_tools.py
│   ├── topics_multilingual.py
│   └── llm_tools.py
├── data/
├── reports/
└── scripts/
```

## Installation and Setup

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/BloomLens-NLP-Project.git
cd BloomLens-NLP-Project
```

Replace `YOUR_USERNAME` with your GitHub username.

### Step 2: Create a Virtual Environment

Python 3.11 is recommended.

```bash
python -m venv .venv
```

Activate on Windows:

```powershell
.\.venv\Scripts\Activate
```

Activate on macOS/Linux:

```bash
source .venv/bin/activate
```

### Step 3: Install Dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Step 4: Configure the Groq API

Create a `.env` file in the project directory using `.env.example` as a template.

```env
GROQ_API_KEY=your_groq_api_key_here
LLM_PROVIDER=groq
DEMO_MODE=false
```

Obtain an API key from:

https://console.groq.com/keys

**Security:** Never upload your `.env` file or API key to GitHub.

### Step 5: Run the Application

```bash
python -m streamlit run app.py
```

Open:

http://localhost:8501

## Deploy on Streamlit Community Cloud

1. Upload the project to a GitHub repository.
2. Visit https://share.streamlit.io.
3. Sign in using GitHub.
4. Create a new Streamlit application.
5. Select your repository and main branch.
6. Set the entry-point file to `app.py`.
7. Select Python 3.11 if available.
8. Configure the Groq API key securely in Streamlit Secrets.
9. Deploy the application.

Example Streamlit Secrets configuration:

```toml
GROQ_API_KEY = "your_groq_api_key_here"
LLM_PROVIDER = "groq"
DEMO_MODE = false
```

The application must be configured to read Streamlit Secrets when deployed.

## Bloom's Taxonomy Levels

| Level | Cognitive Skill | Example |
|-------|-----------------|---------|
| Remember | Recall information | Define artificial intelligence. |
| Understand | Explain concepts | Explain machine learning. |
| Apply | Apply knowledge | Apply binary search. |
| Analyze | Examine relationships | Analyze sorting algorithms. |
| Evaluate | Make judgments | Evaluate model performance. |
| Create | Develop new solutions | Design an AI chatbot. |

## System Workflow

1. User enters questions or uploads a document.
2. The system extracts and preprocesses text.
3. TF-IDF converts text into numerical features.
4. Bloom-level classifiers analyze the questions.
5. VADER performs sentiment analysis.
6. Information extraction identifies verbs and concepts.
7. LDA discovers topics across questions.
8. Multilingual NLP translates questions.
9. The Groq-powered LLM generates or rewrites questions.
10. Streamlit displays the results.

## Applications

- Educational question paper analysis
- Automated question classification
- Bloom's Taxonomy-based assessment design
- AI-assisted question generation
- Multilingual educational support
- NLP research and demonstrations

## Limitations

- Rule-based classification depends on predefined action verbs.
- SVM performance depends on training data quality.
- Sentiment analysis does not directly measure cognitive difficulty.
- Topic modelling requires sufficient text data.
- LLM outputs may require human verification.
- Cloud-based features require an internet connection and a valid API key.
- Large NLP models may require additional memory.

## Future Scope

- Support for additional Indian languages.
- Improved transformer-based Bloom classification.
- Automatic question paper generation.
- More comprehensive model evaluation.
- Teacher feedback and question validation.
- Integration with Learning Management Systems.

## Conclusion

BloomLens combines traditional NLP, Machine Learning, and Generative AI in a single educational application.

It demonstrates text extraction, preprocessing, classification, sentiment analysis, information extraction, topic modelling, multilingual processing, prompt engineering, and cloud-based LLM integration.

The project aims to support educators in creating and analyzing questions according to Bloom's Taxonomy.

## Developed By

**Soham Sabane**  
PRN: 202401110070

**Saumyajeet Sing Bhati**  
PRN: 202401110065

---

**BloomLens – Making Educational Question Analysis Smarter with NLP and Generative AI.**
