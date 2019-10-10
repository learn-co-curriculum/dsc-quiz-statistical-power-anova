# Statistical Power and ANOVA

While we recommend using Python to find the answers to these questions, it is not required. You are more than welcome to use a calculator or pencil and paper to solve them, too.

???

# Quiz - Statistical Power and ANOVA

?: You want to determine the number of observations `n` needed to detect an effect size of 0.3 given a Type I error rate of 0.05 and a Type II error rate of 0.1 when performing an unpaired two-sample t-test. 

You've been provided with incomplete code below to determine `n`.

```python
from statsmodels.stats.power import TTestPower, TTestIndPower
power_analysis = _ _ _
n = power_analysis.solve_power(effect_size=0.3, power=_ _ _, alpha = _ _ _) 
```

Select the answer below that fills in the three blanks, in order, with the correct answer.

( ) TTestIndPower(),  0.1, 0.05 

( ) TTestPower(), 0.9, 0.05 

( ) TTestIndPower(), 0.95, 0.1 

(X) TTestIndPower(), 0.9, 0.05 

?: Which of the following are true statements?

[X] The power of a statistical test increases as the sample size increases, given the same $\alpha$ and effect size.

[ ] The power of a statistical test increases as the effect size decreases, given the same $\alpha$ and sample size.

[X] The power of a statistical test increases as the significance threshold $\alpha$ increases, given the same sample size and effect size. 

[X] The power of a statistical test increases as the effect size increases, given the same sample size and $\alpha$. 


?: Question 3

( ) choice 

( ) choice 

( ) choice 

( ) choice


?: Question 4

( ) choice 

( ) choice 

( ) choice 

( ) choice


?: Question 5

( ) choice 

( ) choice 

( ) choice 

( ) choice