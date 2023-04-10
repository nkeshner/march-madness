# march-madness

## Overview
This project aims to use NCAA game statistics to predict winners in the NCAA men's and women's March Madness tournament. It uses game data from [Kaggle](https://www.kaggle.com/competitions/march-machine-learning-mania-2023) to generate continuous season-long averages for each team and calculate Elo. This data is used to train a model which predicts game scores for each team (given team and opponent stats). Once the model is trained and predictions for each possible men's and women's tournament matchup are made, the tournament is simulated according to the predictions. 

## Installation
1. Clone this repository to your local machine.
```bash
git clone https://github.com/your-username/your-repo-name.git
```
2. Install the required packages using pip (pandas, numpy, scikit-sklearn, scipy, xgboost, graphviz, kaggle). We recommend creating a new virtual environment for this project.
```bash
pip install kaggle
```
3. To use the kaggle API, you need to configure your Kaggle credentials. Follow the instructions in the [Kaggle API documentation](https://github.com/Kaggle/kaggle-api#api-credentials) to set up your API credentials. Once you have your credentials, you can download the Kaggle dataset by running the following command:
```bash
kaggle datasets download -d your-dataset-name
```

## Usage
1. Download the March Madness dataset from [Kaggle](https://www.kaggle.com/competitions/march-machine-learning-mania-2023) and extract the files to the data directory in this repository.

2. Run the `March Madness Predictor.ipynb` notebook to train a model and make game predictions for the upcoming March Madness tournament.

3. After running the `March Madness Predictor.ipynb` notebook, you should have a submission.csv file in the data directory that contains your predictions for the tournament. You can use this file as input for the `Bracket and Odds Simulation.ipynb` notebook.

4. Run the `Bracket and Odds Simulation.ipynb` notebook to simulate a tournament and produce odds for each team using your predictions from the previous step.

