---
title: 재무관리 08 포트폴리오 효과
categories: 
- finance
tags:
- 포트폴리오
- 체계적 위험
- CAPM
- 재무관리
date: 2022-04-12 10:50:20
---

## 재무관리의 지향점 $\Rightarrow$ 가격결정(Pricing)

- 가격과 (기대)수익률은 동일한 개념

  - $\displaystyle P \;=\; \frac{F}{1+r}$

  - $\displaystyle r \;=\; \frac{\;F}{P\;} - 1$

- 즉 하나가 정해지면 나머지도 정해짐

<br>

## 가격결정 : 가치 = 2차원 함수(시간, 위험)

- Value = Function of Time & Risk
  
  - $V = f(T, R)$

<br>

## 위험과 (기대)수익의 관계

- *High Risk High Return*

  - 높은 위험부담이 무조건 높은 수익을 보장하는 것은 아님

  - 평균적으로 높은 수익 기대한다는 것임 $\Rightarrow$ 기대수익

<br>

## 위험의 측정

- 표준편차 = 분산(편차 제곱의 기댓값)의 제곱근

  - 분산 : $\quad \displaystyle Var[X] \;=\; E\left[\left(X - \mu \right)^2\right] \;=\; E\left[X^2\right] - \mu^2 $

  - 단, $\quad \mu \;=\; E[X]$

<br>

## 포트폴리오 수익률 위험의 측정

- 표준편차(분산)
- 단, 잘 분산투자됨(well-diversified)을 전제
- 공분산(상관계수) 개념이 중요함
- 공분산 : $\quad \displaystyle Cov[X,Y] \;=\; E\left[\left(X - \mu_x \right)\left(X - \mu_y \right)\right] \;=\; E\left[XY\right] - \mu_x \mu_y$
- 자기자신과의 공분산이 분산임
  - $Cov[X,X] \;=\; Var[X]$

<br>

## 개별자산 수익률 위험의 측정

- 개별자산 표준편차는 비체계적 위험 포함
- 비체계적 위험은 가격에 반영되지 않음
- $\beta$ : 베타 : 체계적 위험 측정
  - 시장자산에 대한 민감도(기울기)
  - [CAPM 참고](/finance/capm)

<br>

## 참고 1 : 체계적 위험 vs 비체계적 위험

| 비체계적 위험 unsystematic risk | 체계적 위험 systematic risk |
|:---|:---|
| 개별/고유위험 idiosyncratic risk | 시장위험 market risk |
| 분산가능위험 diversifiable risk | 분산불가능위험 non-diversifiable risk |
| 가격 반영 안됨 | 가격에 반영됨 |

<br>

## 참고 2 : 포트폴리오 수익률 분산의 계산

# $$\tilde{r}_p = w_1\tilde{r}_1 + w_2\tilde{r}_2$$

- $\tilde{r}_p$ : 수익률
  - 확률변수로 값을 미리 정할 수 없음 : 값이 확률적으로 정해짐
- $w_i$ : 자산분배비중(가중치)
  - 투자자 자신이 값을 미리 정할 수 있음
- 포트폴리오 수익률은 각 자산 수익률의 가중평균

$E[\tilde{r}_p] = w_1E[\tilde{r}_1] + w_2E[\tilde{r}_2] \; ::: \;\mu_p = w_1\mu_1 + w_2\mu_2$

- 표기를 간단히 하기 위해 기대값을 $\mu$ 로 표기

$Var[\tilde{r}_p] = E[(\tilde{r}_p - \mu_p)^2] \; ::: \;\sigma_p^2$

- 분산은 확률변수의 산포도(분포의 흩어짐의 정도) 측정 개념
- 투자수익률의 변동성(variability) 또는 위험(risk) 측정

$\tilde{r}_p - \mu_p = w_1(\tilde{r}_1 - \mu_1) + w_2(\tilde{r}_2 - \mu_2)$

- 포트폴리오 편차 역시 각 자산 편차의 가중평균임

양변을 제곱하면

$( \tilde{r}_p - \mu_p )^2 = w_1^2 ( \tilde{r}_1 - \mu_1 )^2 +
2w_1w_2 ( \tilde{r}_1 - \mu_1 ) ( \tilde{r}_2 - \mu_2 ) + w_2^2 ( \tilde{r}_2 - \mu_2 )^2$

양변에 기댓값을 취하면

$\sigma_p^2 \; = \; w_1^2\sigma_1^2 +2w_1w_2\sigma_{1,2} + w_2^2\sigma_2^2$

공분산과 상관계수 관계 : $\sigma_{1,2} = \rho\;\sigma_1\sigma_1$

- 상관계수 = 공분산 나누기 표준편차들의 곱
- 공분산 = 상관계수 곱하기 표준편차들의 곱

<br>

# $$ \sigma_p^2 = w_1^2\sigma_1^2 + 2w_1w_2\rho\;\sigma_1\sigma_2 + w_2^2\sigma_2^2 $$

<br>

- 두 자산의 위험(표준편차) 수준이 주어졌을 때

- 그 상관계수가 낮을수록 포트폴리오 분산 작아짐

<br>