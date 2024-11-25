# Project Deliverables

1. **Project report** - to be submitted here -
   - include RMD file and HTML file and any additional files necessary to run your code, except for the provided `NLSY97.csv` file
   - due Tuesday, December 3, 2024, 2:00PM.
2. **Presentation of your project** - 10 minutes - must be given in person during the two allotted times on Monday December 2nd, and Wednesday December 4th, 2024.

# Central Question to be Investigated:

Choose ONE of the following two questions investigating income inequality:

I. **Sex-related differences**: Is there a significant difference in income between men and women? Does the difference vary depending on other factors (e.g., education, marital status, criminal history, drug use, childhood household factors, profession, etc.)?

II. **Race-related differences**: Is there a significant difference in income across racial groups? Does the difference vary depending on other factors (e.g., education, marital status, criminal history, drug use, childhood household factors, profession, etc.)? Note: for this problem you may find it easiest to focus on differences between just two groups. E.g., Black and non-Black, non-Hispanic.

To address this problem you will use the NLSY97 (National Longitudinal Survey of Youth, 1997 cohort) data set. The NLSY97 data set contains survey responses on thousands of individuals who have been surveyed every one or two years starting in 1997.

You will be using a pared down version of the full NLSY97 data set containing 90 variables.
See Canvas for:
- `NLSY97.csv`
- CodeBook file - explains the variables
- Starter Rmd File - starts you off with some basic variable renaming. Go further than what is done here.

A natural outcome variable for the data is **TOTAL INCOME FROM WAGES AND SALARY IN PAST CALENDAR YEAR (2017 survey question)**. This variable gets renamed to `YINC-1700_2017` by the starter script provided. Note that this quantity is truncated aka topcoded, meaning that you do not get to see the actual incomes for the top 2% of earners. For the top 2% of earners, the income variable is set to the average income among the 2% of earners. The implication of this topcoding is something you’ll want to discuss as part of your analysis.

You are NOT expected to use all 90+ variables in your analysis. It suffices to choose a total of 8-14 variables (income, sex/race, + 6-12 others) and to perform a thorough analysis using just those variables.

# Collaboration Policy

This is a group project. You MUST work on this in teams of 3-4 students. Form your group here: People

Discussions between teams is allowed, but all work your team submits must be your own: It is not allowable to use project code or text obtained from other sources, including AI tools, other teams, etc.

All students are expected to comply with the Illinois Tech Code of Academic Honesty. 
https://www.iit.edu/student-affairs/student-handbook/fine-print/code-academic-honesty

Any submitted project that is deemed by the instructor to be in violation of the collaboration policy or academic integrity policy will receive a score of 0.

# Project Report Requirements

Your R Markdown report must include the following sections:

## 1. Introduction: Data Processing and Summarization (10 points)

Begin by describing the data you have available. You will want to display tabular summaries of means and proportions where appropriate. Since the main question is one of gender differences, you may want your tabular summaries to also break things down by gender.

Your score for this section will be based on the following criteria:
- Meaningful variable names, factor variables, and factor level names
- Insightful graphical and tabular summaries of the data
- Proper labelling of figure axes and table columns
- Discussion of the graphical and tabular summaries.

Note: Figures and tables that are presented without accompanying description/discussion will receive at most half credit. To earn full credit, you must describe what each table/figure is showing and discuss any key takeaways. In other words, it is not sufficient to simply display R output. You must also provide thoughtful discussion of the output. Make sure that your discussion could easily be understood by a first year college student trying to learn more about income inequality between men and women.

## 2. Methodology (10 points)

In this section you should provide an overview of the approach you took to exploring and analyzing the data. This is where you tell the story of how you got to your main findings. It is too tedious to carefully format plots and tables for every approach you tried, so you can also use this section as a place to explain the various types of analyses that you tried.

You should address at least the following questions:

i. How did you deal with missing values? What impact does your approach have on the interpretation or generalizability of the resulting analysis?

ii. How did you deal with topcoded variables? What impact does your approach have on the interpretation or generalizability of the resulting analysis?

iii. Did you produce any tables or plots that you thought would reveal interesting trends but didn’t?

iv. What relationships did you investigate that don’t appear in your findings section?

v. What’s the analysis that you finally settled on? What income and gender related factors do you investigate in the final analysis?

Note: Figures and tables that are presented without accompanying description/discussion will receive at most half credit. To earn full credit, you must describe what each table/figure is showing and discuss any key takeaways. In other words, it is not sufficient to simply display R output. You must also provide thoughtful discussion of the output. Make sure that your discussion could easily be understood by a first year college student trying to learn more about income inequality between men and women.

## 3. Analysis and Findings (10 points)

In this section you give a careful presentation of your main findings concerning the main problem of race/sex-related income (in)equality. You should provide, where appropriate:

- Tabular summaries (with carefully labelled column headers)
- Graphical summaries (with carefully labelled axes, titles, and legends)
- Regression output + interpretation of output + interpretation of coefficients
- Assessments of statistical significance (output of tests, models, and corresponding p-values)

Your analysis should include:
- a confidence interval 
- a hypothesis test and 
- a regression model

When utilizing confidence intervals and hypothesis tests, you should discuss and check the normality assumptions.
When running a regression, you should discuss whether the standard diagnostic plots indicate issues with the model (trends in residuals, variance issues, outliers, etc.). 

You will not receive full credit for your analysis unless you clearly display and discuss the diagnostic plots.

Note: Figures and tables that are presented without accompanying description/discussion will receive at most half credit. To earn full credit, you must describe what each table/figure is showing and discuss any key takeaways. In other words, it is not sufficient to simply display R output. You must also provide thoughtful discussion of the output. Make sure that your discussion could easily be understood by a first year college student trying to learn more about income inequality between men and women.

## 4. Conclusions and Discussion (5 points)

In this section you should summarize your main conclusions. You should also discuss potential limitations of your analysis and findings. Are there potential confounding variables that you didn’t control for? Are the models you fit believable?

You should also address the following question: How much confidence do you have in your analysis? Do you believe your conclusions? Are you confident enough in your analysis and findings to present them to policy makers? 
(Note that you will not be deducted points for saying that you are unsure of your analysis. But this is something to reflect upon.)

Note on submitting data files

You may assume that the person grading your report will have the file called `nlsy97.csv` in their working directory. Any other files that you need in order for your Rmd file to knit should be submitted along with your report. You will be responsible for submitting:

- The Rmd file that generates your analysis
- The resulting html file produced by knitting

## 5. Presentation (5 points)
The presentation will be 10 minutes long, and will give an overview of your project report. No project report will be accepted without the associated presentation. A separate link will be provided on Canvas to submit presentation slides.

