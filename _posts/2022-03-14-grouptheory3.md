---
title: 군(group)의 기초 개념 3
categories: 
- Algebra
tags:
- 동형 사상
- isomorphism
- automorphism
- 자기동형사상
- automorphism
date: 2022-03-14 10:54:30
---

## 1. 체의 동형(isomorphic)

- 두 체 $K$ 와 $K'$ 에 대해

- 동형사상이 존재하면 **동형** 이라고 한다.

## 동형 사상(同型寫像 : isomorphism)

- 사상(mapping) $f : K \rightarrow K'$ 가 일대일대응이고  

- $K$ 의 임의의 원소 $x, y$ 에 대해서  

    - $f(x+y) = f(x) + f(y)$ 이고

    - $f(xy) = f(x)f(y)$ 이면  

- 사상 $f$ 를 **동형사상** 이라고 한다.


## 자기 동형 사상(自己同型寫像 : automorphism)

- 앞에서 $K = K'$ 일 때 $f$ 를 **자기동형사상** 이라고 한다.

### 직관적 설명
- 동형사상은 두 집합의 사칙연산구조를 보존하는 함수이고
- 동형 집합은 사칙연산 관점에서 본질적으로 같은 집합이다.

<br>

## 2. 체의 확대

### 대수적 확대체(algebraic extention field)

- 유리계수 방정식 해가 되는 수를 대수적 수(代數的數 : algebraic number)

- 대수적 수가 아닌 복소수를 초월수((超越數 : transcendental number)

- 예 : 유리체 $Q$ 에 무리수 일부를 추가한 체

#### $Q(\sqrt{2}) = \\{ a+b\sqrt{2} \;:\; a, b \in Q \\}$

#### $Q(\sqrt{2}, \sqrt{3}) = \\{ a+b\sqrt{2}+c\sqrt{3} \;:\; a, b, c \in Q \\}$

#### $Q(\alpha) : \alpha = \sqrt[3]{2}$

- $Q(\alpha) = \\{ a+b\alpha+c\alpha^2 \;:\; a, b, c \in Q \\}$

- $\alpha$ 의 삼차 이상 다항식은 모두 2차식으로 축소될 수 있다.

#### 일반적으로 $\alpha = \sqrt[n]{p}$ 이면

- $Q(\alpha) = \\{ a_0 + a_1 \alpha + \cdots + a_{n-1} \alpha^{n-1} \;:\; a_k \in Q \\}$

- $\alpha$ 의 $n$ 차 이상 다항식은 모두 $(n-1)$ 차식으로 축소될 수 있다.












