# Statistics for Data Science
- *Probability*
- *Distribution of Random Variables*
- *Introduction to Statistical Inference*
- *Hypothesis Testing*
- *ANOVA, Goodness of Fit, and Bootstrapping*
- *Linear Regression*
- *Logistic Regression*
- *Time Series*
- *Introduction to Causal Inference*

## [The Winning Switch: Unraveling the Monty Hall Paradox via Simulation] (https://github.com/amanjot-git/data-science-UofT/blob/main/Statistics%20for%20Data%20Science/MontyHall.ipynb)
Inspired by a classic probability puzzle, I developed a Python simulation to explore the Monty Hall problem. This exercise was not only intellectually stimulating but also a great example of how simulation can shed light on counterintuitive probability outcomes.

### Simulation Setup:
The simulation was designed to run thousands of iterations of the Monty Hall game. In each iteration, a car was randomly placed behind one of three doors, and the contestant made an initial choice. The host then opened one of the remaining doors, always revealing a goat.

### Strategy Comparison:
I simulated two strategies: sticking with the initial choice versus switching to the remaining door. By recording the outcomes for each strategy across thousands of iterations, I was able to compare win rates directly.

### Results and Insights:
The simulation consistently demonstrated that switching doors increased the win rate significantly compared to staying with the initial choice. This exercise not only confirmed the counterintuitive nature of the Monty Hall problem but also highlighted the power of simulation in validating probabilistic models and hypotheses.

This project is a prime example of how theoretical probability can be brought to life through simulation, providing tangible evidence to support the strategy of switching doors.

## [Buzzing Differences: Beer vs. Water in Mosquito Attraction Revealed](https://github.com/amanjot-git/data-science-UofT/blob/main/Statistics%20for%20Data%20Science/BeerVsWater.ipynb)
In a project focused on behavioral science and experimental design, I analyzed a dataset that measured the number of mosquitoes attracted under two different treatments: beer consumption versus water consumption.

### Visual Data Exploration:
I began by loading the mosquitos dataset and creating side-by-side boxplots to visually compare the distribution of mosquito counts between the Beer and Water groups. The visualizations revealed that the Beer group had a higher median and a wider interquartile range compared to the Water group.

### Descriptive Statistics:
I computed key descriptive statistics (mean, median, and standard deviation) for each group. The statistics confirmed that, on average, more mosquitoes were attracted when beer was consumed. This provided initial evidence of an association between beer consumption and increased mosquito attraction.

### Permutation Testing via Resampling:
To test the significance of this association, I implemented a permutation test by resampling the data over 10,000 iterations. The test calculated a very low p-value, leading to the rejection of the null hypothesis. This statistically supported the claim that there is a meaningful association between beer consumption and mosquito attraction.

This project combined exploratory data analysis with rigorous statistical testing to validate experimental findings—demonstrating the effectiveness of resampling techniques in hypothesis testing.

## [Risk, Rewards, and Returns: Statistical Inferences in Finance and HR] (https://github.com/amanjot-git/data-science-UofT/blob/main/Statistics%20for%20Data%20Science/CAPM.ipynb)
In another multifaceted project, I applied statistical inference methods to assess both financial and operational data. The project had two key parts: analyzing portfolio performance under the Capital Asset Pricing Model (CAPM) and evaluating the effectiveness of a new HR rewards system on reducing employee absenteeism.

### Analyzing Portfolio Performance:
I used statistical measures such as z-scores and p-values to analyze the distribution of portfolio returns assumed to be normally distributed under CAPM. By calculating expected returns and the probability of negative returns, I provided insights into the risk profile of the portfolio. Additionally, I computed cutoff points for the highest 15% of returns, offering valuable benchmarks for portfolio performance.

### Evaluating HR Rewards System:
Past data indicated that low morale led to significant absenteeism. After the implementation of a new rewards system, I collected a sample of employee data and performed a hypothesis test to determine whether absenteeism had decreased significantly. The test results, based on a 90% confidence level, showed that the new rewards system was effective. I further calculated the probability of a Type II error (missing the reduction in absenteeism) and determined the required sample size for achieving a β of 5%.

### Chi-Square Goodness-of-Fit:
Finally, I performed a chi-square goodness-of-fit test on stock return streaks to evaluate whether the observed distribution of streaks followed the expected geometric distribution. The test confirmed that the stock return streaks did not deviate significantly from the expected values, thereby supporting the efficient market hypothesis.

This comprehensive project showcased how combining financial analysis with HR analytics and robust statistical testing can lead to actionable business insights, helping organizations make informed decisions on both risk management and employee engagement strategies.

