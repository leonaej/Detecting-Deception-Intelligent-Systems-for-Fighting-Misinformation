# Data-Related Information

A `LIAR_data.tsv` file is used, downloaded from Kaggle.

The data is pre-processed to create metadata, and the features are split into three CSV files:

1. **original_features.csv** — Used in `section1.ipynb`; only the statement from the features is used.
2. **combined_df.csv** — Contains the newly created features; used in `section2.ipynb`.
3. **section3.csv** — Contains a sentence-structured column combining all original features; used in `section3.ipynb`.


# How to Run the Code

**Step 1:** Run `feature_engineer.ipynb` to create the CSV files needed for the three sections. One step uses an LLM to extract semantic features.

**Step 2:** Run `section1.ipynb`. This produces a CSV with the truth percentage predictions using only the statement.

**Step 3:** Run `section2.ipynb`. This gives predictions based on the engineered features.

**Step 4:** Run `section3.ipynb`. This produces predictions from the sentence created using the original features.

**Step 5:** Run `endemble.ipynb`. This combines outputs from all three models and determines the optimal weights for final ensemble predictions.
