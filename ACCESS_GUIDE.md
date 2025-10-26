# Access & Workflow Guide

## Data Access (Sciebo)
- Folder shared with assistant: https://rwth-aachen.sciebo.de/f/6347809912
- Access instructions:
  1. Accept the share and add it to your Sciebo client.
  2. On Windows it syncs under C:\Users\amirn\sciebo\thesis-data.
  3. Link inside the project (already set):
     rmdir data /S /Q
     mklink /J data "C:\Users\amirn\sciebo\thesis-data"

## Code & Notebooks (GitHub)
- Repository: https://github.com/anikoo79/thesis-rc-beam
- Typical workflow:
  conda activate thesis-env
  cd C:\Users\amirn\thesis-rc-beam
  git pull
  jupyter lab
  # work...
  git add -A
  git commit -m "message"
  git push

## Progress Verification
- Data registry: DATA_REGISTRY.csv
- Data access doc: DATA_ACCESS.md
- Key notebooks:
  - notebooks/00_environment_check.ipynb
  - notebooks/01_thesis_template.ipynb
  - notebooks/02_data_setup.ipynb
  - notebooks/03_ann_moment_capacity.ipynb

## Collaboration Workflow
- Incoming assistant files:
  - Data -> data/raw/assistant/ or data/external/
  - Scripts -> src/from_assistant/ or notebooks/from_assistant/
- After adding data: append a line to DATA_REGISTRY.csv and commit it.
