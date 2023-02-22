# Predicting the Net Hourly Electrical Energy Output of a Combined Cycle Power Plant

## Multiple Linear Regression in Python using Scikit-Learn
<br>

## 📝 Data Set Information:
The dataset contains 9568 data points collected from a Combined Cycle Power Plant over 6 years (2006 - 2011), when the power plant was set to work with full load. Features consist of hourly average ambient variables Temperature (T), Ambient Pressure (AP), Relative Humidity (RH) and Exhaust Vacuum (V) to predict the net hourly electrical energy output (EP) of the plant.<br>
<br>
A combined cycle power plant (CCPP) is composed of gas turbines (GT), steam turbines (ST) and heat recovery steam generators. In a CCPP, the electricity is generated by gas and steam turbines, which are combined in one cycle, and is transferred from one turbine to another. While the Vacuum is collected from and has effect on the Steam Turbine, the other three of the ambient variables affect the GT performance.<br>
<br>
70% of the data is used for training and 30% is used for testing. Predictions are made for the net hourly electrical energy output (EP) of the plant using the other variables as features. Each coefficient represents the amount of change in the response variable for one unit of change in the predictor variable while holding the other predictors in the model constant. For example, a 1 unit increase in temperature is associated with a 0.45 unit increase in net hourly electrical energy output. From our predicted values, a value such as 432.75 means that the net hourly electrical energy output is 432.75 MW.<br>
<br>

The data set is taken from this [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Combined+Cycle+Power+Plant).
<br>
<br>

## 🛠 Dependencies
* Python 3.x
* Numpy
* Pandas
* Matplotlib
* Scikit-Learn
<br>
<br>

## ⬇️ Installation
1. Clone the repository
```bash
git clone https://github.com/nickmezacapa/multiple-linear-regression.git
```
2. Install the dependencies
```bash
pip install pandas numpy matplotlib scikit-learn
```
3. Run the script
```bash
python main.py
```
<br>

## ✅ Results
This model achieved an R2 score of 0.93, indicating a strong correlation between the independent and dependent variables. The model was able to predict the net hourly electrical energy output of the plant with 93% accuracy. The actual and predicted values are visualized in a scatter plot and a DataFrame is created to compare the actual and predicted values. The DataFrame shows the first 20 rows of the test set, along with the actual value, predicted value, and residual error. A screenshot of the scatter plot is shown below.
<br>
<br>

![Scatter Plot of actual vs predicted electrical energy output](./results/scatter_plot.png?raw=true "Scatter Plot")
<br>
<br>



