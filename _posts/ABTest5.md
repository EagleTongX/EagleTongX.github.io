# A/B Test -- Lesson 5

*Overview*:

Sanity checks

Single Metric

Multiple Metric

Gotchas

**Sanity Checks**:

*choosing Invariant metrics*:

population sizing metrics

actual invariant



data capture 

experiment setup

Infrascture 



**Evaluation**

Goal: see is there a statistically significant result in your experiment, estimate magnitude and the direction of the change, then make decision based on these. 

*Single Evaluation Metric*:



*Simpson's paradox*:

happen when setup has problem or change effect different group differently, 



**Tracking multiple metrics:**

Bonferroni correction*: 

- Very simple
- without any assumption
- Too conserative -- gurantee give $\alpha_{overall}$ at least as small as specified

*Other strategy:*

- control probability that any metrics shows a false positive

  $\alpha_{overall}$ , familywise error rate(FWER)

- control false discovery rate(FDR)  FDR =E [# false positives / # rejections]

  

  

  Recap:

  <u> when looking at the result not just look at significant statistical difference, you are making business decision</u>

  <u>take consideration of the overall business analysis. e.g.  what the engineering cost, customer suppot? Sales issues?</u>

  

  

  

  

  

  