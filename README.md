## Challenge_14 Readme

# Algorithmic Trading Strategies

---

## What this program does

In this program we will use machine learning models to test different trading strategies and compare these strategies by reviewing graphical and numeric data, including accuracy and precision.

---

## Technologies

This program can be run with Mac or Windows systems along with the following requirements:

Python 3.7.1

Jupyter Lab Notebooks

SKLearn

Pandas Library including hvplot



---


## Installation Guide

Make sure to run the appropriate imports:

`import pandas as pd`

`import hvplot.pandas`

`from pathlib import Path`

`import numpy as np`

`import matplotlib.pyplot as plt`

`from sklearn import svm`

`from sklearn.preprocessing import StandardScaler`

`from pandas.tseries.offsets import DateOffset`

`from sklearn.metrics import classification_report`

`from sklearn.linear_model import LogisticRegression`


For more information about Pandas, click [here](https://pandas.pydata.org/)

For more information about hvplot, click [here](https://hvplot.holoviz.org/)

For more information about SKlearn, click [here](https://scikit-learn.org/stable/)


---


## Conclusions


The following graph shows the actual and predicted cumulative returns for a 3 month training period. This graph shows that the predicted strategy returns performed just slightly better than the actual returns.

![Initial SVM returns_3_Month](https://github.com/EmilyBertani/Challenge_14/blob/main/Challenge_14_Starter_Code/SVM_strategy_returns_3_month.png)


The following graph shows the cumulative returns comparison with a 2 month training period. This graph shows that the predicted strategy returns did not perform much differently than the 2 month training period.

![SVM_Returns_2_Month](https://github.com/EmilyBertani/Challenge_14/blob/main/Challenge_14_Starter_Code/SVM_2_month_returns.png)


The following graph shows the cumulative returns with a 6 month training window. This graph shows that the predictions matched with the actual returns for longer than the 2 and 3 month training periods, but then predicted lower for a period of time before having higher predictions towards the end of the data. 

![SVM_Returns_6_Month](https://github.com/EmilyBertani/Challenge_14/blob/main/Challenge_14_Starter_Code/SVM_6_month_returns.png)


Based in these three graphs alone, it appears that the 3 month window strategy has the least amount of volatility.


The following graph shows a 3 month training period from above with the short SMA set to 7 days and the long SMA set to 200 days.

![SVM_Returns_SMA 7_200](https://github.com/EmilyBertani/Challenge_14/blob/main/Challenge_14_Starter_Code/7_200_SMA_windows.png)


The following graph shows a 3 month training period from above with the short SMA set to 7 days and the long SMA set to 150 days.

![SVM_Returns_SMA_7_150](https://github.com/EmilyBertani/Challenge_14/blob/main/Challenge_14_Starter_Code/7_150_SMA_windows.png)


This is the graph of the original training data with a 4 month short SMA and a 100 day long SMA

![SVM_Returns_Original_SMA_4_100](https://github.com/EmilyBertani/Challenge_14/blob/main/Challenge_14_Starter_Code/Original_SMA_4_100.png)

As you can see from these graphs, it appears that using a short window of 7 days and a long window of 150 days predicts slightly better with less volatility than the original 4 day short window and 100 day long window. This will be the strategy that I recommend.

---


## Contributors

Emily Bertani

Emily.Bertani.MD@gmail.com

[LinkedIn](https://www.linkedin.com/feed/)

---

## Licenses

MIT

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

