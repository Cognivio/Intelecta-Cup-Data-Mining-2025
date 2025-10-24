# Readme

Model dari: [darts](https://github.com/unit8co/darts)

Kenapa pake linear?

- Kata reddit Linear bagus: [Reddit](https://www.reddit.com/r/MachineLearning/comments/18f12cj/d_doubts_on_the_implementation_of_lstms_for/)

## Notebook: [raruu-intelecta-cup-training 114.ipynb](./raruu-intelecta-cup-training%20114.ipynb)

- Metode: `LightGBMModel + NaiveSeasonal+ NaiveDrift`

- Score: 151.973
- Output: [submission_114.csv](./submission_114.csv)

## Notebook: [raruu-intelecta-cup-training-linear.ipynb](./raruu-intelecta-cup-training-linear.ipynb)

- Metode: `LinearReg + NaiveSeasonal+ NaiveDrift`

### alt:

- Score: 215.910
- Output: [submission_alt.csv](./submission_alt.csv)

```
split_idx = int(len(_df_ts) * 0.8)

lgbm_base = LightGBMModel(
    lags=lgbm_lags,
    lags_past_covariates=lgbm_lags,
    lags_future_covariates=None,
    output_chunk_length=10,
    random_state=42,
)

base_models = [
    lgbm_base,
    linreg_base,
    naive_drift,
    naive_seasonal
]
```

### low:

- Score: 146.533
- Output: [submission_low.csv](./submission_low.csv)

```
split_idx = int(len(_df_ts) * 0.8)

base_models = [
    # lgbm_base,
    linreg_base,
    naive_drift,
    naive_seasonal
]
```