## [Linear Logic: Transformations, Diagnostics, and the Art of Regression] (https://github.com/amanjot-git/data-science-UofT/blob/main/Statistics%20for%20Data%20Science/LinearReg.ipynb)
In a project centered on regression analysis, I explored several datasets to understand the nature of relationships between variables, applying both linear and non-linear models as needed.

### Exploratory Analysis and Data Transformation:
I began by creating scatter plots for each dataset to visually inspect the relationship between variables. For datasets that displayed non-linear trends (such as exponential or logarithmic relationships), I applied various transformations (logarithmic, exponential, square root) to achieve linearity. This step was crucial because linear regression assumptions must be met for the model to be valid.

### Building OLS Regression Models:
Once the appropriate transformations were identified, I built Ordinary Least Squares (OLS) regression models on both the original and transformed data. For each model, I generated diagnostic charts—including residual plots, leverage plots, and influence plots—to check for normality, homoscedasticity, and the presence of outliers.

### Outlier Analysis and Model Comparison:
In datasets with influential outliers, I compared models built with and without these points. The removal of outliers often led to a noticeable change in the model’s slope, intercept, and R-squared values. This comprehensive analysis allowed me to interpret the regression coefficients accurately, offering insights into how the independent variables affect the dependent variable.

This project emphasized the importance of data transformations and diagnostic testing in regression analysis, ensuring that the final models were both statistically sound and practically interpretable.

## [Health Under the Lens: Data-Driven Insights in Diabetes Risk & Prevention] (https://github.com/amanjot-git/data-science-UofT/blob/main/Statistics%20for%20Data%20Science/Diabetes%20Prevalance-%20Final%20Group%20Project.ipynb)
My most extensive project involved working with a large diabetes dataset. This project spanned data cleaning, enrichment, exploratory data analysis (EDA), hypothesis testing, and predictive modeling—all aimed at uncovering key risk factors for diabetes and informing preventive strategies.

### Data Cleaning and Enrichment:
I began by cleaning the dataset, addressing missing values and inconsistencies. I enriched the data by categorizing patients into different groups based on age, BMI, race, and HbA1c levels. For instance, I created age groups (Under 18, 18-44, 45-64, Over 65), BMI categories (Underweight, Healthy Weight, Overweight, Obesity), and classified HbA1c levels (Normal, Prediabetes, Diabetes). This categorization helped in stratifying the patient population and enabled more granular analysis.

### Exploratory Data Analysis (EDA):
I conducted extensive EDA by generating histograms, boxplots, and bar charts to visualize the distribution of continuous variables (age, BMI, HbA1c, blood glucose) and to compare diabetes prevalence across different groups. For example, side-by-side boxplots highlighted differences in HbA1c levels between diabetic and non-diabetic patients, while bar charts illustrated variations in diabetes prevalence by race and gender. Descriptive statistics and bootstrapping were used to generate confidence intervals, providing a robust statistical foundation for my findings.

### Statistical Analyses and Predictive Modeling:
I built logistic regression models to predict diabetes status based on key risk factors such as hypertension, heart disease, BMI, HbA1c levels, blood glucose levels, and smoking history. I also performed Chi-square tests to evaluate dependencies between diabetes and categorical variables like race and gender. Additionally, time trend analyses were carried out to examine how the prevalence of diabetes—and related health metrics—changed over time (from 2015 to 2022). This multi-layered approach provided insights into which groups were at higher risk and where targeted preventive measures could be most effective.

### Key Insights and Business Impact:
The analysis revealed that older populations, particularly those in the 45-64 and Over 65 age groups, as well as individuals in the Obesity and Overweight BMI categories, exhibited higher diabetes prevalence. Conditions like hypertension and heart disease further compounded the risk. The logistic regression models consistently showed that HbA1c and blood glucose levels were the strongest predictors of diabetes across all racial groups. These findings support targeted health interventions and preventive strategies, enabling healthcare providers to allocate resources effectively and design customized programs for high-risk populations.

### Conclusion
Each of these projects reflects my commitment to leveraging data science to drive actionable insights across varied domains. Whether  predicting financial defaults, solving classical probability puzzles, investigating behavioral phenomena, or advancing healthcare outcomes, my approach is centered on thorough data preprocessing, rigorous statistical testing, and thoughtful model evaluation.

By combining these methodologies, I have been able to provide stakeholders with clear, data-driven recommendations that not only improve operational efficiency but also enhance risk management and preventive healthcare strategies. I am excited to continue exploring new challenges and harnessing the power of data to transform insights into impactful actions.
