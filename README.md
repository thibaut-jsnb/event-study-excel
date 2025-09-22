# event-study-excel

In this event study, I examined the impact of earnings announcements on stock returns.  

First, I estimated the **market model**:  

\[
R_{i,t} = \alpha_i + \beta_i R_{m,t} + \varepsilon_{i,t}
\]

where:  
- \(R_{i,t}\) is the stock return,  
- \(R_{m,t}\) is the market return,  
- \(\alpha_i, \beta_i\) are the regression parameters.  

This regression allowed me to obtain the expected relationship between the stock and the market.  

Then, I computed the **expected return** during the event window:  

\[
\hat{R}_{i,t} = \hat{\alpha}_i + \hat{\beta}_i R_{m,t}
\]

I measured the **abnormal returns (AR)** as the difference between actual and expected returns:  

\[
AR_{i,t} = R_{i,t} - \hat{R}_{i,t}
\]

I aggregated them over time to obtain the **cumulative abnormal return (CAR)**:  

\[
CAR = \sum_{t=T_1}^{T_2} AR_{i,t}
\]

Finally, I applied **t-tests** to the AR and CAR to check whether they were significantly different from zero.  

- If the t-statistic was close to zero (\(|t| < 1.96\) at 5% level), the event had no significant effect.  
- If \(|t|\) was larger, the event generated a **statistically significant market reaction**.  

The results (columns *“Test T CAR”* in the Excel file) showed that some events did trigger **significant abnormal performance**, while others did not — confirming heterogeneous market reactions to earnings announcements.
