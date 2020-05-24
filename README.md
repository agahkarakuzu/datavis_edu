Elementary material &amp; env config to explore Plotly. BrainHack School 2019. 

# Presentation

[![](http://img.shields.io/badge/Zenodo-Presentation-orange?style=flat&logo=microsoft%20powerpoint)](https://zenodo.org/record/3841775#.XsqgFJ5Kg1I)


# Getting started 

### To work with the notebooks in this repository, you have 3 options.

#### 1- Just one click

All you need is a web browser. Cllick the Binder badge below and start working with the notebooks. 

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/agahkarakuzu/datavis_edu/master)

Note that changes you made to the notebooks won't be kept! Don't forget to download notebooks you modified before ending Binder session. 

**Bonus**
[![](https://img.shields.io/badge/Voila-Dashboard-red?style=flat&logo=jupyter)](https://mybinder.org/v2/gh/agahkarakuzu/datavis_edu/master?urlpath=%2Fvoila%2Frender%2FPlotly_Voila.ipynb)

#### 2- Repo2Docker 

If you still would like to work in a container, but also to run it on your local machine instead of Binder's cloud resources, repo2docker is the easiest solution for you! **Make sure that you have Docker installed and running.** Not fully supported for Windows users tho :/. 

First, simply install repo2docker form pyPI:

```
pip install jupyter-repo2docker
```
Then run the following command in your terminal: 

```
jupyter-repo2docker https://github.com/agahkarakuzu/datavis_edu.git
```

After building (it might take a while!), it should output in your terminal something like:

```
Copy/paste this URL into your browser when you connect for the first time,
    to login with a token:
        http://0.0.0.0:36511/?token=f94f8fabb92e22f5bfab116c382b4707fc2cade56ad1ace0
```

#### 3- Create a new conda environment 

Create a new Python 3.6 env: 

```
conda create -n datvis36 python=3.6 anaconda
```

Activate it:

```
source activate datvis36 
```

Clone this repository and navigate into it:
```
git clone https://github.com/agahkarakuzu/datavis_edu.git
cd datavis_edu
```

Install requirements: 
```
pip install -r requirements.txt
```

Install postBuild:
```
cat postBuild | while read in; do eval "$in"; done
```
This should work fine on OSX or Ubuntu, not sure about Windows. Worst case, you can just copy paste the whole content to your terminal :)

You are ready to go! Start your favorite Jupyter interface (ensure that you are in repo): 

```
jupyter notebook 
OR
jupyter lab
```

