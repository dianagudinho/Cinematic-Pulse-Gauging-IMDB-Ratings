# **Cinematic Pulse: Predicting IMDb Ratings** :movie_camera:

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

## :open_file_folder: **Project Files and Structure**

#### 1. **`Final_python.ipynb`**:
- This is the Jupyter Notebook that contains the primary codebase for the project.
- It handles tasks such as:
  - Reading data from CSV/TSV files.
  - Loading and querying SQLite databases (`Cinematic_Pulse1.db`, `Normalised1.db`).
  - Data preprocessing, such as feature engineering and handling missing data.
  - Training machine learning models such as Linear Regression, Random Forest, and Gradient Boosting.
  - Visualizing the results using `matplotlib` and `seaborn`.

#### 2. **`Cinematic_Pulse1.db`**:
- This SQLite database contains raw movie data extracted from the `titles.tsv` file.
- It serves as the main data source for querying movie-related information such as IMDb ID, scores, runtime, etc.

#### 3. **`Normalised1.db`**:
- A normalized version of the movie data stored in `Cinematic_Pulse1.db`.
- This database contains cleaned and processed data for use in machine learning tasks.
- It includes tables like `Media`, `IMDb`, `Season`, `Genre`, and `GenreSplit` that are used for model training and querying.

#### 4. **`titles.csv`**:
- A CSV file containing movie metadata, including titles, types (e.g., movie or TV show), release year, runtime, genres, and IMDb scores.
- Used as an input source for extracting features for the project.

#### 5. **`titles.tsv`**:
- A TSV (Tab-Separated Values) file similar to `titles.csv`, containing metadata about movies.
- It may include different formatting or additional columns compared to the CSV version.

#### 6. **`requirements.txt`**:
- This file contains a list of all the Python libraries required to run the project.


### **Directory Structure**:
```
  . Cinematic-Pulse-Gauging-IMDB-Ratings
    ├── Final_python.ipynb
    ├── Cinematic_Pulse1.db
    ├── Normalised1.db
    ├── titles.csv
    ├── titles.tsv
    └── requirements.txt
```



## :gear: **Installation Instructions**

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


## :arrows_clockwise: Running the Code - What will you find?

1. **Data Preprocessing**:
> The first section of the notebook handles the extraction and cleaning of the movie data from the databases and `.tsv` files. This includes:
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


## :technologist: Technologies Used  
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
