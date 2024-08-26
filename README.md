# Bayesian Model for MLB Batting Average Prediction

## Project Overview
This project aims to predict second-half MLB batting averages using players' first-half performance. By employing a Bayesian hierarchical model, this project provides more accurate and interpretable predictions, accounting for basic prior knowledge about MLB hitters.

## Methodology
A Bayesian hierarchical model was developed and implemented using R, which includes player-specific random effects to capture individual performance variations, and utilization of Markov Chain Monte Carlo (MCMC) sampling as well as pure Monte Carlo simulation for posterior estimation, in comparison to a baseline frequentist approach.

More details on the model and its implementation can be found in the accompanying RMarkdown file.

## Results and Insights
Compared to a frequentist interpretation of the data, a Bayesian approach allows for much higher accuracy in predictions compared to frequentist models.

Refer to the knitted PDF report for comprehensive insights and visual illustrations.

## Installation and Usage Instructions

### Requirements
R (version 4.0 or higher)
RStudio
Packages: tidyverse, invgamma

### Installation & Usage Steps
1. Clone this repository to your local machine:
```bash
git clone [https://github.com/yourusername/mlb-batting-average-prediction.git](https://github.com/awindsheimer1/MLB_Batting_Averages_Bayesian_Model)
```
2. Open the project in RStudio, and install the required packages:
```R
install.packages(c("tidyverse", "invgamma"))
```
3. Prepare your data in a CSV file with the following columns: player_id, first_half_AB, first_half_H, position (where position is either pitcher or non-pitcher).
4. Run the script mlb_prediction_model.R to fit the model and generate predictions.
```R
source('mlb_prediction_model.R')
```
The output will include summary statistics and visualization of the posterior distributions.

## Contributions and Contact
This project was created by Andrew Windsheimer. Reach out with any comments to [awindsheimer1@gmail.com](awindsheimer1@gmail.com).

