
Overview
- Notebook: [mainFile.ipynb](mainFile.ipynb)
- Dataset: [asylum_seekers.csv](asylum_seekers.csv)
- Purpose: preprocess UNHCR-style asylum data, engineer features, run classical ML and deep learning experiments, and produce a comprehensive evaluation report and visualizations.

Key cells / symbols
- Data & features: [`features`](mainFile.ipynb), [`X_train_scaled`](mainFile.ipynb), [`y_test`](mainFile.ipynb)
- Models (created in the notebook): [`seq_model`](mainFile.ipynb), [`deep_model`](mainFile.ipynb), [`func_model`](mainFile.ipynb), [`sub_model`](mainFile.ipynb), [`log_reg`](mainFile.ipynb), [`rf_model`](mainFile.ipynb), [`gb_model`](mainFile.ipynb)
- Evaluation & reporting: [`models_dict`](mainFile.ipynb), [`predictions`](mainFile.ipynb), [`metrics`](mainFile.ipynb)

How to run
1. Ensure dependencies are installed (cell near top runs pip install).
2. Open [mainFile.ipynb](mainFile.ipynb) in Jupyter / VS Code and run cells top-to-bottom.
3. The notebook loads [asylum_seekers.csv](asylum_seekers.csv), preprocesses, trains models, evaluates, and plots a 4x5 dashboard of results.

Outputs
- Console: printed accuracy/loss/classification reports for each model.
- Visual: combined figure with confusion matrices, ROC/PR curves, accuracy bar, prediction distributions, complexity comparisons and summary table.

Notes & tips
- Column names in the CSV are used as-is; the notebook handles a misspelled header `'Tota pending start-year'`.
- If you see "Too many bins" during hist plotting, reduce `bins` in the prediction-distribution plots or filter out NaN/inf probabilities before plotting.
- For reproducibility, seed is set for train/test split; adjust `random_state` in `train_test_split` or model constructors as needed.

Contact
- Use the notebook cells & inline comments for quick edits. Refer to the links above to jump to relevant cells/variables.


