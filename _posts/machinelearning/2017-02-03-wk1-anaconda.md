---
layout: post
title: "DLNDF: Anaconda & Jupyter "
author: nitya_n
modified:
categories: machinelearning
excerpt:
tags: [deep-learning, nanodegree, dlndf, anaconda]
image:
  feature: color-flame.png
comments: true
share: true
---

# Accountability: Progress Report (Thu, Feb 2)

> **TL;DR**
> 
> I am a lifelong learner and autodidact currently invested in growing my understanding of machine learning and deep learning. So I enrolled in the Udacity Deep Learning Nanodegree Foundations, a 17-week curriculum that covers key topics and concepts. I'm using these posts to keep myself accountable by sharing my progress and goals for each week.
> 
> [_You can read the longer version here_](http://study.camp/machinelearning/deep-learning-nd/)


```
TODAY
```
_Finish reviewing Anaconda and Jupyter lessons. Start watching the lessons on Regression_



## PART 1: Anaconda

The lesson was primarily focused on getting Anaconda installed and getting a cheat sheet for usage. I'll just put my cheatsheets here for reference.

> What is Anaconda?

 * Distribution of libraries and software specifically built for data science.
 * Conda = package and environment manager 

> Install Notes

I had an existing Anaconda install but decided to upgrade it after seeing the advice to move to _Python36_ given that is the default mandated for Jupyter. However, my upgrade attempt did open my eyes to some interesting issues, so thought I'd capture them.

Anaconda is available for Windows/MacOS/Linux. Installers here: [https://www.continuum.io/downloads](https://www.continuum.io/downloads).

It complements existing Python dist on computer. _Default Python used by programs will be that installed by Anaconda_. Udacity recommends: Python 3.5, 64-bit installer (required for Jupyter)

**I had**: Anaconda 4.3.9 for OSX (Python 2.7, 64-bit). I used ```conda update anaconda``` to update it from my previous 4.1.x version but it had conflicts with updating python versions. Instead I had to delete/move the "anaconda" directory from my home and then reinstall a fresh version from the downloaded package 

**I now have**: Anaconda 4.3.x on Python 3.6 However this removes previously created environments which required me to manually re-create them. To prevent this in future, I will adhere to best practice of _always_ exporting env to a saved YAML file within project directory.


> AboutPackages

Packages are modular components that reflect specific versions of software libraries for use within a Python runtime. A package can itself have dependencies on other packages.

```
# Install Package
> conda install numpy   

# Install multiple packages
> conda install numpy scipy pandas

# Install specific version of package
> conda install numpy=1.10```

# Dependencies auto installed (e.g., below installs numpy dependency as well)
> conda install scipy

# Update package (one at a time, or all for current environment)
> conda update tensorflow
> conda update --all

# List installed packages in environment
> conda list

# Remove package
> conda remove tensorflow

# Search for package 
> conda search beautifulsoup
```


> About Environments

Environments created sandboxes where specific versions of software dependencies are enforced, leading to deterministic runtimes. A default _python version_ is associated with an environment at creation

```
# Ex: Create new env named "my_new_env" with listed packages
> conda create -n my_new_env numpy tensorflow

# Specify default python install for environment during creation
> conda create -n my_new_env python=3 numpy tensorflow

# Activate environment
> source activate my_new_env

# Deactivate environment
> source deactivate my_new_env

# Install packages within environment
> conda install

# Save environment to named YAML file
> conda env export > environment.yaml

# Load environment from named YAML file
> conda env create -f environment.yaml

# List environments
> conda env list

# Remove outdated environments
> conda env remove -n env_name
```


> Best Practies

1. Create two standard named environments set to Python2 and Python3. Always use these to do general purpose coding (since prompt will clearly show you which python context you are running in)
2. Always export environments to a local project-env.yaml file so that others can replicate/restore your environment in an effortless and deterministic manner. Also saves time when using a new computer or migrating to one.
3. Conda doc: [website](http://conda.pydata.org/docs/using/index.html)
4. Conda myths: [JVP article](https://jakevdp.github.io/blog/2016/08/25/conda-myths-and-misconceptions/)


```
TOMORROW:
```
_Finish reviewing Anaconda and Jupyter lessons. Start watching the lessons on Regression_
