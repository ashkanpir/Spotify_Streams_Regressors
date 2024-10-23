# Spotify Streams Regressors

This repository contains the code and analysis for predicting Spotify song stream counts using various regression models. The project applies machine learning techniques to model and predict the number of streams based on a variety of song and playlist features.

## Project Overview

The primary objective of this project is to build regression models that accurately predict the number of streams a song will receive on Spotify. The dataset includes features such as playlist appearances, audio attributes (danceability, speechiness, etc.), and chart rankings from platforms like Spotify, Apple, and Deezer.

## Models Used

Several regression models were tested and fine-tuned, including:

- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**
- **ElasticNet**
- **Random Forest**
- **Gradient Boosting**
- **XGBoost**
- **LightGBM**
- **AdaBoost**
- **KNeighbors**
- **Decision Trees**

The best-performing models were fine-tuned using cross-validation and hyperparameter optimization, and feature engineering was applied to improve accuracy.

## Key Results

- **Best Models**: LightGBM and XGBoost consistently achieved the best performance, with R² values around 0.80 and RMSE values close to 218 million.
- **Feature Engineering**: Interaction terms and careful feature selection helped to enhance model performance.
- **Stacking**: A stacked model combining the predictions of LightGBM, Gradient Boosting, and XGBoost provided comparable results to the best individual models.

## Features Used

The following features were identified as most relevant for predicting stream counts:
- Playlist appearances on Spotify, Apple, and Deezer
- Chart positions on Spotify, Apple, Deezer, and Shazam
- Audio attributes such as danceability, speechiness, and artist count

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
