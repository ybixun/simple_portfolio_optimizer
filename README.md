[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# Simple Portfolio Optimizer Project

This project provides a portfolio optimizer model that allows asset/portfolio managers to efficiently get an optimized allocation of stocks and bonds based on annualized returns and conditional variance-at-risk (VaR).

## Introduction

This project was actually done for the purpose of my school module where we are required to do up an individual project that involves using linear optimization to resolve a business problem. Being someone from a finance/accounting background, I thought of using linear optimization to improve the efficiency of coming up with allocation of assets and bonds to get an optimized portfolio for clients depending on their risk appetite and their expected returns.

In this case, WealthisHealth Pte. Ltd. is a fictitious company that will roleplay as the client in this project.

Gurobi solver was originally used for the optimization model for the purpose of school project. Now that I put it up on my github public repository, I editted the code and changed it to using ORT-Tool, an open-source solver, so the portfolio optimizer can be used anytime.

## Features

- Linear-optimization model that can be utilized to get optimized allocation of assets.
- Data visualisation on aiding the asset/portfolio manager in other aspects of portfolio management.
- Automation in extracting the returns and details from all the .csv documents into a master list of consolidated stocks. 

# Usage

This project is done solely on Jupyter Notebook and can be accessed using the following way:

## 1. Setup

* Ensure you have Python and Jupyter Notebook installed, or Anaconda Software on your machine. Please refer to respective installation guides for the different softwares required for the setup.

* Clone the repository into your local directories or download the files.

```bash
git clone https://github.com/[YourUsername]/[YourRepository].git
```

* Navigate into the cloned repository.

```bash
cd [YourRepository]
```

## 2. Dependencies

The dependencies for this project are listed in the requirements.txt file located in the project's root directory.

* To install these dependencies, you can use pip by running the following command in your terminal:

```bash
pip install -r requirements.txt
```

* For conda environments, you can use the environment.yml file with the following command:

```bash
conda env create -f environment.yml
```

## 3. Run Jupyter Notebook

* Start the Jupyter Notebook server by running this command in your terminal:

```bash
jupyter notebook
```

This will open a new tab on your default web browser, showing a list of notebooks in the project.

## 4. Open the Notebook

* In the Jupyter Notebook server, navigate to the directory containing the notebook files (.ipynb) and open the notebook file you wish to open.

## 5. Execute the Notebook

* You can run the notebook document step-by-step (one cell a time) by pressing shift + enter.

* Alternatively, you can run the whole notebook in a single step by clicking on the menu Cell -> Run All.

Please note that some cells may rely on the results of earlier cells. Therefore, if you're running cells individually, make sure to run them in order.

## 6. Using the Portfolio Optimizer

* After running the whole notebook, you will be stopped at the selection segment where you are prompted for the amount to invest. Key in the amount that you wish to invest.

* Next, key in the portfolio style you wish to adopt. There are 5 to chose from:
1. High-Roller
2. Aggressive
3. Balanced
4. Conservative
5. Gradual Growth

* Subsequently, key in the maximum bond default score. Ensure that the amount key in is 1.0 or more.

* Lastly, key in the max porportion allowed for each asset, between 0 to 1 inclusive.

* The optimizer will run and results will be shown in a data table at the Optimiser section.


# Credits
Yu Bixun - Initial Work - https://github.com/ybixun

## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
This project is licensed under the terms of the [MIT License](LICENSE).
