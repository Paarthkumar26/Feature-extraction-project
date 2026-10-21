# Anime Feature Extraction Project

This notebook uses pandas to extract useful fields from anime title strings and explore the resulting data. It reads `anime.csv`, derives episode counts and release durations, and checks for the highest-scoring and longest entries.

## Dataset

The notebook expects `anime.csv` in the same folder as the notebook. It includes anime ranking, title, and score information; title strings contain episode counts and release date ranges used by the extraction steps.

## Requirements

- Python 3
- Jupyter Notebook or JupyterLab
- pandas
- NumPy
- python-dateutil

Install the dependencies if needed:

```bash
pip install pandas numpy python-dateutil jupyter
```

## Run the notebook

1. Keep `anime.csv` beside `Feature extraction project.ipynb` (or update the path in the notebook).
2. Open the notebook in Jupyter Notebook or JupyterLab.
3. Run the cells in order.

## What the notebook does

- Loads and inspects the anime dataset.
- Extracts episode counts from the text in the `Title` column and converts them to integers in a new `Episodes` column.
- Extracts title release date ranges into a `Total Time` column.
- Converts each date range into an inclusive duration in months in a `Months` column.
- Finds the anime entry with the highest score and the entry with the most episodes.

The extraction logic relies on the title text following the patterns present in this dataset. Results describe the supplied `anime.csv` data and may need adjustment for differently formatted titles.
