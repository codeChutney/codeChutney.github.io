---
title: No non-sense ML quickstart
parent: AI
permalink: "/tutorial/ai/quickstart"
---

# No non-sense ML quickstart

It is important to get started quickly, get your hands dirty...when you want to learn something, especially code/technologies/frameworks.

So, here is a no non-sense quickstart for ML using Python, VS Code(IDE), Anaconda(Distro). Lets also use Jupyter Notebooks which also comes with the Python extension for VS Code.

**Why VS Code?** Lightweight, Free(for both Individual and Professional use at the time of writing this), (most) popular among python users, cross-platform, very good support for python and python for data science.

**Why Anaconda?** It is a distro that comes with the most popular AI/ML/Data Science dependencies or packages. You can learn these details later, don't let it delay you.

**Why Jupyter Notebooks?** Helps you divide your Python code into cells and run/debug them individually. Very useful when processing large data sets.

# Lets get started:
* Install VS Code. Simple .exe or .dmg download and execution from the Microsoft site with all defaults.
* Install Anaconda. Download [installer](https://docs.anaconda.com/anaconda/install/windows/){:target="_blank"} and run it with all the defaults.
* Open VS code, on the left pane you should see the Extensions button, click on it, type Pyhon in the search bar. Install the one from Microsoft.

	![]({{ 'Screen Shot 2020-09-11 at 21.05.33.png' | relative_url }})
 
* The only other thing is to tell VS code where the python interpreter is. Use the one from anaconda.
* Thats it for the setup. Now lets run the most popular and simple ML exercise.
* This is just a guide of how to get started, so paying no attention to naming conventions etc., hit ```Ctrl + Shift + p``` in VS Code. Now that the python extension is installed you should see 'Python: Create new blank Jupyter notebook' once you start typing 'Jupyter'. Select it.
* Name the file anything you want, say 'housing_price_predictor_model'. That should help create a ```*.ipynb``` file.
* That's it for now, lets write a couple of lines of code and then go get the csv files.

```
//should be part of anaconda
import pandas as pd
//setting the file path for melbourne data
melbourne_data_path = './housing_data/melb_data.csv'
```
* Not much we can do without the data. Here are the links to the cvs files on kaggle: [melbourne](https://www.kaggle.com/dansbecker/melbourne-housing-snapshot){:target="_blank"} and [iowa](https://www.kaggle.com/nickptaylor/iowa-house-prices){:target="_blank"} .
* Now lets take a look at the data. 

```
melbourne_data = pd.read_csv(melbourne_data_path)
// describes your data statistically(will show mean, count, standard deviation etc)
melbourne_data.describe()
//see the columns
melbourne_data.columns
//see count
melbourne_data.count()
```

### References(See/Read these):

1. [VSCode](https://code.visualstudio.com/Download){:target="_blank"}
2. [Anaconda](https://docs.anaconda.com/anaconda/install/windows/){:target="_blank"}
