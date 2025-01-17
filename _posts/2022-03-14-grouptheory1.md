---
title: 군(group)의 기초 개념
categories: 
- Algebra
tags:
- group theory
- magma
- semi-group
- monoid
- group
- algebraic structure

date: 2022-03-14 10:54:00
---

# Magma $\supset$ Semigroup $\supset$ Monoid $\supset$ Group / Field

## 마그마(Magma)는 어떤 연산에 대해 닫혀있는 집합

- 즉 임의의 이항연산이 부여된 대수구조

## 반군(半群 : semigroup)

- 결합법칙(associativity)을 따르는 이항연산에 대해 닫힌 집합/대수구조

    - 따라서 연산을 두 번 이상 연속적으로 수행할 때 <br> 그 순서를 표시하는 괄호가 불필요하다.

    - $Semigroup \subset Magma$

## 모노이드(monoid)

- 항등원을 갖는, 결합 법칙을 따르는 이항연산 갖춘 대수구조    

    - 반군의 정의에서 항등원의 존재를 추가

    - $Monoid \subset Semigroup \subset Magma$

- 예 1 : $<\mathbf{N}, +>$

- 예 2 : $<\mathbf{Z}, \;\times>$

- 예 3 : N차원 실수 정방행렬(square matrix) 집합과 행렬곱

    - 행렬곱은 교환법칙은 성립하지 않으나 결합법칙은 성립

    - 항등행렬 $I$ 존재하나, 모든 행렬이 가역인 것은 아니다

## 군(group)

- 역원 가지는 모노이드 = 항등원과 역원 가지는 반군

    - 즉 역원과 항등원이 존재하고 결합법칙이 성립하는 연산구조 

    - $Group \subset Monoid \subset Semigroup \subset Magma$

    - 교환법칙까지 성립하면 아벨군(Abelian group)이라고 함

- 예 1 : 2차원 실수 가역(invertible) 정방행렬 집합과 행렬곱

    - 항등원 : 항등행렬 $\;I$

    - 역원 : 역행렬

- 예 2 : $<\mathbf{Z}, +>$

    - 항등원 : 0

    - 역원 : $\;-1$ 을 곱한 값

## 체(field)

더하기와 곱하기 성격의 두 종류 연산이 잘 구비된 집합/대수구조
- 즉 사칙연산이 잘 정의된 집합
    - 빼기는 더하기의 역원
    - 나누기는 곱셈의 역원

- 예 : 유리수집합, 실수집합, 복소수집합

### < 어떤 집합 $F$ 가 체가 되기 위한 10가지 조건 >

#### 0. (F) 집합 $\;F\;$ 위에 덧셈과 곱셈이 정의되어 있다.

#### 1. (A1) 덧셈에 대해 교환법칙이 성립한다.

#### 2. (A2) 덧셈에 대해 결합법칙이 성립한다.

#### 3. (A3) 덧셈의 항등원 $\;0$ 이 존재한다.

#### 4. (A4) $F$의 모든 원소 $\;a$ 에 대해 역원 $\;-a$ 가 존재한다.

-  따라서 뺄셈도 항상 가능하다.

#### 5. (M1) 곱셈에 대해 교환법칙이 성립한다.

#### 6. (M2) 곱셈에 대해 결합법칙이 성립한다.

#### 7. (M3) 곱셈의 항등원 $\;1$ 이 존재한다.

#### 8. (M4) $F$ 의 $\;0$ 아닌 모든 원소 $\;a$ 에 대해 역원 $\;a^{-1}$ 가 존재한다.

- 따라서 $\;0$ 이외의 수로는 항상 나누기를 할 수 있다.

#### 9. (D) 덧셈과 곱셈에 대해 좌우 분배법칙이 모두 성립한다.

<br>

---

### <이항연산 대수 구조의 정리>

---

| 성질 | Magma | Semigroup | Monoid | Group | Field |
|:---|:---|:---|:---|:---|---|
| 연산에 닫혀있다 | O | O | O | O | O |
| 결합법칙 성립 | X | O | O | O | O |
| 항등원 존재 | X | X | O | O | O |
| 모든 역원 존재 | X | X | X | O | O |
| 두 연산($+$, $\times$) | X | X | X | X | O |
| 분배법칙 성립 | X | X | X | X | O |
