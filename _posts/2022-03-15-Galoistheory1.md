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

### 아벨과 갈루아의 업적

- 오차이상 다항식을 풀 수 없음을 증명

- 이를 이해하기 위해 대수적 구조를 알아야

### 대수적 구조(algebraic structure)
- 집합 + 수학적 구조
    - 두 원소 사이에 정의되는 연산(operation)의 성질
    - 결합법칙, 교환법칙, 분배법칙, 항등원/역원의 존재
- 예 : 군(group), 체(field), 벡터공간(vector space)
    
<br>

# Magma $\supset$ Semigroup $\supset$ Monoid <br> $\supset$ Group $\supset$ Field

- [대수학 기초 참조](/algebra/grouptheory1)

### < 이항연산 대수 구조의 정리 >

---

| 성질 | Magma | Semigroup | Monoid | Group | Field |
|:---|:---|:---|:---|:---|---|
| 연산에 닫혀있다 | O | O | O | O | O |
| 결합법칙 성립 | X | O | O | O | O |
| 항등원 존재 | X | X | O | O | O |
| 모든 역원 존재 | X | X | X | O | O |
| 두 연산($+$, $\times$) | X | X | X | X | O |
| 분배법칙 성립 | X | X | X | X | O |

<br>
