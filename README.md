# End to End Student Performance Prediction

## Overview
The Student Performance Prediction project aims to build an end-to-end pipeline to predict students' performance in mathematics based on various features such as gender, race/ethnicity, parental level of education, lunch type, test preparation course, reading score, and writing score. This project utilizes machine learning models to provide accurate predictions, enabling educators to identify students who may need additional support.

## Table of Contents
1. [Project Structure](#project-structure)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Dataset](#dataset)
6. [Model Training](#model-training)
7. [Prediction Pipeline](#prediction-pipeline)
8. [Results](#results)
9. [Contributing](#contributing)
10. [License](#license)

## Project Structure
The project is organized as follows:
```
student-performance-prediction/
├── data/
│   ├── raw/
│   ├── processed/
├── models/
│   └── model.pkl
├── notebooks/
│   ├── EDA_STUDENT_PERFORMANCE.ipynb
│   ├── model_training.ipynb
├── scripts/
│   ├── data_preprocessing.py
│   ├── model_training.py
│   ├── predict.py
├── templates/
│   └── index.html
├── app.py
├── requirements.txt
└── README.md
```

## Features
- **Data Preprocessing**: Handling missing values, encoding categorical variables, feature scaling.
- **Model Training**: Training and evaluating machine learning models.
- **Prediction**: An end-to-end pipeline for predicting student performance.
- **Web Interface**: A user-friendly web application for inputting data and viewing predictions.

## Installation
To set up the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/student-performance-prediction.git
   cd student-performance-prediction
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. **Run the Web Application**:
   ```bash
   python app.py
   ```
   This will start a web server. Navigate to `http://127.0.0.1:5000/` in your web browser to access the application.

2. **Input the required data** through the web interface and get the predicted math score.

## Dataset
The dataset used in this project contains information about students' demographics, parental education levels, lunch types, test preparation courses, and scores in reading and writing. 

## Model Training
The model training process includes the following steps:

1. **Data Preprocessing**:
   - Handling missing values.
   - Encoding categorical features using one-hot encoding.
   - Scaling numerical features.

2. **Model Selection**:
   - Training multiple models (e.g., Linear Regression, Random Forest) and selecting the best-performing model based on evaluation metrics.

3. **Model Evaluation**:
   - Evaluating the model using metrics such as Mean Squared Error (MSE) and R-squared.

## Prediction Pipeline
The end-to-end prediction pipeline includes:

1. **Data Collection**: Collect input data from the user via the web interface.
2. **Data Preprocessing**: Preprocess the input data to match the format used during model training.
3. **Prediction**: Use the trained model to predict the student's math score.
4. **Output**: Display the predicted score on the web interface.

## Results
The results of the model are presented on the web interface, where users can see the predicted math score based on their input features.

## Contributing
Contributions are welcome! Please read the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines on how to contribute to this project.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

By following the steps and guidelines provided in this README, you can set up, run, and contribute to the Student Performance Prediction project effectively.
