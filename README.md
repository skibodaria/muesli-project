# Project - Data Analysis

This project was developed by the Data Analytics team at [Spiced Academy / neuefische GmbH](https://www.spiced-academy.com/en) and is centered around exploratory data analysis [(EDA)](EDA_Checklist.pdf) and statistical analysis techniques. It is performed as a group work and is delivered after the second teaching module of the [Data Analytics Bootcamp](https://www.spiced-academy.com/en/program/data-analytics).

## Topic and Task
The task was to complete a case study and answer specific questions, coming from a stakeholder by performing data analysis and visualisation.  The detailed [task description](assignment.md) is provided.

## Suggested Workflow for GitHub
* the original repository is [provided](https://github.com/spiced-academy/cayenne-clusters-m2-muesli-project),
* one of the team members [forked](https://github.com/skibodaria/cayenne-clusters-m2-muesli-project) it and added the others as collaborators

These both repositories are not available for GitHub users outside of the Spiced Academy / neuefische GmbH environment, so this repository is a **mirror** of the original team repo. It represents the analysis I implemented using the provided data and task, and also the files we used to present the results as a team. To check out the work of all collaborators, either check the commit history, or address them directly:
* [Erick B. Salas](https://github.com/PatricioElLobo)
* [Antonio Schmidtgen](https://github.com/antonio-schmidtgen)

## Additional Instructions
* include or check the `.gitignore` file in the repo. At the least the **data** folder should be listed, since it's better to make sure **not to push any data to GitHub**;
* recommended but not necessary: work on different branches;
* create a new `.ipynb` file and start with the EDA!
  - it's a good idea to split different steps into different notebook; intermediate results can be saved as `.csv`-files;
  - when working separately from team mates, use different files that can be combined later, or work carefully to avoid merge conflicts;
* split tasks in the group, push results and merge into main if other person needs the results;
* in the end: merge everything into the main branch.

## Main Steps:
1. **Data Load & Read**: the data was unpacked from a `.zip` file and read from `.xlsx` file tabs. Each tab was saved as an independent `.csv` files.
> Normally, `.csv` files are not shared on GitHub but for the learning purpouses and reproducibility the raw files and the clean versions are saved in the folder [/data_csv](/muesli-project/data_csv).

2. **Data Cleaning & Merging**: each of the four separated tables was examined and cleaned (e.g., data formats, duplicated values, etc.). Each tab was then was saved for archiving and iterative research design purposes. After the four tables were merged together to be able to picture and trace the Muesli company workflow -- from an order to warehouse to logistics company to actual delivery.

3. **Data Engineering**: several additional metrics were created to understand if the delivery process matches the description and target provided by the warehouse manager and logistics company manager. 

4. **Data Exploration: Distributions, Descriptive Statistics**: statistical overview for week structure, different order characteristics, and delivery process was created.

5. **KPIs: Calculation & Visualization**: multiple visualizations were build to see if region, shipment mode, number os items ordered, day of ordering, origin etc. affect the delivery process.

6. **Conclusions & Recommendations**: main conclusions were summarized in a presentation and delivered to the class.

## Repo Structure
* `[assignment.md](assignment.md)` is a list of instructions for the project, including the main deliverables and questions + KPI targets;
* `[eda_checklist.pdf](eda_checklist.pdf)` serves as a reminder of the main steps at this stage of analysis;
* `[/data_csv](data_csv)` provides with the data on the Muesli company ordering and delivery process;
* `[/analysis](analysis)` contains an `[eda_analysis.ipynb](analysis/eda_analysis.ipynb)` with all the stages described above, from data loading to formulating conclusions;
* `[/presentation]` provides materials in `.pptx` format, being presented and discussed in the class.