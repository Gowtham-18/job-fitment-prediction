# Job-Fitment-Prediction
A pipeline to predict job “fit” for candidates based on job‐description text and candidate profiles.  

It supports:

- **Content-Based Filtering** via TF-IDF + cosine similarity  
- **Synthetic Label Generation** for `fit`/`no-fit`  
- **Supervised Classification** (Logistic Regression, Random Forest)  
- **Unsupervised Clustering** (K-Means + PCA visualization)

## Install dependencies:

pip install -r requirements.txt

## Dataset:
- Download the dataset
- Generate a Kaggle API token (kaggle.json) from your Kaggle account.
- Place kaggle.json in this folder or in ~/.kaggle/.
- In the notebook you’ll run:
  !kaggle datasets download -d ravindrasinghrana/job-description-dataset -p ./data
  !unzip -q ./data/job-description-dataset.zip -d ./data

Open the notebook
Run cells in order
Enter your own candidate profile in the final cell to see top-N recommendations, fit‐flags, and cluster assignment.

## Data Source:
Kaggle Job Description Dataset by Ravindra Singh Rane:
https://www.kaggle.com/datasets/ravindrasinghrana/job-description-dataset
