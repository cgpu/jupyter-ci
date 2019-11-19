# Jupyter CI

This repository demonstrates automated verification of a [Jupyter](http://jupyter.org/) notebook. Whenever the `.ipynb` file is updated it is executed by [GitLab Actions](https://github.com/features/actions). Any errors are automatically emailed to the author and clearly indicated by the following badge: ![build status](https://github.com/mwoodbri/jupyter-ci/workflows/Validation/badge.svg)

The provided example is a lightly modified version of the "Alignment viewing and filtering" recipe from [The scikit-bio cookbook](http://nbviewer.jupyter.org/github/biocore/scikit-bio-cookbook/blob/master/Index.ipynb). The [rendered version](http://nbviewer.jupyter.org/urls/gitlab.com/mwoodbri/jupyter-ci/raw/master/Alignment%20viewing%20and%20filtering.ipynb) is available via nbviewer.

To use your own notebook:

1. Clone this repository
2. Replace the notebook
3. Add any additional dependencies to `requirements.txt`. Note that the [SciPy Stack](https://www.scipy.org/stackspec.html#stackspec) is provided by default.
4. Check in your changes and push to GitLab

You'll then receive an email indicating whether the notebook could be executed and the badge will update accordingly.

This approach was inspired by an [investigation of data science reproducibility](https://markwoodbridge.com/2017/03/05/jupyter-reproducible-science.html) for Open Data Day 2017.

This repository is a port of [jupyter-ci](https://gitlab.com/mwoodbri/jupyter-ci/) from GitLab CI to GitHub Actions.
