# GA TECH BOOTCAMP FINAL PROJECT (MACHINE LEARNING) 
# Predicting Box Office Revenue
For our machine learning project, we will be predicting, analyzing, and visualizing movie box office revenue totals based on a number of different attributes. 
## Dataset Source:
    https://www.kaggle.com/  
    tmdb-box-office-prediction/data 
    AWS Loading: s3://boxofficepredictions/Merged_Frames.csv
    
    https://developers.themoviedb.org/3

# Cleaning and preprocessing
We will then clean and preprocess the data and apply machine learning models to predict and visualize the accuracy of the model and will present our findings through a public tableau dashboard.

Machine Learning Library: Scikit-Learn using supervised learning 

We will do this by using Pythons Pandas, matplotlib, and Tableau 

# Dataset Features: 
Collection,
Budget,
Genre,
Original Language,
Spoken Language
Runtime,
Production Company,
Production County,
Release Date

# Target:
Revenue


# Deployment
Deploy HTML using app.py via FLASK

# Navigating our Folders and Final Conclusion
All of the machine learning preparation and model creation we carried out in the Notebook Folder.
- The TMDB_API_PULL.ipynb contains our api pull code where we merged the data frames, we then exported the merged frame to place in our AWS Bucket. 
- The Processing_and_Models.ipynb is the notebook that contains all data preprocessing (including normalization and hyperparameter tunining) as well as model creation. 
    - The model we eneded up deciding on was RandomForestRegressor. After Normalizing the data, this model produced a 
# Training Score of 0.95 and a Testing Score of 0.73 
   - To counteract the present overfitting issue we ran a randomized grid search to produce the best parameters
   - After adding the parameters, we ran the model again and got 
# Training Score: 0.6422128894515788 and a Testing Score: 0.6536014008701967
- The Creating_Trees.ipynb contains the code used to create our Random Tree Regressor Graphics. 

All of the .py, .html, and .css files are used to deploy a site (on a local host) to display our findings 
