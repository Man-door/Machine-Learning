# Machine Learning Mandor Recommendation System

This repository contains a machine learning project for building a recommendation system to recommend Mandor (workers) based on a variety of input features. The project uses deep learning techniques, particularly regression models, for the recommendation task.

## Project Structure

### 1. **Dataset Folder**
- **`sejasa_raw.csv`**: Raw dataset scraped from the website `sejasa.co.id`, containing unprocessed data.
- **`data_cleaned.csv`**: Cleaned dataset after data wrangling, with missing values and inconsistencies addressed.
- **`data_final.csv`**: Final dataset used for training the machine learning model.

### 2. **Model Folder**
- **`ML_model.h5`**: The trained model saved in H5 format.
- **`ML_model.tflite`**: The TensorFlow Lite version of the model for efficient deployment on mobile and embedded devices.

### 3. **Notebooks**
- **`dataset.ipynb`**: Jupyter notebook containing the process of cleaning the dataset (`data_cleaned.csv`).
- **`model_final.ipynb`**: Jupyter notebook for creating the final deep learning model (recommendation system using regression).

## Project Details

### 1. **Data Cleaning**
The `dataset.ipynb` file demonstrates the entire data wrangling process, including:
- Handling missing values in the dataset.
- Normalizing numerical features like `pengalaman`, `rating`, and `portofolio`.

### 2. **Model Creation**
The `model_final.ipynb` file contains the code for building a deep learning model:
- The model uses multiple inputs such as service type, location, user ratings, work experience, and portfolio.
- The model is trained using regression to predict relevance scores for Mandor recommendations.
- The final model is saved as both `.h5` and `.tflite` for easy deployment and inference.

## Installation
You can install them using pip:

```bash
pip install -r requirements.txt
