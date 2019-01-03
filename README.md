# reference-code-experimental-design

First, a link to a helpful blog article: [Which hypothesis test to perform?](https://towardsdatascience.com/which-hypothesis-test-to-perform-89d7044d34a1)


### Content of conceptual notebooks

1) **Statistical Significance Testing:** Demonstrate different forms of statistical tests on recorded metrics of a hypothetical A/B test to see if there is a statistical difference between the two groups. Key content:
    - proper setup with testing of invariant metric and evaluation metric
    - difference between analytic and simulation-based approaches

2) **Experiment Sizing:** Demonstrate how to use the knowledge of the desired practical significance boundary to plan out an experiment. Demo of analytic approach and discussion of alternative approaches

3) **Non-parametric tests:** Demonstrate alternative approaches to standard hypothesis tests to analyze experiments. Standard hypothesis tests rely on means of normal distributions. But there may be scenarios where there is uncertainty about the true variability of a metric's distribution, a lack of data to assume normality, or you want to do inference on a statistic that lacks a standard test. 

Non-parametric tests are not just as a workaround for cases like this, but also as a second check on experimental results. The main benefit of non-parametric tests is that they don't rely on many assumptions of the underlying population, and so can be used in a wider range of circumstances compared to standard tests.
Tests covered in this notebook:
    - based on resampling
        - Bootstrapping
        - Permutation
    - without bootstrapping
        - Rank-Sum-Test
        - Sign-Test

4) **Early Stopping:** Demonstrate that when you peek at the results of an experiment before data collection is complete, and choose to stop early because the test is showing statistical significance, you run the risk of a significant increase in your Type I error rate.


### Content of mini-projects / examples

**Example T-test Stroop:** Very small project. The objective is to demonstrate hypothesis testing based on observations regarding the so called Stroop Effect. A paired / dependent 2-sample-t-test is used for the hypothesis testing.

**Examples A/B-Testing Web:** Demonstrate and test some functions I have written for hypothesis testing, especially with A/B-tests (on proportions). The custom function files can be found in the codebook folder / repository.


### Install

This project requires **Python 3.x** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [Scipy](https://docs.scipy.org/doc/scipy/reference/index.html)
- [matplotlib](http://matplotlib.org/)
- [seaborn](http://seaborn.org)

You will also need the custom file `hypothesis_functions`that can be found in my `codebook`repository.

You will also need to have software installed to run and execute an [iPython Notebook](http://ipython.org/notebook.html)