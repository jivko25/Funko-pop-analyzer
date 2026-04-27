# Funko Pop Analyzer

Analysis of how the **film industry** (TMDB-style metadata) relates to the **Funko Pop!** collectibles market: genres, production geography, correlations between ratings and figure counts, average MSRP, and interactive visualizations.

## Project layout

| File | Purpose |
|------|---------|
| `movies.ipynb` | Load and clean movie data from `movies.csv` (TMDB-like dataset). |
| `funko.ipynb` | Process a Funko inventory export (`funko.csv`). |
| `index.ipynb` | Main report (**The Vinyl Kingdom**): loads processed `final_movies.csv` and `final_funko.csv`, hypotheses, Plotly charts, and narrative analysis. |

Raw data in the repo: `movies.csv`, `funko.csv`. Running the notebooks produces merged/final tables `final_movies.csv` and `final_funko.csv` (these can be large—do not push individual CSVs over GitHub’s size limits without [Git LFS](https://git-lfs.github.com/) or excluding them from history).

## Requirements

- Python 3.10+ (recommended)
- Jupyter Notebook, JupyterLab, or VS Code with `.ipynb` support

Install dependencies (minimum to run the notebooks):

```bash
pip install pandas numpy matplotlib seaborn plotly scipy dash jupyter
```

## Getting started

1. Clone the repository and open the project folder.
2. Install the dependencies (above).
3. Start Jupyter:

   ```bash
   jupyter lab
   ```

4. Suggested order:
   - Run `movies.ipynb` and `funko.ipynb` first (to build or refresh the final CSVs).
   - Then open `index.ipynb` for the full cross-domain analysis.

## Notes

- Imports include **Dash** and **Plotly**—some visuals are meant as interactive charts inside the notebook/browser context.
- If `git push` fails because of large files, see GitHub’s policy on objects over 100 MB ([Git Large File Storage](https://git-lfs.github.com/) or removing huge CSVs from Git history).

## License

Educational / analytical project. Add your own license if you redistribute.
