# A/B Test -- Lesson 3

**Metric Definition**

Before define the metric: what you are going to use the matrics for?

Step:

1. Have one sentence easily understand summary. e.g. "active user"
2. Figure out all details about the metrics. e.g how do you define active is ?
3. Take all the individual data measurement to summarize a single metric.
4.  Think how general applicable the metric is.

![image-20190314221322465](/Users/tongxin/Library/Application Support/typora-user-images/image-20190314221322465.png)



*How to gather additional data*

- User Experience Research (UER) + good for brainstroming + special equipment

- Focus groups + get feedback on hypotheticals - run the risk of group think

- Surveys: useful for metrics you can't directly measure yourself

  (Be careful about the survey result, can't directly compare to other results)



Retrospective analysis:  establish correlation



**Define a metric**

High-level metric: click-through-probability = #users who click / #users who visit

Def #1(cookie probability):  For each [time interval],  #cookies that click/#cookies

Def #2(pageview probability):  # pageview with a click within [time interval] /#pageviews

Def #3(Rate): #clicks/ #pageviews 

***Categories of summary metrics***:

- Sums and counts. e.g. #users who visited page
- Means, medians and percentiles. e.g. median latency of page load
- Probabilities and rates. e.g. probability has 0 or 1 outcome in each case, rate has 0 or more.
- Ratios. Any two numbers divied by each other. e.g. P(revenue-generating click)/P(any clicks)

**Measure sensitivity and robustness**

e.g. Choose summary metric for latency of a video

Do retrospectivce analysis

**Calculating Variability**

To calculate a confidence interval you need: 

- Variance(standard deviation)
- Distribution



| Type of metric     | Distribution       | Estimated variance     |
| ------------------ | ------------------ | ---------------------- |
| Probability        | Binorminal(normal) | $\hat{p}(1-\hat{p})/N$ |
| Mean               | Normal             | ${\hat\sigma}^2/N $    |
| Median/Perscentile | Depends            | Depends                |
| Count/difference   | Normal(maybe)      | Var(x) + Var(y)        |
| Rates              | Poisson            | $\bar{x}$              |
| Ratios             | Depends            | Depends                |

E.g. Calculate confidence interval of mean:

Measure: Mean number of homepage visit per week

$N_1$ ~ $N_7$  mean number of homepage visit per week

$\bar{N}$ = $N_1+....+N_7$ 

$\sigma$ = SD($N_1....N_7$) Standard Deviation 

SE = $SD/\sqrt{N}$  Standard Error

Margin of error = z score * SE (for normal distribution)

***A/A Test***:

Usecase: 

- Compare results to what you expect(sanity check)
- Estimate variance and calculate  confidence interval
- Directly estimate confidence interval

*Summary*:

We need to understand the distribution of the underlying data to compute variability



