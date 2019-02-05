# Chebyshev's Inequality
When a distribution is Gaussian it follows the 68-95-99.7 rule i.e.
68% of data lie between μ-σ and μ+σ 
95% of data lie between μ-2σ and μ+2σ
99.7% of data lie between μ-3σ and μ+3σ

What if we don’t know a distribution is Gaussian or not?
But we know that the mean is finite and standard deviation is non-zero infinite
Suppose,
X% of data lies within μ-2σ and μ+2σ
Y% of data lies within μ-1.5σ and μ+1.5σ
Z% of data lies within μ-1σ and μ+1σ... How should we find the ranges in this kind of distribution?

Suppose if we want to calculate salary of Individuals and we know mean=40K and std dev=10K
Ques1-What % of individuals have salary in the range of [20K,60K]?
observation-It is in the 2sigma range
Ques2- What % of individuals have salary in the range of [10K,70K]?
observation-It is in the 3sigma range
Chebyshev’s Inequality states-
P(|X-μ| >= k*σ) <= 1/k^2
or
P(μ-k*σ < X < μ-k*σ) > 1- 1/k^2     
Ans1- 
P(40K-2*10K < X < 40K+2*10K)> 1-1/4
P(20K < X < 60K) > 0.75
This implies atleast 75% of the people have salaries between 20K to 60K

Ans2-
P(40K-3*10K < X < 40K+ 3*10K) > 1-1/9
P(10K < 70K) > 8/9
P(10K < 70K) > 88.888
This implies approx 90% of the people have salaries between 10K to 70K
