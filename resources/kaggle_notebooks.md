# Using Kaggle notebooks

Kaggle offers free compute (including 30 hour of GPU time per week) via their notebooks feature. See the documentation [here](https://www.kaggle.com/docs/notebooks) for the full details. Kaggle notebooks are a great solution especialy, if you are working with a Kaggle dataset or a model that requires GPU compute. There are some advantages and disadvantages to Kaggle notebooks over GitHub Codespaces:

**Advantages relative to GitHub Codespaces:**
1. Much more powerfull than a dual core GitHub codespace
2. Integreated directly with Kaggle datasets

**Disadvantages relative to GitHub Codespace:**
1. Limited/no real acces to underlying Linux instance
2. Less flexible/more cumbersome, especially for project with multiple files
3. Risk of causing merge conflicts

To illustrate the use of Kaggle notebooks for data science projects, let's walk through setting up the Cats vs Dogs image classifier. These instructions assume you already have a phone number verified Kaggle account, and a project repository that you are working on. If not, fork my [gperdrizet-image-classification repo.](https://github.com/4GeeksAcademy/gperdrizet-image-classification).

**To get started you will need to do ~3 things:**

1. Create a new Kaggle utility script notebook for the helper functions module and import it from GitHub
2. Create a new Kaggle notebook for the image classifier and import your notebook from GitHub
3. Add the dogs vs cats competition datasource to your Kaggle notebook

## 1. Create a Kaggle utility script notebook

This notebook will hold our helper functions module allowing us to import it into our project notebook, just like we would in a Codespace. If the project you are working on is just a single notebook and you are not importing custom functions from another file, you can skip this step.

1. Click your profile icon and select 'Your Work'
2. Click the '+ Create' button and choose 'New Notebook'
3. Name the notebook something descriptive (I chose image-classification-functions)
4. Under 'File' click Link to GitHub. (If this is the first time you have linked a notebook, follow the prompts to login and authorize)
5. Under 'File' click 'Import Notbook', select 'GitHub' and paste the full URL to the file on GitHub (not the repo main page!). Mine is [this](https://github.com/4GeeksAcademy/gperdrizet-image-classification/blob/main/src/image_classification_functions.py)
6. Click 'Import'

You should see a notebook interface with some example code. If you were setting a new project, you could start coding right away.

## 2. Get the notebook from GitHub

1. Click 'File' and select 'Link to GitHub'
2. Follow the prompts to Authorize Kaggle to access your GitHub profile
3. Click 'File', then 'Import Notebook'
