# vortextech-aimlweek2:
Week 2 task for the VortexTech AI & ML Internship: building a classification model with scikit-learn.

## What this is

I reused my Week 1 dataset (the Netflix titles dataset from Kaggle). It doesn't come with a ready-made yes/no column, so I picked my own binary target: predicting whether a title is a **Movie** or a **TV Show** from its release year, content rating, and country.

I deliberately left out the `duration` and `listed_in` (genre) columns even though they're strong predictors, because they leak the answer directly (e.g. duration says "min" for movies and "Seasons" for TV shows, and some genre tags are literally named "TV Dramas").

## Models used

- Logistic Regression
- Decision Tree Classifier

Both were evaluated with accuracy, precision, recall, and F1-score. Full writeup and results are in the notebook.

## How to run it

1. Clone this repo
2. Install dependencies: `pip install pandas scikit-learn jupyter`
3. Make sure `netflix_titles.csv` is in the same folder as the notebook
4. Open `week2_classification.ipynb` in Jupyter and run all cells

## Files

- `week2_classification.ipynb` — the notebook with all code, results, and analysis
- `netflix_titles.csv` — the dataset (from Kaggle)
- `README.md` — this file
