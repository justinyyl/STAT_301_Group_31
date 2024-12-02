# STAT_301_Group_31

# Group Final Report
Create an electronic report with a maximum of 2000 words (excluding citations) using Jupyter. The report should include the posed question, conducted analysis, and derived conclusion. Only one team member needs to submit this report. It is not required to include all tasks completed by each group member in their individual assignments. Make sure to reach a consensus among all team members on the final content of the report. If needed, consult your TA and Instructor for further guidance.

You must submit two files:
- The source Jupyter Notebook (```.ipynb``` file)
- the rendered final document (```.html``` file)

All pieces of code in your Jupyter Notebook must have a comment saying who was responsible for developing that piece of code and who else contributed, if any other member. For example,

```R
# Main developer: Rodolfo 
# Contributor: Seren (debugged)
model <-
     my %>%
     code %>%
     that %>%
     does %>%
     whatever
```
Also, keep your code clean and well-formatted. I strongly suggest you review [Tidyverse's style](https://style.tidyverse.org/syntax.html).

Each report should include the following sections:
- Title
- Introduction
- Methods and Results
- Discussion
- References

## (1) Introduction
Start with relevant background information on the topic to prepare those unfamiliar for the rest of your proposal.

Formulate one or two questions for investigation and detail the dataset that will be utilized to address these questions.

Additionally, align your question/objectives with the existing literature. To contextualize your study, include a minimum of two scientific publications (these should be listed in the References section).

## (2) Methods and Results
In this section, you will include:

### a) “Exploratory Data Analysis (EDA)”

- Demonstrate that the dataset can be read into R.
- Clean and wrangle your data into a tidy format.
- Plot the relevant raw data, tailoring your plot to address your question.
- Make sure to explore the association of the explanatory variables with the response.
- Any summary tables that are relevant to your analysis.
- Be sure not to print output that takes up a lot of screen space.
- Your EDA must be comprehensive with high quality plots.

### b) “Methods: Plan”

- Describe in written English the methods you used to perform your analysis from beginning to end, and narrate the code that does the analysis.
- If included, describe the “Feature Selection” process and how and why you choose the covariates of your final model.
- Make sure to interpret/explain the results you obtain. It’s not enough to just say, “I fitted a linear model with these covariates, and my R-square is 0.87”.
    - If inference is the aim of your project, a detailed interpretation of your fitted model is required, as well as a discussion of relevant quantities (e.g., are the coefficients significant? How does the model fit the data)?
    - A careful model assessment must be conducted.
    - If prediction is the project's aim, describe the test data used or how it was created.
- Ensure your tables and/or figures are labelled with a figure/table number.

## (3) Discussion
In this section, you’ll interpret the results you obtained in the previous section with respect to the main question/goal of your project.

- Summarize what you found and the implications/impact of your findings.
- If relevant, discuss whether your results were what you expected to find.
- Discuss how your model could be improved;
- Discuss future questions/research this study could lead to.

## (4) References
At least two citations of literature relevant to the project. The citation format is your choice – just be consistent. Make sure to cite the source of your data as well.