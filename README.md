# Football Analysis and Prediction

## Overview
This project provides an in-depth analysis and prediction of football (soccer) matches using data and machine learning. The analysis focuses on three key areas:

1. **Goalscoring Trends Over Time:** Investigates the average goals per match across different eras, competitions, and teams.
2. **Penalty Shootout Analysis:** Analyzes penalty shootout data to identify patterns and assess the impact of shooting order on the outcome.
3. **Match Outcome Prediction:** Predicts the outcome of a football match using a machine learning model (XGBoost), based on previous team performance data.

All these analyses and predictions are contained within a single Jupyter notebook, making it easy to run and explore.

## Project Structure
The repository contains the following key components:

Football-Analysis-and-Prediction/
│
├── data/
│   ├── results.csv           # Match results with scores and tournament info
│   ├── goalscorers.csv       # (Optional) Dataset with goalscorers info
│   └── shootouts.csv         # Information on penalty shootouts
│
├── National Teams.ipynb      # Jupyter notebook containing all the analysis and prediction code
├── requirements.txt          # List of required Python libraries
├── README.md                 # Project documentation
└── .gitignore                # Git ignore file to exclude unnecessary files



## Setup Instructions

### Prerequisites
Ensure you have the following installed on your machine:
- Python 3.x
- Jupyter Notebook or JupyterLab for running the `.ipynb` notebook
- Required Python libraries (see `requirements.txt`)

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/MohamedGuedira/Football-Analysis-and-Prediction.git
    ```

2. Navigate into the project directory:
    ```bash
    cd Football-Analysis-and-Prediction
    ```

3. Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    ```

### Running the Notebook
1. Open Jupyter Notebook or JupyterLab in your terminal:
    ```bash
    jupyter notebook
    ```

2. Open the `National Teams.ipynb` notebook:
    - In the Jupyter interface, navigate to `National Teams.ipynb` and open it.

3. Run each cell to perform the following analyses:
    - **Cell 1:** Analyzes the average goals per match across different eras and competitions.
    - **Cell 2:** Examines penalty shootout patterns and the impact of the shooting order.
    - **Cell 3:** Predicts the outcome of a football match using the XGBoost model based on previous data.

### Example Usage
In the `National Teams.ipynb` notebook, you can run the cells sequentially to perform all three analyses. For instance, to predict a match outcome using the XGBoost model, modify the input teams in **Cell 3** like this:

```python
team1 = "Brazil"
team2 = "Argentina"
predict_match_outcome(team1, team2, model, le_team)
