# GLM Visualizations

This project provides visual demonstrations of commonly used **Generalized Linear Models (GLMs)**, tailored for user experience (UX) researchers and behavioral scientists. These models go beyond simple linear regression, enabling you to analyze binary outcomes, skewed durations, counts, proportions, and ordinal ratings more accurately.

## 📘 Purpose

Linear regression is widely used in UX research, but it assumes your outcome is continuous, normally distributed, and unbounded. UX data often breaks these assumptions. This project shows how to apply alternative models that better fit real-world data, helping researchers avoid misinterpretation and extract more meaningful insights.

Each model is demonstrated with:

- Simulated data representative of UX scenarios  
- A corresponding Bayesian model using `brms`  
- A `ggplot2` visualization with smoothed trends or predicted curves  
- Exported PNG plots for presentation or documentation

## 📦 Models Included

This R Markdown file demonstrates the following GLMs:

1. **Poisson Regression** - for modeling count data  
2. **Logistic Regression** - for binary (yes/no) outcomes  
3. **Negative Binomial Regression** - for overdispersed count data  
4. **Gamma Regression** - for skewed time/duration data  
5. **ExGaussian Regression** - for reaction time or response latency modeling  
6. **Ordered Logistic Regression** - for Likert-style ordinal scales  
7. **Beta Regression** - for proportions bounded between 0 and 1  
8. **Distributional Regression** - for modeling both the mean and variance of the outcome

## 📂 Outputs

All plots are saved to the `glm_plots/` directory in `.png` format using `ggsave()`.

Each plot is named after its corresponding model, e.g.:

- `poisson.png`  
- `logistic.png`  
- `gamma.png`  
- etc.

## 🛠 Requirements

To run this project, you’ll need the following R packages installed:

```r
install.packages(c("tidyverse", "ggplot2", "brms", "bayesplot", "cmdstanr"))
```

You must also have CmdStan installed for Stan-based modeling via brms.

📑 How to Use
Open the R Markdown file in RStudio

Run each code chunk or knit the whole document to HTML

Visuals and model outputs will be generated automatically

Check the glm_plots/ folder for exported PNG files
