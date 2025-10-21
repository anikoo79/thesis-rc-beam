# Data Access

## Sciebo (Primary Storage)
- Folder: C:\Users\amirn\sciebo\thesis-data
- How project links to it (Windows):
  1) rmdir data /S /Q
  2) mklink /J data "C:\Users\amirn\sciebo\thesis-data"

## Layout (expected)
- data/raw/ (originals, immutable)
- data/external/ (lightly cleaned third-party)
- data/interim/ (working files)
- data/processed/ (analysis-ready datasets)
- data/samples/ (tiny samples kept in GitHub)

## Small samples in Git
- data/samples/beam_samples_small.csv
