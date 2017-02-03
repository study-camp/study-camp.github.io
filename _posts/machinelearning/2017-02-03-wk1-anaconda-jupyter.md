---
layout: post
title: "DLNDF: Anaconda & Jupyter "
author: nitya_n
modified:
categories: machinelearning
excerpt:
tags: [deep-learning, nanodegree, dlndf, tools]
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



### Goals

_Finish reviewing Anaconda and Jupyter lessons. Start watching the lessons on Regression_

### Anaconda

The lesson was primarily focused on getting Anaconda installed and getting a cheat sheet for usage. I'll just put my cheatsheets here for reference.

> What is Anaconda?

 * Distribution of libraries and software specifically built for data science.
 * Conda = package and environment manager 

> Install Notes

I had an existing Anaconda install but decided to upgrade it after seeing the advice to move to _Python36_ given that is the default mandated for Jupyter. However, my upgrade attempt did open my eyes to some interesting issues, so thought I'd capture them.

 1. Available for Windows/MacOS/Linux. Installers here: [https://www.continuum.io/downloads](https://www.continuum.io/downloads)
 2. Complements existing Python dist on computer. _Default Python used by programs will be that installed by Anaconda_
 3. Udacity recommends: Python 3.5, 64-bit installer  
 4. I have: Anaconda 4.3.9 for OSX (Python 2.7, 64-bit) 
    * I used ```conda update anaconda``` to update it from my previous 4.1.x version but it had conflicts with updating python versions
    * Instead I had to delete/move the "anaconda" directory from my home and then reinstall a fresh version from the downloaded package 
 5. Now have: Anaconda 4.3.x on Python 3.6 _however this removes previously created environments so I need to redo those_
 6. Note: See the notes on "saving/loading" environments later -- for future purposes, I plan to adhere to this approach and _always_ keep a saved YAML file within my projects, to simplify these kind of restores


```
AboutPackages
```

Packages are modular components that reflect specific versions of software libraries for use within a Python runtime. A package can itself have dependencies on other packages.

> 1. Install package: e.g.,  ```conda install numpy``` 
> 2. Install multiple packages: e.g., ```conda install numpy scipy pandas``` 
> 3. Install specific version of package e.g., ```conda install numpy=1.10```
> 4. Install dependencies e.g., ```conda install scipy``` also installs _numpy_ which _scipy_ depends on
> 5. Update package: ```conda update tensorflow``` (for one) or ```conda update --all``` to update all packages in that environment
> 6. List installed packages in environment: ```conda list``` 
> 7. Remove package: ```conda remove tensorflow```
> 8. Search for package ```conda search beautifulsoup```


``` 
About Environments
```

Environments created sandboxes where specific versions of software dependencies are enforced, leading to deterministic runtimes. A default _python version_ is associated with an environment at creation

_Managing env_

> 1. Create a new "named" environment:  ```conda create -n my_new_env numpy tensorflow``` (where -n provides arg for name)
> 2. Specify default python install for environment during creation: ```conda create -n my_new_env python=3 numpy tensorflow``` (use version can be general e.g., "2" or "3" - or specific e.g., "3.3")
> 3. Activate environment: ```source activate my_new_env``` (environment name will appear in terminal prompt as prefix)
> 4. Deactivate environment: ```source deactivate my_new_env```
> 5. Running ```conda install``` (or other package management commands) within an activated environment ensures changes are localized to that environment.

_Saving & Loading env_

> 1. Save environment: as metadata in _YAML_ format => ```conda env export > environment.yaml```
> 2. Load environment: recreate from _YAML_ => ```conda env create -f environment.yaml```
> 3. Note to self: save env to _yaml_ for any project by default. If you need to upgrade or move Anaconda and lost your previous created environments, this lets you restore them from files.
> 4. Listing enviroments: ```conda env list```
> 5. Remove outdated environments ```conda env remove -n env_name```

```
Best Practies
```


> 1. Using environments: _recommends created pre-defined py2 and py3 named environments corresponding to Python2 and Python3 versions. Simplies the ability to do general purpose coding for each case_
> 2. Sharing environments: _recommends always creating saved env file for projects to allow others to restore/replicate your work._ (Note to self: let's use convention of adding _conda_env.yaml_ as default named file for project )
> 3. Conda doc: [website](http://conda.pydata.org/docs/using/index.html)
> 4. Conda myths: [JVP article](https://jakevdp.github.io/blog/2016/08/25/conda-myths-and-misconceptions/)


### Jupyter



### Fri Goals:

_Finish watching the lessons (5) on Regression and (6) on Siraj's Neural Network_
