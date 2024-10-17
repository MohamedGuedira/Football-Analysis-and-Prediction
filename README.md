# Football Analysis and Prediction

## Overview
This project provides a comprehensive analysis of football (soccer) match data, including:

- **Goalscoring trends over time:** Analyze the average goals per match for each era, competition, and team.
- **Impact of rule changes on goal scoring:** Explore the impact of rule changes, such as the introduction of penalty shootouts, on goal-scoring trends.
- **Penalty shootout analysis:** Study the patterns of penalty shootouts, identifying common winners and whether the first shooter has an advantage.
- **Predict match outcomes using XGBoost:** Machine learning model to predict the outcome of a match based on teams and previous data.

## Project Structure
The repository is structured as follows:

football-analysis/ 
│
├── data/ 
│ ├── results.csv # Contains match results with scores and tournament info 
│ ├── goalscorers.csv # (Optional) Dataset with goalscorers info 
│ └── shootouts.csv # Contains information on penalty shootouts 
│ 
├── analysis/ 
│ ├── goals_analysis.py # Code for analyzing goals trends, rule changes, and goal margins 
│ ├── shootouts_analysis.py # Code for analyzing penalty shootouts 
│ └── prediction.py # Code for predicting match outcomes using XGBoost 
│ 
├── requirements.txt # List of required Python libraries
├── README.md # Project documentation 


## Setup Instructions

### Prerequisites
Ensure you have the following installed on your machine:
- Python 3.x
- Required Python libraries (see `requirements.txt`)

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/MohamedGuedira/Football-Analysis-and-Prediction.git
    ```

2. Navigate into the project directory:
    ```bash
    cd football-analysis
    ```

3. Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    ```

### Running the Analysis
1. **Goals Analysis:**
    - To analyze goalscoring trends, rule changes, and goal margins, run the `goals_analysis.py` script:
      ```bash
      python analysis/goals_analysis.py
      ```

2. **Penalty Shootout Analysis:**
    - To study shootouts and identify common winners, run the `shootouts_analysis.py` script:
      ```bash
      python analysis/shootouts_analysis.py
      ```

3. **Predict Match Outcomes:**
    - To use machine learning to predict match outcomes, run the `prediction.py` script:
      ```bash
      python analysis/prediction.py
      ```

### Example Usage
After setting up the environment, you can predict the outcome of a match using the XGBoost model. For example, to predict the outcome of a match between Brazil and Argentina, you can run:

```python
team1 = "Brazil"
team2 = "Argentina"
predict_match_outcome(team1, team2, model, le_team)

This will generate a bar chart showing the predicted probabilities for each possible outcome (Home Win, Draw, Away Win).
