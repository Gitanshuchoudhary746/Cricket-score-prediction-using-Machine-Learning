# Cricket Score Prediction Using Machine Learning

## Abstract

Cricket scoring prediction is a fusion of sports analytics and guesswork at a high level with many parameters that are not easily predictable, such as player form, pitch conditions, weather, and match dynamics. This paper explores cricket score analysis based on machine learning in comparison to statistical methods. Real-world datasets are used, considering factors like bowler economy rates, resources available during different phases of the match, and ground-specific performances. Through feature engineering, the accuracy of the prediction model was improved, while also revealing biases and limitations influencing the prediction results. This study aims to improve several areas of predictive analytics in sports, providing insights to make cricket predictions more scientific and data-driven rather than guesswork, leading to higher accuracy in sports predictions.

**Index Terms:** Random Forest Regression, XGBoost, K-Nearest Regressor, Support Vector Machine (SVM), Decision Tree Regression, Linear Regression

## Introduction

Cricket, one of the most popular sports globally, has evolved into a rich domain for data analysis and predictive modeling. Advanced analytics and machine learning techniques enable the exploration of new dimensions of the sport, including the prediction of match outcomes and player performance, with a specific focus on cricket scores. Predicting cricket scores is complex due to factors like player form, pitch conditions, weather, and opposition strength. While traditional statistical methods often fall short, machine learning offers powerful tools to address these challenges by leveraging historical match data and advanced algorithms to uncover hidden patterns. This paper provides a comprehensive analysis of cricket score prediction using machine learning, exploring methodologies, challenges, and solutions.

## Dataset and Preprocessing

* **Data Sources:** Data was collected from reliable sources such as Cricinfo and Kaggle.
* **Features:** Key attributes included:
    * Batting team, Bowling team, Venue
    * Current over, Runs conceded (Ball-by-ball), Wickets conceded (Ball-by-ball)
    * Runs in last 5 overs, Wickets in last 5 overs
    * Batsman strike rate, Batsman average runs scored
    * Bowler's average runs per over, Bowler's average wicket per match
    * Total runs scored in each match
* **Data Preprocessing:**
    * Conversion of raw, unstructured, or missing data into a structured and usable form.
    * Handling missing values by imputation or elimination, resolving duplicates, and maintaining data consistency.
    * Encoding categorical variables into numerical formats.
    * Outlier detection and removal.
    * Extensive data cleaning procedures to eliminate irrelevant rows and remove redundant variables to enhance generalization.

## Methodology

The project involved the following key steps (as illustrated in Figure 1 of the paper):
1.  **Data Collection and Integration:** Gathering ball-by-ball match data, player and team statistics, and venue details.
2.  **Data Preprocessing:** Removing irrelevant columns, handling missing values, scaling/normalizing numerical features, and encoding categorical features.
3.  **Feature Engineering:** Calculating metrics like Batter Strike Rate, Bowler Economy Rate, and custom metrics like average runs and wickets.
4.  **Model Selection and Training:**
    * Candidate Models: Random Forest Regressor, Decision Tree, SVM, XGBoost, and Linear Regression.
    * Evaluation Metrics: Train score, test score, and error metrics (Mean Squared Error, Mean Absolute Error).
    * **Selected Model:** Random Forest Regressor was chosen due to its optimal trade-off between bias and variance and its ability to handle complex, non-linear datasets effectively.
5.  **Model Evaluation:** Using Mean Absolute Error (MAE) and comparing performance across models.
6.  **Prediction and Visualization:** Predicting match scores and visualizing outcomes.

## Performance Analysis

The performance of the selected Random Forest Regressor model was evaluated as follows:

* **Train Score:** 99.05%
    * Indicates how well the model adapted to the training data.
* **Test Score:** 99.73%
    * Indicates how well the model generalizes to new, unseen data.
* **Error Metrics:**
    * **Mean Squared Error (MSE):** 4.42
        * Average of the square of the difference between predicted and actual values.
    * **Mean Absolute Error (MAE):** 55.76
        * Average of the absolute difference between predicted and actual values.
    * **Root Mean Squared Error (RMSE):** 7.46
        * Square root of MSE, providing an error metric in the same units as the target variable.

(Refer to Figure 2 for a comparative analysis of different models and Figure 3 for a scatter plot of predicted vs. actual runs using a Gradient Boosting model example from the paper.)

## Future Work

Future research directions include:
* **Real-time Data Integration:** Incorporating data from wearables, ball-tracking technologies, and environmental factors.
* **Hybrid Models:** Combining machine learning with causal analysis methods (e.g., Bayesian networks).
* **Edge Computing & AR:** Developing lightweight predictive models for onsite analytics and using augmented reality for visualization.
* **Multi-modal Data:** Integrating data from video analysis and commentary sentiment.
* **Ethical AI Frameworks:** Exploring causal reasoning and ethical considerations in predictions.

## Conclusion

The evolution of predicting cricket scores using machine learning algorithms like Random Forest regression and XGBoost has shown significant advancement. This study achieved a test accuracy of 99.73% by modeling ball-by-ball data, performance metrics, and in-game dynamism, implying that ensemble methods can capture complex patterns in cricket. Challenges include unpredictability in live matches, ethical data use considerations, and real-time adaptation needs. The future of cricket analytics lies in exploring causal reasoning, multi-modal data, and ethical AI frameworks to further enhance match strategies and fan engagement.

## Authors

* Sayed Sajid Ali (22053359@kiit.ac.in)
* Gitanshu Choudhary (22053160@kiit.ac.in)
* Gautam Kumar (22053323@kiit.ac.in)
* Anuja Kumar Acharya (anujafcs@kiit.ac.in)

School of Computer Engineering, Kalinga Institute of Industrial Technology (Deemed University), Bhubaneshwar 751024, India.

---

**Note:** This README is generated based on the content of the research paper "Cricket Score Prediction Using Machine Learning." For complete details, methodology, and discussions, please refer to the full paper.
