# Used_Car_Price_Prediction_UA

Jupyter Notebook project for training a fully-connected Neural network for estimating the value of used cars according to their attributes. 

#### Python frameworks used: 
- `Keras` for machine learning
- `Pandas` for data exploration
- `Matplotlib` and `Seaborn` for data visualization
- `Sklearn` for data preprocessing and performance evaluation.
- `FastML` for splitting into train, val and test sets

#### Data preprocessing techniques applied:
- `Standard scaling` for numerical features
- `One-hot` encoding for categorical features

#### Neural network architecture:
- Dense layer of size 256, activation: `ReLU`, input size: 243 (after data transformation)
- Dropout layer, `dropout_rate`: 0.15 
- Dense layer of size 128, activation `ReLU`
- Dropout layer, `dropout_rate`: 0.1
- Dense layer of size 64, activation `ReLU`
- Dropout layer, `dropout_rate`: 0.05
- Dense layer of size 32, activation `ReLU`
- Dropout layer, `dropout_rate`: 0.02
- Dense layer of size 1, activation `Linear`

`Loss`: Mean Squared Error, `batch_size`: 256, `epochs`: 225, `optimizer`: Adam.

#### Neural network performance on the testing set:
- `Mean absolute error (MAE)`: 960 ($)
- `Coefficient of determination (R2)`: 0.968
