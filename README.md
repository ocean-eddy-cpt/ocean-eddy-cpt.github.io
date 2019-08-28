# Ocean Eddy CPT Website

[![Build Status](https://travis-ci.com/ocean-eddy-cpt/ocean-eddy-cpt.github.io.svg?branch=source)](https://travis-ci.com/ocean-eddy-cpt/ocean-eddy-cpt.github.io)

## About this repository

This repo is home to a [Sphinx](http://www.sphinx-doc.org/en/master/) project
used to generate <https://ocean-eddy-cpt.github.io>.
It uses [GitHub pages](https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages)
to host the project documentation.
The source code for the documentation lives in the `source` branch.
The built html lives in the `master` branch.
We use [doctr](https://drdoctr.github.io) to build the documentation on
[Travis CI](https://travis-ci.com/ocean-eddy-cpt/ocean-eddy-cpt.github.io).
This is configued in the `.travis.yml` file.

## Contributing to the documentation

The documentation can be written in either markdown (`.md`) or
restructuredtext (`.rst`).
To edit or add to the documentation, make a pull-request to this repo.

## Building the documentation locally

```bash
# install the required packages
pip install -r requirements.txt

# build the docs
cd doc
make html

# preview the output
cd _build/html
python -m http.server
```
