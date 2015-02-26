---
layout:     post
title:      Think Stats
date:       2015-02-24 13:16:00
summary: I'm currently reading Chap2. of Think Stats by Allen B. Downey. I summarized something that I marked. Chap2 is about distributions. 
categories: book, python, data science
---
## chap 2. Distributions

### Keywords
몇 가지 중요한 키워드를 정리하였다.

#### histogram
* plotting histograms
* normal distribution, Gaussian distribution
* outliers

#### Summarizing Distributions
* central tendency
* modes
* spread
* tails
* outliers
* mean vs average

#### Variance
* S^2 = variance
* S = standard deviation
* mean()
* var()
* std()

#### Effective Size
* Cohen's d
* d = x1 - x2 / s
	* pooled standard deviation, s
	* s = n1 * var1 + n2 * var2 / (n1 + n2)
	* s = sqrt((n1 - 1) * var1 + (n2 - 1) * var2 / (n1 + n2 -2))

Cohen's d로 샘플 사이즈 수가 충분한지 확인할 수 있다. d 값에 따라 CI 수준을 확인할 수 있다. 예를 들어 d = 1.72인 경우, 95% CI는 1.66~1.78 이므로 충분히 크고 값의 차이를 확인하는데 충분한 크기임을 알 수 있다.

**[위키 중 일부](http://en.wikipedia.org/wiki/Effect_size#Cohen.27s_d)**

> Cohen's d is frequently used in estimating sample sizes for statistical testing. A lower Cohen's d indicates the necessity of larger sample sizes, and vice versa, as can subsequently be determined together with the additional parameters of desired significance level and statistical power.

#### Reporting Results
* We have seen several ways to describe the difference.
* The answer depends on who is asking the question.
* **You should design statical reports and visualizations that tell a story clearly.**

결과를 리포트하기 전에 무엇을 설명하고 어떻게 보여줘야할지 미리 디자인 해야한다는 뭔가 당연한 듯한 이야기. 월스트리트저널 인포그래픽 가이드를 읽어야 하나.
