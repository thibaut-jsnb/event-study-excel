# event-study-excel

In this event study, I examined the impact of earnings announcements on stock returns.

First, I estimated the market model:

Model:
Ri,t = αi + βi · Rm,t + εi,t

where:

Ri,t is the stock return,

Rm,t is the market return,

αi and βi are the regression parameters.

Then, I computed the expected return during the event window:

R̂i,t = α̂i + β̂i · Rm,t

I measured the abnormal returns (AR) as:

ARi,t = Ri,t − R̂i,t

I aggregated them over time to obtain the cumulative abnormal return (CAR):

CAR = Σ (from t = T1 to T2) ARi,t

Finally, I applied t-tests to the AR and CAR to check whether they were significantly different from zero.

If the t-statistic was close to zero (|t| < 1.96 at the 5% level), the event had no significant effect.

If |t| was larger, the event generated a statistically significant market reaction.

The results (columns “Test T CAR” in the Excel file) showed that some events did trigger significant abnormal performance, while others did not. That is confirming heterogeneous market reactions to earnings announcements.
