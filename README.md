# Chebyshev-s-Inequality
When a distribution is Gaussian it follows the 68-95-99.7 rule i.e.
68% of data lie between u-sigma and u+sigma 
95% of data lie between u-2sigma and u+2sigma
99.7% of data lie between u-3sigma and u+3 sigma

What if we don’t know a distribution is Gaussian or not?
But we know that the mean is finite and standard deviation is non-zero infinite
X% of data lies within u-2sigma and u+2sigma
Y% of data lies within u-1.5sigma and u+1.5sigma
Z% of data lies within u-1sigma and u+1sigma

Suppose if we want to calculate salary of Individuals and we know mean=40K and std dev=10K
Ques1-What % of individuals have salary in the range of [20K,60K]?
observation-It is in the 2sigma range
Ques2- What % of individuals have salary in the range of [10K,70K]?
observation-It is in the 3sigma range
Chebyshev’s Inequality states-
P(|X-u| >= k*sigma) <= 1/K^2
or
P(u-k*sigma < X <u+k*sigma) > 1- 1/k^2     
Ans1- 
P(40k-2*10K < X < 40K+2*10K)> 1-1/4
P(20K < X < 60K) > 0.75
This implies atleast 75% of the people have salaries between 20K to 60K

Ans2-
P(40K-3*10K < X < 40K+ 3*10K) > 1-1/9
P(10K < 70K) > 8/9
P(10K < 70K) > 88.888
This implies approx 90% of the people have salaries between 10K to 70K
