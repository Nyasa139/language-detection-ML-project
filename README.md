# Language Detection System

A machine learning project that detects the language of a given text input.  
The system takes a sentence or paragraph as input and predicts the language using a trained ML model.

## Languages Supported

This model can detect the following languages:

1. English
2. Hindi
3. French
4. Spanish
5. Portugeese
6. Italian
7. Russian
8. Sweedish
9. Malayalam
10. Dutch
11. Arabic
12. Turkish
13. German
14. Tamil
15. Danish
16. Kannada
17. Greek
18. Bengali

> Note: The dataset labels contain spellings like `Portugeese` and `Sweedish`, so the model may output those exact names.

## Project Workflow

### 1. Dataset Collection

The project uses a language detection dataset containing text samples from multiple languages.  
Additional Hindi, Malayalam, and Bengali sentences were added to improve prediction performance for Indian languages.

### 2. Data Exploration

The dataset was checked for:

- Number of rows and columns
- Missing values
- Empty text entries
- Language distribution

### 3. Data Cleaning and Preprocessing

The text data was cleaned using preprocessing steps such as:

- Converting text to lowercase
- Removing punctuation
- Removing numbers
- Removing extra spaces
- Keeping Unicode characters so languages like Hindi, Bengali, Malayalam, Tamil, Kannada, Greek, Arabic, and Russian are preserved

### 4. Model Training

The cleaned text data was used to train a machine learning model for language classification.

The model was trained using:

- Text vectorization
- Machine learning classification
- Train-test split for evaluation

### 5. Model Evaluation

After training, the model was tested on unseen data.  
The accuracy score was checked to understand how well the model performs.

### 6. Model Saving

The trained model was saved using `joblib` so it can be reused without training again.

### 7. Frontend

A simple frontend can be created using Streamlit where the user enters text and the system predicts the language.

## How to Run the Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/Nyasa139/language-detection-system.git
cd language-detection-system
