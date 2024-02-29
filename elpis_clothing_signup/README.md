# Elpis Clothing Signup
## Problem
The appearance of a website's form is crucial in promoting customer experience, especially for eCommerce businesses. Elpis Clothing, a new eCommerce clothing brand, is focused on optimizing user experience for their pre-launch page. They are currently assessing the effectiveness of their pre-launch page by collecting emails from site visitors. The primary goal is to gather as many emails as possible in preparation for the website launch.

## Approach
To assess the effectiveness of our pre-launch page, my approach involves conducting an A/B experiment comparing two versions of the email sign-up feature:

* Control: This version features a blue submit button, representing the current design.
* Treatment: In this variation, we've introduced a green submit button as an alternative.

By analyzing user engagement and sign-up rates for both versions, my aim is to understand which design resonates better with our audience and generates more email sign-ups. This approach can help us optimize the pre-launch page for maximum effectiveness.

## Conduct AB Testing
1. Explore data 
2. Fomulate Hypothesis:
*  Set hypothesis parameters, including significance level (alpha), statistical power, and minimum detectable effect (MDE):
    * Ho: The sign-up rates of blue and green buttons are the same.
    * Ha: The sign-up rates of blue and green buttons are different.
3. Design Experiment:
* Determine the randomization unit, calculating the sample size and determining the experiment duration
4. Run Experiment and Visualization
* Collect data on control and treatment sign-up counts, sign-up rates, and sample sizes
5. Assess Validity Threats:
    * Perform AA test to ensure that there is no underlying difference between the control and treatment to begin with
    * Perform Chi-Square test on group sizes to check for sample-ratio mismatch (SRM). This test ensures that the randomization algorithm worked
6. Conduct Statistical Inference
* Apply statistical tests on the email sign-up AB test, including Chi-Squared Test and T-Test.
7. Compute Results with Confidence Interval

## Results
* From the test, we observed an improvement of 12.8% lift from the benchmark (blue) at 9.6%. The result was statistically significant with a 95% confidence interval between 5.7% and 19.9%.

* Given that we observed practical and statistical significance, our recommendation is to launch the new submit button in green.

# Usage

## Installation
To use this project, ensure you have the following libraries installed:
* Pandas
* Numpy
* Seaborn
* Matplotlib
* statsmodels

You can install these libraries using pip, Python's package manager. Here's the command to install them:

!pip install pandas numpy seaborn matplotlib statsmodels

## Preparing the datasets
* Load the provided data files from the data folder:
    * pretest.csv
    * test.csv

## Running the Code
* Run the provided notebook (elpis_clothing_signup.ipynb) to load data, explore data, conduct AB test, and obtain results. Ensure all dependencies are installed beforehand.