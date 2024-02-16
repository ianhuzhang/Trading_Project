This is a summary of my project, which implements a Pairs-Trading Mean Reversion trading strategy.

Note: This is not meant to be run, but rather as a display of the code and results.

This project is based on the Mean-Reversion trading theory, that assets will typically not deviate from their long-term growth patterns. Pairs-Trading enhances this strategy, by trading the spread, or difference, between prices of two closely correlated assets. This is accomplished by taking positions in both assets, such that a return to the "expected" spread would be profitable.

This project takes publicly available asset pricing data, separates it into training and testing datasets, and optimizes certain parameters, such as the ratio of positions (Hedge Ratio) between the assets, "risk tolerance" (Bollinger Band width), or "memory" (lookback window), for optimal performance on the training datasets. The resulting strategy is then run on the testing dataset, to analyze performance.

This project was overall successful, although not as profitable as we would like. We ran the possibility of overfitting the data on the training dataset, as our grid search algorithm for finding optimal paramters was not the most sophisticated. Future improvements might be achieved by implementing better, more robust optimization algorithms.

Credits: Thanks to Ishaan Goel, as well as the Maroon Capital mentors at UChicago.
