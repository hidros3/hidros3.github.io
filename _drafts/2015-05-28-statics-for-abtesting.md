---
layout:     post
title:      ab testing을 위한 통계
date:       2015-05-28 23:00:00
summary:    ab testing을 진행하는데 필요한 통계 지식에 대하여
tags: ab testing, statics
---

## Sample Size

예를 들어 기존 A안의 Conversion Rate가 4%고 B안을 목표를 4.5%라고 했을 때, difference 0.004가 의미하는 것은 B가 4.1%에서 4.9%까지 분포한다는 것이다. B안의 최소값이 4.1%일 때 그래도 A인 4%보다 크기 때문이다. 이럴 때 필요한 샘플 수는 다음과 같다.

```R
estimate <- function(targetRate,difference,errorProb) {
    ceiling(-log(errorProb)*targetRate/(difference^2))
}
est <- estimate(0.045,0.004,0.05)
print(est)
## [1] 8426
```
