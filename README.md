# **Cinematic Pulse: Predicting IMDb Ratings**

<img width="996" alt="image" src="https://github.com/user-attachments/assets/572e961f-8e9c-4b8d-b815-c8bf7d4a8173">


An ML project that predicts IMDb ratings based on various cinematic features like genres, content types, and more. This tool analyzes historical movie data and provides insights to filmmakers and data enthusiasts about expected audience reception.

![Build Status](https://img.shields.io/badge/build-passing-blue)
![Python Version](https://img.shields.io/badge/python-3.8%2B-orange)
![License](https://img.shields.io/github/license/dianagudinho/Cinematic-Pulse-Gauging-IMDB-Ratings)

---

## **Features**

:white_check_mark: **Rating Prediction**: Predicts IMDb ratings using machine learning algorithms like Random Forest, Linear Regression, and Gradient Boosting.

:white_check_mark: **Database Integration**: Uses SQLite databases (`Cinematic_Pulse1.db`, `Normalised1.db`) for efficient data storage and access.

:white_check_mark: **User-friendly Interface**: Streamlit application for easy interaction and visualization of IMDb predictions.

:white_check_mark: **Comprehensive Data**: Movie metadata is used for feature engineering, with data sourced from `.csv` and `.tsv` files.

---

## **Project Files and Structure**

#### **Main Files**:
- `Final_python.ipynb`: The Jupyter notebook containing all the code for data preprocessing, model training, and evaluation.
- `Cinematic_Pulse1.db`: SQLite database used for storing and retrieving movie data.
- `Normalised1.db`: Another SQLite database used for normalized data.
- `titles.csv` & `titles.tsv`: Datasets containing movie titles and metadata for prediction.

#### **Directory Structure**:

  . Cinematic-Pulse
    ├── Final_python.ipynb
    ├── Cinematic_Pulse1.db
    ├── Normalised1.db
    ├── titles.csv
    ├── titles.tsv
    ├── requirements.txt

## **Installation Instructions**

### **Prerequisites**:
- Python 3.8 or higher
- Jupyter Notebook
- SQLite for database integration
- Dependencies listed in `requirements.txt`

### **Setup Instructions**:

1. **Clone the Repository**:
   ```
   git clone https://github.com/dianagudinho/Cinematic-Pulse-Gauging-IMDB-Ratings.git
   cd Cinematic-Pulse-Gauging-IMDB-Ratings
   ```
2. **Install Dependencies**:
   Make sure you're in the project directory, and install the required libraries:
   ```
   pip install -r requirements.txt
   ```
3. **Set Up Databases**:
   Make sure that both `Cinematic_Pulse1.db` and `Normalised1.db` are present in the project folder, as they are required for querying the movie data. No extra setup is needed.
   
4. **Open Jupyter Notebook**:
   Launch the `Final_python.ipynb` file to run the code and see step-by-step outputs.


## Running the Code  

1. **Data Preprocessing**:
> The first section of the notebook handles the extraction and cleaning of the movie data from the databases and `.csv/.tsv` files. This includes:
> Loading the movie titles and associated metadata from the provided datasets.
> Handling missing values, encoding categorical features, and normalizing data where necessary.
2. **Feature Engineering**:  
> Features such as genre, runtime, director, and other movie attributes are extracted and prepared for machine learning models.
> The processed data is stored in the `Normalised1.db` for further use.
3. **Model Training**:
> The models used for IMDb rating prediction include:

- Random Forest: Provides the best accuracy for IMDb rating prediction.
- Linear Regression: Fast and interpretable.
- Gradient Boosting: Focuses on boosting prediction accuracy by correcting errors.
  
> You can switch between models in the notebook and evaluate their performance using standard metrics like RMSE.

4. **Visualization**:
> After making predictions, the results are visualized using Seaborn and Matplotlib. 


## Technologies Used  
- Languages: `Python`
- Libraries:
  - Data Handling: `pandas`, `numpy`
  - Database : `sqlite3`
  - Visualization: `matplotlib`, `seaborn`  
  - Machine Learning: `scikit-learn`  
- Machine Learning Models:  
  - Logistic Regression  
  - Random Forest
  - Gradient Boosting
 

## License
This project is licensed under the MIT License - see the LICENSE file for details.  

## Contact

Created by <a href="mailto:diagudinho@gmail.com">Diana Minine Gudinho</a> - feel free to contact me!  
