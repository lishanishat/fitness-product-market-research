# Fitness Product Market Research

Statistical analysis of customer data to build purchaser profiles for three treadmill product lines, using hypothesis testing to identify which customer traits actually distinguish buyers.

> Coursework project with Tanya Smriti Victor Charles.

## Business questions
- What are the demographic and fitness characteristics of buyers for each treadmill model (FE285, FE580, FE605)?
- Do customer characteristics (income, age) differ significantly across product lines?
- Does self-rated fitness level predict planned weekly usage?
- Does marital status affect treadmill usage?

## Data
Customer survey data (age, gender, education, marital status, planned weekly usage/miles, self-rated fitness, income) for three treadmill models. [Source](https://raw.githubusercontent.com/csbfx/cs22a/main/fitness.csv).

## Methods
- **EDA:** distributions of age, income, fitness level, and miles across product lines (histograms, box plots)
- **Central tendency analysis:** mean, median, mode across key variables
- **Hypothesis testing:** independent t-tests (usage by marital status; miles by fitness level) and one-way ANOVA (income across product lines), with normality/variance assumptions checked

## Key findings
- No statistically significant difference in treadmill usage between single and partnered customers
- Customers with higher self-rated fitness (4-5) plan significantly more weekly miles than those rating themselves lower (1-3)
- Income rises clearly by model (ANOVA, p < 0.001): FE285 (~$46,400 avg) < FE580 (~$49,000 avg) < FE605 (~$75,400 avg) -- FE605 buyers earn substantially more than buyers of the other two models

## Tools
Python, pandas, SciPy (t-tests, ANOVA), Matplotlib, Seaborn

## Run it
Open `Fitness_Product_Market_Research.ipynb` in Jupyter or Colab -- the dataset loads directly from the source URL, no download needed.
