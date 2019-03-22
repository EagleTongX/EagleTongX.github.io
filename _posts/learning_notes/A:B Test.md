# A/B Test -- Lesson 1

***Overview***:

- Choose a metric
- Review statistics
- Design
- Analyze

**What A/B test can**:



**What A/B test can't**:

- Not useful for new experiences

Depends on two question: 

1. What's your baseline for comparison?

2. How much time you need in order for your user to adapt new experience?

<u>A/B Test can't really tell you if you're missing something</u>

<u>Clear control and clear metrics</u>

**Other Techniques**:

Focus group

User research

User experience study:

You can have a consistent response from your control and your experiment group to determine and structure the experiment 



*Goal of A/B Testing*: design an experiment that is going to be robust and give you repeatable results so that you can actually make a good decision to whether lunch the new product or feature or not.



*Metrics for website*:

- total number of course/task completed
- number of clicks 
- Click-through-rate:  number of clicks/ number of page views
- Click-through-probability: unique visitors who click/unique visitors to page

*How to decide which metric to use?*

Click-through-rate: when you want to measure the usability

Click-through-probability: when you want to measure the total impact. e.g. whether users are progressing to the second level of funnel

*When can you use binomial distribution?*

1. 2 type of outcomes
2. Independent events
3. Identical distribution: P same for all

*Confidence Interval*:

The center of confidence interval

The margin of error = Z-score (of confidence level) * standard error

In binomial distribution, the standard error is : $\sqrt{p(1-p)/N}$



**Hypothesis Testing**

Null Hypothesis($H_{0}$) : $Pcontrol$ = $Pexperiment$

Alternative Hypothesis($H_{A}​$): $Pexperiment​$ != $Pcontrol​$

Measure $$\hat{P}cont $$ and  $\hat{P}exp$

 Calculate $$P(\hat{P}exp - \hat{P}cont|H_{0})$$  and compare with the cutoff($\alpha$), if less than $\alpha$ , then reject null

*How to compare two samples?*

Calculate pooled standard error:

X: number of action  N: total number

$X_{cont}$ $X_{exp}$   $N_{cont}$  $N_{exp}​$

$\hat{P}_{pool} = (X_{cont} + X_{exp})/(N_{cont}+N_{exp})$

SE$_{pool}$ = $\sqrt{\hat{P_{pool}*(1-\hat{P}_{pool})* (1/N_{cont} + 1/N_{exp})}}$

$\hat{d} = \hat{P}_{exp} - \hat{P}_{cont}$

In H$_{0}​$: d = 0  $\hat{d} ​$ ~ N(0, $SE_{pool}​$)   follow normal distribution

If $\hat{d}$ > Zscore * $SE_{pool}$ or $\hat{d}$ < - Zscore * $SE_{pool}$, reject Null hypothesis

**Pick up Practical significant**

*Determine the sample size*:

Sample size determined by:

1. your baseline conversion rate
2. the absolute minimum detectable effect(MDE/$d_{min}$) you pick. this is the minimum difference between control and experiment conversion rates you will be able to detect.
3. $\alpha$ : by default keep it as 95%
4. $\beta$ : by default keep is as 20%

*How to choose how many page views?*

$\alpha$ = P(reject null | null  True)​

$\beta$ = P(fail to reject | null False)

small sample: $\alpha$ low, $\beta$ high

large sample: $\alpha$ same, $\beta$ lower

1- $\beta ​$ = sensitivity   often 80%

 **Example**![image-20190314210432013](/Users/tongxin/Library/Application Support/typora-user-images/image-20190314210432013.png)

![image-20190314211352619](/Users/tongxin/Library/Application Support/typora-user-images/image-20190314211352619.png)



*How to make decision when uncertain?*

Communicate to desicion maker, user other factors besides data when data is not certain. 