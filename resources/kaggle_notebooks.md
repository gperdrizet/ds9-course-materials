# Using Kaggle notebooks

Kaggle offers free compute (including 30 hour of GPU time per week) via their notebooks feature. See the documentation [here](https://www.kaggle.com/docs/notebooks) for the full details. Kaggle notebooks are a great solution especialy, if you are working with a Kaggle dataset or a model that requires GPU compute. There are some advantages and disadvantages to Kaggle notebooks over GitHub Codespaces:

Advantages relative to GitHub Codespaces:
1. More powerfull than a dual core GitHub codespace
2. Integreated directly with Kaggle datasets

Disadvantages relative to GitHub Codespace:
1. Limited/no real acces to underlying Linux instance
2. Less flexible/more cumbersome to work on multiple file projects
3. Risk of causing merge conflicts

To illustrate the use of Kaggle notebooks for data science projects, let's walk through setting up the Cats vs Dogs image classifier. These instructions assume you already have a phone number verified Kaggle account, and a project repository that you are working on. If not, fork my [gperdrizet-image-classification repo.](https://github.com/4GeeksAcademy/gperdrizet-image-classification).

To get started you will need to do ~3 things:

1. Create a new Kaggle utility script notebook for the helper functions module and import it from GitHub
2. Create a new Kaggle notebook for the image classifier and import your notebook from GitHub
3. Add the dogs vs cats competition datasource to your Kaggle notebook

## 1. Create a new notebook

1. Click your profile icon and select 'Your Work'
2. Click the '+ Create' button and choose 'New Notebook'

You should see a notebook interface with some example code. If you were setting a new project, you could start coding right away.

## 2. Get the notebook from GitHub

1. Click 'File' and select 'Link to GitHub'
2. Follow the prompts to Authorize Kaggle to access your GitHub profile
3. Click 'File', then 'Import Notebook'
