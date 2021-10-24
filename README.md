# Tradelog Simulator

### What and Why

Python script ro simulate trading performance based on historical trading data. </br>
Script takes your trading Data (like Gross P/L or R/R) CSV as an input and creates a simulation for a given number of trades. </br>

![image](https://user-images.githubusercontent.com/6221944/138590780-6fc5477a-9164-4d23-8c92-3bac523c50c1.png)

Data input turnes into simulation plot 👇

![image](https://user-images.githubusercontent.com/6221944/138590861-83256593-e8e3-45bc-ae50-d5644e6e80a1.png)

The output can be used to analize the performance of your trading stratagy. The script can be modified to do other analytics.

### Libraries used

- [`pandas`](https://pypi.org/project/pandas/) for creating table-like dataframes to store your input and sim data
- [`tkinter`](https://docs.python.org/3/library/tkinter.html) for simple file dialog
- [`plotly`](https://pypi.org/project/plotly/) for nice looking graphs

### How it all works

1. Script takes a dataset, lets say 100 trades of your Gross P/L
1. Dataset is devided into ranges of outcomes from max win to max loss
1. The occurrence rate for each range is calculated
1. The rate is extrapolated over *n* number of trades and randomly shuffled
1. The rusult is randomly plotted as running P/L over a given number of trades

Example dataset

![image](https://user-images.githubusercontent.com/6221944/138591230-e46d5233-15db-4c10-ba1e-4cccd4793f74.png)

Each range (80 trades split in 5 ranges) and calculated outcome

![image](https://user-images.githubusercontent.com/6221944/138591237-0f124b4c-906b-4df0-9133-388c87fea26c.png)
![image](https://user-images.githubusercontent.com/6221944/138591363-6922b5a1-028c-4eb2-a7c5-3b47394ffd0b.png)

### Try the script

Prepare your data first. This can be a single column CSV. </br>
Run the script `tradelog_sim.py` and choose the file. On the output you get your current trading stats and simulation graph. </br>
***Make sute the column you are working with is named Data***

![image](https://user-images.githubusercontent.com/6221944/138591542-258cea41-2fa8-4c19-b9de-108a8ae2bce2.png)

