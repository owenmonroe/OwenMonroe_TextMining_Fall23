This is a guide to help you set up Python, Jupyter notebook, and other packages you will need on your system to engage in class lab activities. _You are NOT required to use Python for your assignments and projects._ However, because Python seems to be the most commonly used language for text mining/NLP these days, we will focus on it for practice.

# Download and install Anaconda environment for Python 3.8
[https://www.anaconda.com/download/](https://www.anaconda.com/download)

Anaconda environment will help you manage and deploy packages/libraries more efficiently.

To get started with conda, see [Conda Getting Started guide](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html) 

# Create new anaconda environment for this class called _textmining_ 

```sh
conda create --name textmining python=3.8.8
```

# Activate environment

```sh
source activate textmining
```

# Check version (should be 3.8.8)

```sh
python --version 
```
# Install packages

Be sure to install these specific versions so that everyone in the class is using the same environment and debugging is easier.

```sh
conda install nb_conda=2.2.1
conda install nltk=3.6.2
conda install -c conda-forge spacy=3.0
conda install scikit-learn=0.24.2
conda install pandas=1.3.1
conda install matplotlib=3.4.2
```

# Install spaCy English model

```sh
python -m spacy download en_core_web_sm
```

# Install wordcloud for visual representation of the corpus

```sh
conda install -c conda-forge wordcloud
```

# Use Jupyter notebooks
Most class exercises will be provided to you as Jupyter notebooks. To open a Jupyter notebook in this setup, open up the terminal and navigate to the folder containing the notebook; then activate the textmining environment to access these libraries and start up the notebook:

```sh
source activate textmining
jupyter notebook
```

If you're new to Jupyter notebooks, you can check out a tutorial here:

* [Jupyter notebook tutorial](https://www.dataquest.io/blog/jupyter-notebook-tutorial/)

***

This guide has been adapted from [https://github.com/dbamman/anlp21/blob/main/0.setup](https://github.com/dbamman/anlp21/blob/main/0.setup). 
