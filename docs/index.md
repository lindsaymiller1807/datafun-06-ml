# Project Documentation

> Use this hosted documentation site to tell your
> data story. Include a narrative telling your
> results, observations, and interpretations.
> Display visuals as needed for a compelling story.

## Professional Workflow

See [**Workflow B: Apply Example Project**](https://denisecase.github.io/pro-analytics-02/workflow-b-apply-example-project/)
to get a project like this running on your machine.

## Professional Projects

- We code like the pros to help us **focus on the analytics**.
- Most files in this repository will never be touched.
- If curious about a file, check out the
  [Professional Python Project Explainer](https://denisecase.github.io/professional-python-project-explainer/).

## Documentation Index

- **Home** - this landing page
- [**Project Instructions**](./project-instructions.md)
- [**Concepts**](./concepts.md)
- [**Data Card**](./data-card.md)
- [**API**](./api.md)

## Initial Results

I used **flipper length (mm)** to predict **body mass (g)** for the Palmer Penguins dataset using a simple linear regression model.

The model learned the following relationship:

```text
body_mass_g = 49.851 × flipper_length_mm - 5816.874
```

### Model Results
- **Baseline RMSE:** 751.68
- **Linear Regression RMSE:** 356.05
- **Baseline R-squared:** -0.002
- **Linear Regression R-squared:** 0.775


The linear regression model performed much better than the baseline model. The RMSE decreased from 751.68 grams to 356.05 grams, meaning the model's predictions were much closer to the actual body masses.

The R-squared value of 0.775 means that approximately 77.5% of the variation in body mass in the test data was explained by flipper length in this model.

### Prediction Plot

The prediction plot shows a clear positive relationship between flipper length and body mass. Penguins with longer flippers generally had greater body mass.

![Flipper Length vs. Body Mass](./images/regression-predictions.png)

### Residual Plot
The residuals are scattered above and below zero. This means the model sometimes overpredicts and sometimes underpredicts body mass rather than consistently making errors in only one direction.

![Residuals for Flipper Length Model](./images/regression-residuals.png)

### Interpretation

Based on these results, flipper length appears to be a useful predictor of body mass for this dataset. The linear regression model improved substantially over the baseline model, reducing RMSE from 751.68 grams to 356.05 grams. The model also achieved an R-squared value of 0.775, meaning that about 77.5% of the variation in body mass in the test data was explained by flipper length. However, the residual plot shows that some prediction error remains, so flipper length alone does not explain all variation in body mass.
