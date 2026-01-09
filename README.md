# Air-Ticketing-Forecasting-Using-RNN

This notebook, air_ticket_forecasting_using_rnn.ipynb, demonstrates the application of Recurrent Neural Networks (RNNs) for probabilistic time-series forecasting. Using the Darts library, it specifically explores how deep learning models can capture and predict uncertainty in fluctuating data, such as airline passenger traffic.

Key Features
Probabilistic Forecasting: Unlike deterministic models that provide a single point estimate, this implementation uses Monte Carlo sampling and Gaussian Likelihood to generate a range of potential outcomes, accounting for risk and variance.

Advanced RNN Architectures: Implements a Long Short-Term Memory (LSTM) network to handle long-term dependencies in the data.

Covariate Integration: Demonstrates the use of Future Covariates—external signals (like noise modulators or calendar events) known in advance—to improve the model's understanding of when volatility is likely to increase.

Synthetic & Real-World Analysis: Uses both the classic AirPassengers dataset and synthetic non-stationary noise series to stress-test the model’s ability to map oscillating uncertainty.

Technical Workflow
Preprocessing: Data scaling and transformation using the Darts Scaler.

Modeling: Configuring an RNNModel with LSTM cells, dropout for regularization, and likelihood parameters for probability distribution.

Validation: Splitting series into training/validation sets and assessing performance via the R2 Score (achieving ~0.89) and visual density plots.

Visualization: Comparative plotting of actual vs. predicted values with shaded uncertainty intervals.
