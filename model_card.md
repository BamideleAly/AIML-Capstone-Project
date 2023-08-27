# Model Card

See the [example Google model cards](https://modelcards.withgoogle.com/model-reports) for inspiration. 

## Model Description

**Input:** Describe the inputs of your model 

The model takes as input a set of economic indicators related to exchange rate stability, real interest rate, and foreign reserves. These indicators are collected over a specific time frame (2000-2021) and represent the economic conditions of Nigeria. Economic indicators were sourced from the World Bank's official website.

**Output:** Describe the output(s) of your model
The model generates predictions for the future exchange rate stability based on the input economic indicators.

**Model Architecture:** Describe the model architecture you’ve used

The model architecture initially consists of an XGBoost regression model, an ensemble learning algorithm that combines the predictions of multiple weak learners (decision trees) to produce a robust and accurate prediction. Two neural network models were also explored for comparison, but due to challenges in data accuracy and availability, they were not adopted. Further explorations using deep learning techniques may be necessary. 

## Performance

Give a summary graph or metrics of how the model performs. Remember to include how you are measuring the performance and what data you analysed it on. 

The model's performance is evaluated using the Root Mean Squared Error (RMSE) metric, a common measure of prediction accuracy. RMSE indicates the average magnitude of the differences between predicted and actual values. The model is trained on historical economic data spanning from 2000 to 2021 and evaluated on both a validation and a test set.

Validation RMSE: The validation RMSE is approximately 36.97. This value represents the average difference between the model's predicted exchange rate stability and the actual values in the validation dataset. A lower RMSE indicates better predictive accuracy. The validation RMSE of 36.97 suggests that, on average, the model's predictions deviate from the actual values by this amount in the validation dataset.

Test RMSE (XGBoost): The test RMSE for the XGBoost model is approximately 30.38. This value reflects the average difference between the model's predicted exchange rate stability and the actual values in the test dataset. The XGBoost model demonstrates its ability to make accurate predictions on previously unseen data.

These RMSE values provide insights into the magnitude of prediction errors and how well the model generalizes to different datasets. 


## Limitations

Outline the limitations of your model.
i) Limited Scope: The model's performance is dependent on the quality and relevance of the input economic indicators. If important indicators are missing or not accurately measured, the model's predictions may be less accurate.

ii) Data Quality: The accuracy of the predictions is influenced by the accuracy and consistency of the historical economic data. Any inaccuracies or inconsistencies in the data could affect the model's performance.

iii) Extrapolation Risk: The model's predictions are based on historical data, and its ability to forecast beyond the range of historical data might be limited. Extrapolating too far into the future could introduce uncertainty and potential inaccuracies.


## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 

i) Interpretability vs. Performance: While the XGBoost model provides high predictive accuracy, its ensemble nature makes it less interpretable compared to simpler models like linear regression. The trade-off between interpretability and performance should be considered based on the specific use case.

ii) Computation Time: XGBoost involves training multiple decision trees and can be computationally intensive. While the model provides accurate predictions, the training process might require more time compared to simpler models.

## Ethical Considerations
i) Bias and Fairness: there are potential biases in the data and model predictions due to the country considered for the model. Thus, more data with more economic variables should be tested with different and more efficiency neural networks models to mitigate the bias and ensure more fairness in the model outcome. 

ii) Privacy: there are no privacy concerns as the World Bank uses data delivered by the members-countries. If the data used for training contains sensitive information, mention how privacy concerns are addressed.

## Use Cases
Describe the potential use cases for your model:

i) Decision Support: the model's predictions can be used to support decision-making in financial and economic contexts.

ii) Scenario Analysis: the model can be used to analyze different economic scenarios and their potential impact on exchange rate stability and thus to stress test a portfolio of bonds issued by the Nigerian sovereign or companies on the sell-side or buy-side. 

iii) Interpretability Techniques
If applicable, mention any techniques used to enhance the interpretability of your model:

- Feature Importance: the scores used and discussed across the Jupyter notebook provide some explanations, which indicates that the model is easy to interpret and understand by any lay person/ 
- Partial Dependence Plots: The plots showcased supports the intrepretability of the predictions.

## Future Work
Highlight areas for future improvement and development:

i) Additional Data: Discuss the potential benefits of incorporating more economic indicators, different data sources, or data from a wider time range.

ii) Advanced Techniques: Mention the possibility of exploring more advanced machine learning techniques, such as deep learning models, ensemble models, or time series models.

iii) Data Quality Improvement: Describe plans to address data quality issues, such as missing data or inaccuracies in historical economic indicators.

## Real-world Impact
Discuss the potential real-world impact of your model:
i) Policy Making: My model's predictions could influence policy decisions related to economic stability and exchange rates.

ii) Investment Strategy: My model's predictions could be used by investors to inform their currency-related investment strategies.

iii) Economic History: My model could be used for further research in economic and monetary history as my initial plan was. 







