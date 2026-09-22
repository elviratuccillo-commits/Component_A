# Component A 
## Introduction 
Component A is a Python project that analysis financial data. This project uses historical price data to analyse closing prices and identify trends through a moving average. 
The goal is to transform the input data into a visual output that can be used to observe price movements and trends. 

# Project Overview 
`analysis.py` loads historical price data from `prices.csv`, processes it using pandas, calculates a 20-day simple moving average, and using matplotlib generates a plot comparing the daily closing price with the moving average.

# Data 
The input dataset is stored in `data/prices.csv` and it contains two columns 
1. date: the date of each observation 
2. close: the closing price for that date 

Before the analysis, the data si loaded into a pandas DataFrame, the dates are converted into a date format and observations are sorted chronologically. 

# Output 
The output of the analysis is a plot showing the historical closing prices and the 20 day simple moving average. The plolt is s stored in `outputs/plot.png`. 

The output folder is excluded from Git tracking because the generated file can be recreated by running the analysis script.

# Project Structure 
```
Component_A/
│
├── data/
│   └── prices.csv
│
├── outputs/
│   └── plot.png
│
├── src/
│   └── analysis.py
│
├── .gitignore
├── .venv/
├── requirements.txt
└── README.md
```
## Main Component 
`src/analysis.py`: contians the main script 
`data/prices.csv`: input financial data 
`outputs/plot.png`: generated analysis result 
`requirements.txt`: contains the Python packages required to run the project.
`.gitignore`: specifies files and directories that should not be tracked by Git.
`.venv/`:contains the local Python virtual environment.
`README.md`: provides documentation for the project.

# Running the project 
1. Create the virtual environment 
```bash
python3 -m venv .venv
```
2. Activate the virtual environment 
```bash
source .venv/bin/activate
```
3. Install the dependencies 
```bash
pip install -r requirements.txt
```
4. Run the analysis 
Run the script `analysis.py`, it reads the input data and process the closing prices calculating the 20 day simple moving average, and generates the plot.
The resulting visualization is saved in:
`outputs/plot.png`




