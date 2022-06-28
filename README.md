# Project_2_recommender

The project is carried out as a part of the Recommendation Systems at the University of Adam Mickiewicz in Poznań. \
Based on materials from the repository https://github.com/PiotrZiolo/recommender-systems-class \
Author: Maciej Barabasz 

## Goal

The aim of the project are:
- preparing dataset of hotel recommendations for neural network recommender,
- selecting best features for the model,
- preparing neural network model
- tuning parameters
- finding the best HR@10 in the final evaluation for recommended hotels for users,
- comparing the results against Amazon recommender and Netflix recommender.

## Scores
![2022-06-28_21h37_17](https://user-images.githubusercontent.com/25958431/176272599-51309702-63e9-402d-b546-a26098d68390.png)

## Best Parameters 
```python
n_neg_per_pos=18, 
epochs=20, 
batch_size=400, 
drop_out=0.7000000000000001, 
learning_rate=0.0005, 
neurons=300
```

## Requirements
- Anaconda 3.8
- Git bash

## Instalallation
```bash
pip install pandas
pip install numpy
pip install matplotlib
pip install seaborn
pip install torch
pip install livelossplot
```

## Starting up project locally
- Create a folder on your local machine where you want stash this project. Open this folder and right click in it. From scroll menu select Git Bash here. After application opens insert this line:
```git
git clone https://github.com/Maciasty15/Project_2_recommender.git
```
- Prepare your conda environment (instructions given for Windows, but it should be similar on other systems):

    Open Anaconda Prompt as administrator.

    Make sure you're in the repository main folder. Run the following command:
```bash
conda env create --name rs-proj-env -f environment.yml
```
- Activate just created environment with the following command:
```bash
 conda activate rs-proj-env	
```
- Then type:
```
 jupyter notebook
```
A new tab with Jupyter Notebook should open in your browser.

In Jupyter Notebook open projec_2_data_preparation.ipynb.

In tab menu select "Cell" and hit "Run all". Wait for the process to finish and close project_2_data_preparation.ipynb

In Jupyter Notebook open project_2_recommender_and_evaluation.ipynb

In tab menu select "Cell" and hit "Run all". Wait for the process to finish.

NOTE: project is not finished so some errors will be displayed
