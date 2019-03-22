# A/B Test -- Lesson 4

*Overview*:

choose subject

choose population

Size

Duration



**Choose the subject**

*Unit of diversion* :

how we define an indivisual subject in the experiment

Commonly use: 

- User id: stable, unchanging, personally identifiable

- Anaoymous id (cookie): change when you switch browser or device, user can clear cookies 

- Event:  no consistent experience, use only for non-user-visible changes

  not common: IP address

*Consideration for choosing diversion?*

1. User consistency (for user visible change, use useid or cookie)

   you need to consider if the change user visible or not, yo ualso need to consider what you want to measure

2. Ethical considerations: depends on what data being collected and which diversion you use

3. Variability 

*Unit of Analysis vs. Unit of diversion*

Unit of analysis is the denominator or your metric. e.g. in CTR, clicks/pageviews, pageview is unit of analysis

when unit of analysis = unit of diversion, variability tends to be lower and closer to analytical estimate, which means analytic variance are more likely to match empirical variance. 

**Choose of population**

*Intra-user Experiments*:

expose the same user to this feature being on and of over time, and analyze how they behave in different time windows.

*Interleaved Expeiments:*

expose the same user to the A and B side at the same time.

*Inter-user Experiments*:

get different people in the A side and B side 

*Target of population*:



*Population vs. Cohort*:

*when to use cohort*:

1. looking for learning effect
2. examing user retentionn
3. increase user activity

4. anything require user to be established

Using cohort limit your experiment to a subset of the population, which can affect variability. 

**Experiment Design and Sizing**

Sizing : ?



**Duration vs. Exposure**



Unit of analysis is the denominator of your metric, that is, the N to calculate the standard deviation of your metric. 





