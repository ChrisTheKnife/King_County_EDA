# Readme for King County EDA Project

This Readme-file gives an overview about:
* The project objective
* Description of the notebooks
* Needed datasets
* Requirements and setup

## Project Objective

Based on a dataset about sold houses in King County the needs of a certain stakeholder shall be inspected and recommendations should be drawn. The stakeholder may even be a seller or buyer of houses.

In this EDA the stakeholder is Amy Williams, a italian mafiosi. She has two needs:

1. Wants to sell several central houses (top 10%) over time
2. Needs average outskirt houses over time to hide from the FBI

My assumption is, that the second need is more urgent, so that it will be on prio 1 and handled first.

Based on these needs research questions are drawn:

**Need #2 - Prio 1**

„(Need) buy average outskirt houses over time to hide from the FBI“

Which estates are
* not central, 
* inconspicuous, 
* far away from the FBI, 
* not observed from the FBI,
* have good possibilities to escape?

**Need #1 - Prio 2**

„Sell several central houses (top 10%) over time“

* Which are the top 10% houses?
* At which time shall Amy sell them without causing a stir? 

## Description of the notebooks

* Need #2 will be analysed in [EDA_Amy_RQ2]
* Need #1 will be analysed in [EDA_Amy_RQ1]. This notebook is Work-in-Progress.

## Needed datasets

For both notebooks the following datasets are needed:
* Information about houses sold in King County: King_County_House_prices_dataset.csv . Find this one [here](https://www.kaggle.com/harlfoxem/housesalesprediction).
* Information about the airports which are located in Washington State: airports.csv . [Here](https://davidmegginson.github.io/ourairports-data/airports.csv) you will find a CSV which contains a big number of airport data. You might prepare the code in the notebooks in order to get the airports of Washington State.


## Requirements

- pyenv
- python==3.9.4

## Setup

For this purpose you use following commands:

```bash
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

### Unit testing (Optional)

If you write python scripts for your data processing methods, you can also write unit tests. In order to run the tests execute in terminal:

```bash
pytest
```

This command will execute all the functions in your project that start with the word **test**.
