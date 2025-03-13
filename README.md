# Life-Expectancy

## Literature Review

Existing research has examined the determinants of life expectancy, often focusing on socioeconomic factors such as GDP, income, and mortality rates. However, many studies have relied on single-year data, limiting their ability to capture temporal trends and dynamic relationships between variables. While previous research has recognized the importance of immunization coverage and the Human Development Index (HDI) in influencing life expectancy, a comprehensive analysis incorporating these factors alongside other relevant variables, such as socioeconomic indicators and healthcare access, remains scarce.

Furthermore, many existing studies have employed basic statistical models, such as linear regression, without fully leveraging the potential of more sophisticated methods, like mixed-effects models, to account for complex data structures and hierarchical relationships. Recent advancements in healthcare access, particularly in developing countries over the past 15 years, have significantly impacted mortality rates and life expectancy, underscoring the need for updated analyses that incorporate these changes.

Life expectancy, a fundamental indicator of a population's health and well-being, is influenced by a complex interplay of factors such as:

- **Health Factors**: Adult mortality, infant deaths, alcohol consumption, measles cases, BMI, polio coverage, diphtheria coverage, HIV prevalence.
- **Economic Factors**: Country status, income composition of resources, total expenditure, GDP.
- **Social Factors**: Schooling, population size, under-five deaths, thinness rates.

Understanding these factors is essential for developing effective public health strategies to improve global health outcomes.

## Research Question

**What are the key factors influencing life expectancy globally, and how do these factors differ between developed and developing countries over time?**

This research aims to explore the key determinants of life expectancy, particularly focusing on the disparities between developed and developing countries over time. By examining the evolving landscape of factors such as socioeconomic status, healthcare access, nutrition, and environmental factors, this study seeks to identify critical areas for intervention to promote longer and healthier lives.

## Data Sources and Methodology

### Data Creation

The life expectancy data used in this study is sourced from:

1. **World Health Organization (WHO)**: Data collected using standardized methods, including life tables and statistical tools that summarize mortality rates at different ages in a population.
2. **United Nations (UN)**: Supplementary demographic data collected from member states, including mortality rates and socioeconomic indicators.

### Response Variable:

**Life Expectancy**: Defined as the average number of years a newborn infant is expected to live if current mortality rates persist.

### Predictor Variables

- **Economic Factors**: GDP, income composition of resources.
- **Health Factors**: Adult mortality, infant mortality, alcohol consumption, immunization coverage (Hepatitis B, Polio, Diphtheria), HIV prevalence, measles cases, BMI.
- **Social Factors**: Schooling, population size, under-five deaths, thinness rates.

### Confounding Variables

- **Population size**: Larger populations may have higher mortality rates due to overcrowding and limited healthcare resources.
- **Healthcare infrastructure**: Differences in healthcare quality can impact life expectancy estimates.

These factors were considered but not included as direct predictors to minimize bias.

### Handling Missing Data

- **Numeric Variables**: Imputed with median values to reduce the impact of outliers.
- **Categorical Variables**: Missing values replaced with "Unknown."

A thorough data cleaning process was implemented to enhance reliability and validity.

## Exploratory Data Analysis (EDA)

### Key Findings

- Summary statistics revealed a significant variation in life expectancy (ranging from 36.3 to 89 years).
- Histogram analysis showed that most observations fall between 60 and 80 years, highlighting global disparities.

### Correlation Heatmap:

- **Positive correlation**: Schooling and life expectancy.
- **Negative correlation**: Adult mortality and life expectancy.
- **Strong correlation**: GDP and health expenditure.

EDA provided crucial insights into variable distributions, relationships, and potential multicollinearity issues.

## Analytical Methods

### Machine Learning Models

Three models were used to predict life expectancy as a binary outcome (High vs. Low):

1. **Logistic Regression**: Provides interpretable coefficients.
2. **Ridge Regression**: Addresses overfitting through regularization.
3. **Lasso Regression**: Performs feature selection by eliminating less relevant predictors.

### Model Evaluation

- ROC Curves were used to compare model performance.
- Logistic Regression and Lasso Regression performed the best.

### Predictor Importance Analysis:

1. Key determinants: Income Composition, HIV Prevalence, Infant Deaths.
2. Box Plots revealed disparities between developed and developing countries.
3. Temporal Trends: Life expectancy has generally increased from 2000 to 2015.
4. Scatter Plots: Showed strong correlation between schooling and life expectancy.
5. Geographical Analysis: Life expectancy varies significantly by region.

## Results and Discussion

### Top Predictors:

- **Income Composition**: Primary driver of life expectancy.
- **HIV Prevalence & Infant Deaths**: Negatively impact life expectancy.
= **Schooling**: Strong correlation with better health outcomes.

## Conclusion

This study investigated the key determinants of life expectancy, highlighting disparities between developed and developing countries. The results confirmed that:

- Income composition is the strongest predictor of life expectancy.
- HIV prevalence and infant deaths negatively impact longevity.
= Education (schooling) plays a crucial role in improving life expectancy.

Machine learning models provided insights into predictor importance and regional disparities. While life expectancy has improved globally over time, significant inequalities remain, necessitating targeted public health interventions.

## Limitations

- Reliance on secondary data may introduce biases.
- Limited predictor variables: Future research should incorporate environmental and policy factors.

## Future Work

- Implement mixed-effects models to account for hierarchical structures.
- Extend the study with real-time health data to assess emerging trends.
- Develop policy recommendations to address disparities in life expectancy.

This research underscores the importance of economic stability, disease control, and education in promoting healthier populations worldwide. By addressing these factors, policymakers can implement more effective strategies to enhance global life expectancy outcomes.
# Life-Expectancy
