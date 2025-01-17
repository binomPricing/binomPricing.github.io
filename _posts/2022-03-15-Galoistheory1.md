---
title: 대칭-갈루아이론(신현용, 신기철)
categories: 
- Algebra
tags:
- group theory
- Galois theory
- algebraic structure
- 군론
- 갈루아 이론
- 대수적 구조
- magma
- monoid
- semigroup
- group
- field
date: 2022-03-15 10:54:00
---

### 대수학(algebra)은 다항식의 풀이에 관한 연구

- 대수학의 주제가 1차, 2차, 3차, 4차 방정식 풀이라면,

- 추상대수학(abstract algebra) 또는 현대대수학(modern algebra)

    - 주제는 오차다항식 풀이

### 다항식의 근의 공식이 존재한다는 말과 같은 뜻

- 다항식을 풀 수 있다

- 다항식을 거듭제곱근(radicals)을 사용해 풀 수 있다

- 가해(可解 : solvable, soluble) 다항식이다

### 참고 : 근의 공식이 없다고 근이 없는 것은 아니다

- 대수학의 근본정리(Fundamental Theorem of Algebra) 

    - 복소수 범위에서 n 차 방정식은 n 개(중근 포함)의 해가 있다

- 요지는 **유리수계수를 가지는 오차 이상 다항식**에 대해 <br> **일반화된 근의 공식을 구할 수 없다**는 것이다

    - 일부 고차방정식은 근을 구하는 방법이 있다

        - 예 : $x^5 - 2 = 0$ 등 특수한 형태의 방정식은 풀이법이 존재함

### 아벨과 갈루아의 업적

- 오차이상 다항식을 풀 수 없음을 증명

- 이를 이해하기 위해 대수적 구조를 알아야

### 대수적 구조(algebraic structure)

- 집합 + 수학적 구조

    - 두 원소 사이에 정의되는 연산(operation)의 성질

    - 결합법칙, 교환법칙, 분배법칙, 항등원/역원의 존재

- 예 : 군(group), 체(field), 벡터공간(vector space)
    
<br>

# Magma $\supset$ Semigroup $\supset$ Monoid $\supset$ Group $\supset$ Field

- [대수학 기초 참조](https://binompricing.github.io/algebra/grouptheory1)

### < 이항연산 대수 구조의 정리 >

---

| 성질 | Magma | Semigroup | Monoid | Group | Field |
|:---|:---:|:---:|:---:|:---:|---:|
| 연산에 닫혀있다 | O | O | O | O | O |
| 결합법칙 성립 | X | O | O | O | O |
| 항등원 존재 | X | X | O | O | O |
| 모든 역원 존재 | X | X | X | O | O |
| 두 연산($+$, $\times$) | X | X | X | X | O |
| 분배법칙 성립 | X | X | X | X | O |

<br>
