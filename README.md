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

In 1989, the government of British Columbia presented its mission statement regarding the purpose of its public education system: "to enable learners to develop their individual potential and to acquire the knowledge, skills, and attitudes needed to contribute to a healthy society and a prosperous and sustainable economy." Graduating from secondary school is one of the key indicators of the success or failure of this mission statement. Furthermore, the differences in outcomes between graduates and non-graduates are stark. For example: compared with graduates, non-graduates earn 22% less on average, are less healthy and more likely to be incarcerated, and among the effects of these outcomes are lower tax revenues and increased government costs.
A categorical model that predicts the likelihood of a student graduating from secondary school could be used to give schools and districts more information about their students and more insight as to where time, staff and resources should be focused. At a more granular level, a teacher could be given this information in order to tailor the focus of a class to more academic or more practical topics. BC teachers are empowered to focus on big ideas as well as specific core and curricular competencies, so this prediction would inform how they plan and deliver the course content.
Publicly available data are 'masked' when groups/subsets are small enough to risk individuals being identified. For this reason, a Freedom of Information and Protection of Privacy (FIPPA) request will need to be made to access the raw data. Once a complete dataset is secured, categorical models (logistic regression, XGBoost, decision tree) will be explored.

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
