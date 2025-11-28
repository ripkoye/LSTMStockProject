new environment:

conda env create -f environment.yml -n lstmstockproject

conda activate lstmstockproject

conda install something

conda env export --from-history > environment.yml


to pull the environment:
git pull
conda env update -f environment.yml -n lstmstockproject --prune


project directory:
LSTMPROJECT/
 -- data/                  #ideally we have raw and modified separated
 ---- Stock-Market-Data
 -- src/
 ---- __init__.py
 ---- whatever scripts
 -- notebooks/
 ----- explore.ipynb
 -- models/
 ----- some random models.pth
 environment.yaml
 README.md
 main.py