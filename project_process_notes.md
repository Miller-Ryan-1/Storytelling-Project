Y-axis is customers
X-axis is months, normalized
two lines plotted - total and churned, which always < total
Total(n) = Total(n-1) + (1- churn(n))
n@tmax, total should equal total records / sum churned 

1.  Problem: Churn
a) Total percent of all people, who were ever customers, churned
b) Some comparative value
c) I used a comp bridge: I normalized all records to the same starting month, and graphed (and measured) each months total active (count of month's records * (1-churn), and total churned (count of months records * (churn))
Then I made that a running 12 month average, to balance out the inconsistencies.  That I compare to this stat that I found here {url:stat}. 
THUS) we see that churn is in fact a problem, with the variauable of interest being churn

2. Valuation of the Problem (in other words, the everity): 
a) I sought to find a way to give a quantitavite measure of the average lost potential revenue per customer, as from a businee perspective, that is part of the problem - just how bad is it.  This allows stakeholders to make their own judegemenmts with the best information available for thise particular decicions.  Help them by knowing how to optimize what data they need to make an informed decision.
b) -->To do this I took the difference between the length of a churned and non churned customer (20 months) and then pricing that at the average customer monthly revenue.  So just trying to use general statistics to get quick analysis. This equaled around $1200 per customer and thereofre a total of $xxM to the firm.  It's a problem.

3.  Now I want to know more about, and try to really pinpoint, the variables that affect the variable of interest.  In this case churn.
a) First looked at the general temporeal trend - how is it changing in time.  Most customer xhurn in the first month (70% of all who churn) it then decreases, although somewhat randomly (goes up and down but generla trend is negative).
b) Now removing time from the analysis, I looked at over that whole time what drove the most incidents or churn.  Did this by just throwing the other variables at churn and seeing how chrun was affected.  Old, partners, seniors, etc.  Most had little effect.  But I saw that it was electronic checks, and in particular fiber {using the two charts} that had the biggest impacts.
c) I went back and did another time analysis to see how these different services and payment methods changed over time (as in, does it match the general trend)
d) So at the end of this I can identify the greatest drivers of churn by raw numbers, and if these wre time dependant at all (which then makes the bulk analysis less useful) *call this concept of analyzing data holding time constant on one hand (bulk analysis) with analyzing data over time (temporal analysis).  The less the variables vary with time, the closer the relationship of indpendance between the bulk and temporal properties.  THE BEST MODEL IS THE ONE WITH THE MOST INDEPENDANT TEMPORAL AND BULK VARIABLES.  The equation is:
target_variable_impact_score = 
in this case,
churn_impact_score = bulk_factor * temporal_factor * (factor that is related to the indpendance of bulk_factor and temporal_factor, which can be shown but how each of the bulk variables impacts changes the same with time, even if some of the are clealy huge impacts). max_churn_impact_score = ( (bulk_factor * temporal factor) * COR(factors) ) / (bulk_factor * temporal factor), closer to 1 more impactful compared to all other metrics.
COR(factors) is how dependant, and therefore how each effects the other.  This is actually two components: some  specific measurement of correlation between two variables (This algorithmic equation needs some more thought, but I think it is very easy to figure out) and then some other factor that is a PDE? that changeds in response to the correlation level and which is optimaize when this entire clause is closest two 1 - means comopletely independant.
Thus, the number is optimized at 1 (total independant), it is the maximum because and change positive or negative from it leads to a suboptimal outcome.

4.  Now I can give an estimated value of what can be recovered (the ideal case)
The estimated value is the difference between the status quo and the idealized situation which is when the correlation clause = 1.  Otherwise it has a unique value for each month that all variables should changed with in perfect unison to oen another - aka the variables with the max_churn_impact_score

5.  Lastly, I proppose a qualitative solution based on the data to get to that optimal situation.
If by removing x as a payment option, or y as the service option, or  as any composite set of variables, 
*SO you need a tool that can determine, automagically, the optimal set of variables.  Anyway, without going there, I said we feel you can reduce that churn by taking these actions (and if they ask, yes you can back it up with data and analysis)

6. So, in sum, using an identified target variable (given by the executives - churn) we first identifed if it was in fact a problem, then give a valuation to define the magnitude of the problem.  Next I do my bulk and tempoeral analysis against the target variable, and identify the overall most impacct variables.  Lastly, we proposed a changed and value created by that change.

Target variable = churn
target variable goal value = industry standard for good (x% per time period) equivalent
variables can be lumped together and normalizee to time in a bulk analysis,
they can then be compared against one another and overall impact
optimized value can then be found based on the goal you target (in this case, the industry standard)

