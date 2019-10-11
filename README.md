# Statistical Power and ANOVA

While we recommend using Python to find the answers to these questions, it is not required. You are more than welcome to use a calculator or pencil and paper to solve them, too.

???

# Quiz - Statistical Power and ANOVA

?: You want to determine the number of observations `n` needed to detect an effect size of 0.3 given a Type I error rate of 0.05 and a Type II error rate of 0.1 when performing an unpaired two-sample t-test. You've been provided with incomplete code below to determine `n`.

```python
from statsmodels.stats.power import TTestPower, TTestIndPower
power_analysis = ___
n = power_analysis.solve_power(effect_size=0.3, power=___, alpha = ___) 
```

Select the answer below that fills in the three blanks, in order, with the correct answer.

( ) `TTestIndPower()`,  `0.1`, `0.05` 

( ) `TTestPower()`, `0.9`, `0.05` 

( ) `TTestIndPower()`, `0.95`, `0.1` 

(X) `TTestIndPower()`, `0.9`, `0.05` 

?: Which of the following are true statements?

[X] The power of a statistical test increases as the sample size increases, given the same $\alpha$ and effect size.

[ ] The power of a statistical test increases as the effect size decreases, given the same $\alpha$ and sample size.

[X] The power of a statistical test increases as the significance threshold $\alpha$ increases, given the same sample size and effect size. 

[X] The power of a statistical test increases as the effect size increases, given the same sample size and $\alpha$. 


?: You are performing 20 statistical tests simultaneously, and have set a signficance threshold of $\alpha = 0.05$ to reject the null hypothesis. What is the Bonferroni-corrected significance threshold you should use to control for Type I errors? 

( ) 0.05  

( ) 0.01 

( ) 0.005 

(X) 0.0025


?: We want to compare the means of two independent samples of unequal size. What kind of test do we need to perform?

( ) One-sample t-test

( ) Paired two-sample t-test

( ) Unpaired two-sample t-test

(X) Welch's t-test


?: You're trying to test different ways of brewing espresso and want to assess the influence of brewing temperature, `tempC`, and brewing pressure, `prssBar`, on the espresso foam index, a measure of espresso foam quality. In your experiment, there are three  possible different brewing temperatures and two possible different brewing pressures. You use Python and `statsmodels` to generate an ANOVA table and obtain the following result: 

![ANOVA table](images/anova_table.png | width = 500)

Select all features that had a significant effect at $\alpha = 0.01$ on the espresso foam index according to your results. 

[X] `tempC` had a significant effect on the espresso foam index.

[X] `prssBar` had a significant effect on the espresso foam index.

[ ] No features had a significant effect on the espresso foam index. 


???