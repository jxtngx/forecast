# Forecast Studio

## Overview

Forecast Studio is a public template for artificial intelligence and machine learning research projects using Lightning AI's [PyTorch Lightning](https://lightning.ai/docs/pytorch/latest/) on [Lightning Studios](https://lightning.ai/).


## Source Module

`forecast.core` should contain code for the Lightning Module and Trainer.

`forecast.components` should contain experiment utilities grouped by purpose for cohesion.

`forecast.pipeline` should contain code for data acquistion and preprocessing, and building a TorchDataset and LightningDataModule.

`forecast.serve` should contain code for model serving APIs built with [FastAPI](https://fastapi.tiangolo.com/project-generation/#machine-learning-models-with-spacy-and-fastapi).

`forecast.lab` should contain code for the command line interface built with [Typer](https://typer.tiangolo.com/) and [Rich](https://rich.readthedocs.io/en/stable/).

`forecast.pages` should contain code for data apps built with streamlit.

`forecast.config` can assist with project, trainer, and sweep configurations.

## Base Requirements and Extras

Forecast Studio installs minimal requirements out of the box, and provides extras to make creating robust virtual environments easier. To view the requirements, in [setup.cfg](setup.cfg), see `install_requires` for the base requirements and `options.extras_require` for the available extras.

The recommended install is as follows:

```sh
python3 -m venv .venv
source .venv/bin/activate
pip install -e ".[all]"
```
