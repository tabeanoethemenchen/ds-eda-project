# ds-project-template

Template for creating ds simple projects

## Requirements
For installation of the the virtual environment, run:

```
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

### Environment

This repo contains a requirements.txt file with a list of all the packages and dependencies you will need. Before you install the virtual environment, make sure to install postgresql if you haven't done it before.

```bash
brew update
brew install postgresql
```
### Task 
### Introduction to topic and task
The aim of this project is to familiarize with the EDA (Exploratory Data Analysis) part of the Data Science cycle.
For this purpose, several **steps** will be followed
- fetching data from a database
- data cleaning
- Getting an general overview
- explore correlations of data
- plotting different data points and correlations
- coming up with suggestions to the stakeholder

We work on the King County Dataset of houses and sales and we take on the role of a real estate marketer who wants to broker a property to client **Larry Sanders**.
The client has the following **requirements** for his new home:
- it should be located on the water
- Larry has a limited budget available
- the house should be in a nice condition
- the house should be located rather isolated
- no children should live in the immediate neighborhood, because Larry is afraid of germs
- he himself has some children

During the notebook the following **assumptions** were made
- Larry has at least 2 children
- a 'nice' condition refers to the objects with a `condition` of 4 or 5
- most people would like to have a bedroom for each of their kids; thus Larry would like to have at least 3 bedrooms (one for his own and one for each of his at least 2 kids). In addition, he wants his neighbors to have as little bedrooms as possible (because than it's more likely, that they don't have any kids)
- a house is isolated, when the distance to the neighbors is high; re, the average size of neighboring plots or/and the size of one's own plot can be used as an indicator

In addition, we will address some **general questions**:
- how does the location at the waterfront influence the price?
- is the number of bedrooms associated with the size of the property?
- does the condition of the property influence it's price?


### Procedure
1. export of data from postgreSQL database
2. first exploration of data content (dimensions of table, columnames etc. (more details to colum names: `column_names.md)...)
3. exploration of correlations
4. reducing the number of properties due to the requirements of the client
5. analysing the **general questions** above
6. coming up with 3 suggestions for the client