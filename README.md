# Medicine Recommendation System

## Overview

The Medicine Recommendation System is a machine learning-based web
application that predicts diseases from user-input symptoms and suggests
suitable medicines, precautions, workouts, and diets.

## Project Structure

    Medicine-Recommendation-System/
    │
    ├── dataset/
    │   ├── description.csv
    │   ├── diets.csv
    │   ├── medications.csv
    │   ├── precautions_df.csv
    │   ├── Symptom-severity.csv
    │   ├── symtoms_df.csv
    │   ├── Training.csv
    │   └── workout_df.csv
    │
    ├── model/
    │   ├── rf.pkl
    │   └── svc.pkl
    │
    ├── static/
    │   └── heal.jpg
    │
    ├── templates/
    │   ├── index.html
    │   └── result.html
    │
    ├── main.py
    └── README.md

## Step-by-Step Implementation

### Step 1: Data Collection and Preprocessing

-   Use the CSV files in the `dataset` folder.
-   Datasets contain symptoms, diseases, medications, precautions, etc.
-   Clean data using pandas, encode symptoms as numeric features.

### Step 2: Model Training

-   Load `Training.csv`.
-   Use classifiers like RandomForest and SVC.
-   Train and save them as `rf.pkl` and `svc.pkl`.

### Step 3: Backend (Flask)

-   `main.py` handles the backend logic.
-   It loads the trained models and dataset files.
-   Accepts user symptoms input and predicts disease.
-   Displays medicine, precaution, diet, and workout suggestions.

### Step 4: Frontend (HTML/CSS/JS)

-   Located in `templates` and `static` folders.
-   The home page takes symptom input or speech recognition.
-   Displays predicted results in styled boxes.

### Step 5: Running the App

1.  Open terminal in project folder.

2.  Run:

    ``` bash
    python main.py
    ```

3.  Open browser and visit:

    ``` bash
    http://127.0.0.1:5000
    ```

### Step 6: Model Files

-   `rf.pkl` -- Random Forest Model
-   `svc.pkl` -- Support Vector Classifier

### Step 7: Dependencies

Install required packages:

``` bash
pip install pandas numpy scikit-learn flask
```

### Step 8: Features

-   Predict disease using symptoms.
-   Speech recognition input.
-   Recommends medicines, precautions, diet, and workout plans.
-   Simple UI with Flask and HTML templates.

### Step 9: Future Enhancements

-   Add deep learning model.
-   Integrate real-time database.
-   Enhance UI/UX with React or Angular.
-   Add authentication and patient record system.

## Author

Developed by Krishna Meena
