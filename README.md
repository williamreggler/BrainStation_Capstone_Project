# BrainStation Data Science Capstone Template

This is a template repository for setting up your capstone project: it includes a simple folder structure and placeholder files for the most important assets you will be creating.

## Usage

1. Start a new GitHub repo using this template.
2. Update your `LICENSE` file with date and owner.
3. Update your `README.md` file to reflect the project - see a sample structure below and please refer to Synapse on what needs to be included here. 
4. Set up and activate your conda environment:
    - Create a new `conda` environment for your capstone project.
    - Activate the environment and export:
        ```bash
        conda env export > conda.yml
        ```
    - Make sure re-export every time after you update the environment.
    - You can reset your conda environment by running:
        ```bash
        conda env create -f conda.yml
        conda activate <your-env-name>
        ```
5. Add your own notebooks in `./notebooks/` and remove placeholders.
6. Add your own data in `./data/` and remove placeholder. Note: `.gitignore` will ignore the data folder when you push to github, save a copy of your raw and processed data, pickled models in a Google Drive folder and add the link in the `data_links.md` file.
7. Add your project documents, figures, reports, presentation pdf's in the `./docs` and remove placeholders.
8. Add your references (tutorials, papers, books etc.) in `./references`. 
9. Add your own scripts in `./src/` and remove unnecessary folders.

Feel free to rename the folder and customize the project structure to best fit your work - this template is just the starting point.

------------------------------------------------------------------------------

## Predicting Likelihood of Graduating from Secondary School in British Columbia
=========================

### Executive Summary

Marathon running has grown exponentially in popularity over the last few decades, with events like the Boston Marathon attracting tens of thousands of participants from around the world. For many, marathons symbolize a pinnacle of personal achievement, offering the unique opportunity for amateur runners to compete alongside elite athletes on the same course. Beyond the emotional and social appeal, marathons provide significant physical and mental health benefits, including improved cardiovascular fitness, mental resilience, and community connection. However, the distance of 42.2 kilometers (26.2 miles) presents immense physical and psychological challenges, especially in pacing and endurance management.

This project aims to leverage data from the Boston Marathon (2015–2017) to develop a machine learning model that predicts a runner’s performance change between the first and second halves of the race – a phenomenon often referred to as "positive splitting." Using data from the Boston Marathon from 2015 to 2017, the baseline model is a random forest regressor, chosen for its ability to handle complex, non-linear relationships. Additional algorithms, such as XGBoost, will be explored to improve accuracy and robustness. Key features include demographic variables and times and paces at key milestones (e.g. 15K, 25K). This predictive model seeks to uncover patterns and trends that influence pacing strategies and runner outcomes.

The insights generated from this project hold value for multiple stakeholders. Runners could use the predictions to fine-tune their training and pacing strategies, reducing the risk of exhaustion or injury and optimizing their race-day performance. Race organizers could also benefit by using these insights to adjust course resources, such as medical aid stations, water distribution, and volunteer placement, ensuring better safety and support for all participants. By combining the power of machine learning with historical data, this project aspires to contribute to the broader understanding of marathon performance and preparation.

### Demo

... Show your work:
...     Data visualizations
...     Interactive demo (e.g., `streamlit` app)
...     Short video of users trying out the solution


### Methodology

... High-level diagrams of entire process:
...     various data processing steps
...     various modelling directions
...     various prototyping directions


### Organization

#### Repository 

* `data` 
    - contains link to copy of the dataset (stored in a publicly accessible cloud storage)
    - saved copy of aggregated / processed data as long as those are not too large (> 10 MB)

* `model`
    - `joblib` dump of final model(s)

* `notebooks`
    - contains all final notebooks involved in the project

* `docs`
    - contains final report, presentations which summarize the project

* `references`
    - contains papers / tutorials used in the project

* `src`
    - Contains the project source code (refactored from the notebooks)

* `.gitignore`
    - Part of Git, includes files and folders to be ignored by Git version control

* `conda.yml`
    - Conda environment specification

* `README.md`
    - Project landing page (this page)

* `LICENSE`
    - Project license

#### Dataset

... Google Drive links to datasets and pickled models

### Credits & References

... Include any personal learning
