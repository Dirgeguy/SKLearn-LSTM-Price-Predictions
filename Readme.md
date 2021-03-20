# LSTM Stock Predictor


In this repo, we compare the effectiveness of the same base Long Short-Term Memory Recurrent Nerual Network trained on different input features to predict the price of Bitcoin. 

We have two features to train our models with, a 10 day lag window for one, and a 10 day window of Bitcoin fear and greed index values.

Both models were built with a 70-30 split for training and testing, and scaled using a MinMaxScaler. The eventual comparison between predicted and actual prices was the metric for judgement between the models.

As seen at the terminus of the respective notebooks, the Fear and Greed Index (FNG) seemed to be the weaker of the two in predictive power, while the Closing Prices produced the strongest results. Both models had the same construction, leading my observations to conclude that despite providing useful high-level analytical information, the Fear and Greed Index is not a strong enough solo feature for predictive purposes. This leads me to believe the FNG index should only be used as an additional feature. The closing price did fair better, and although missing exact prices, it does reflect the momentum well.
