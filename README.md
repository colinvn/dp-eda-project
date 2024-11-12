# Exploratory Data Analysis (EDA) project

This repository was created as part of a part-time data science bootcamp by neue fische. Students were provided with a dataset on house prices in King County (Washington, USA) found in `data/King_County_House_prices_dataset.csv`.

The task was to conduct exploratory data analysis (EDA) in a Jupyter notebook with a particular client's profile in mind. The full assignment can be found in `resourceses/assignment.md`. The client chosen for this notebook was _Amy Williams_, whose profile will be described below. The time allotment was five half-days.

## Content


This repository contains:
- `EDA.ipynb`: Jupyter notebook with the completed EDA task; this is the main file
- `requirements.txt`: lists the required Python packages (see below on how to install)
- dir `data`: folder with the original housing data; further data will be loaded into this directory by the notebook
- `EDA-slides.pdf`: a reduced form of the final presentation
   - the actual presentation was created using Jupyter slides to allow for interactivity
   - see the instructions below on how to re-create the interactive slides (requires running the notebook)
- dir `resources`: folder with further material, in particular
   - images used for the slides
   - `assignment.md`: original task description
   - `workflow.md`: further task explanations
   - `column_names.md`: original column data description
   - dir `optional`: supporting scripts that were not used
   - dir `starters`: original `README-starter.md`, `EDA-starter.ipynb`, and `requirements-starter.txt` files which have been changed as part of the exercise

The findings were presented jusing Jupyter slides. Instructions in re-creating the slides can be found below. The notebook first goes through the steps of EDA in iterated cycles of assessment/understanding, preparation/cleaning, analysis, and visualisation. At the end, cells for a slide show are set up.

## Setup

Requirements:
- pyenv
- python==3.11.3

Install the virtual environment and the required packages by following commands:

   ```BASH
   pyenv local 3.11.3
   python3 -m venv .venv
   source .venv/bin/activate
   pip install --upgrade pip
   pip install -r requirements.txt
   ```

Afterwards, open and run `EDA.ipynb`. In addition, if you want to create Jupyter slides, run

   ```BASH
   jupyter contrib nbextension install --sys-prefix
   ```

when you set up the environment. After the notebook was successfully run, do

   ```BASH
   jupyter nbconvert EDA.ipynb --to slides --no-input --post serve
   ```

to create the slides. 