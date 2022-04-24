---
title: 군론(group theory) 기초
categories: 
- Algebra
tags:
- group theory
- cyclic group
- symmetric group
- dihedral group
- subgroup
- normal subgroup

date: 2022-03-14 10:54:20
---

## 군(group)의 정의

다음 조건을 만족하는 "공집합 아닌 집합(G)"을 군이라 한다.

1) 어떤 연산($\cdot$)에 대해 닫혀있다

- $x, y \in G \Rightarrow x \cdot y \in G$

2) 결합법칙이 성립한다.

- $(x \cdot y) \cdot z = x \cdot (y \cdot z)$

3) 항등원이 존재한다.

- $\exists 1 \in G : 1 \cdot x = x \cdot 1 = x \;\; \forall x \in G$

4) 역원이 존재한다.

- $\exists x^{-1} \in G \;\; \forall x \in G: x^{-1} \cdot x = x \cdot x^{-1} = 1 $

## 군의 전형적인 예

- 회전시키기 : 순환군

- 순서바꾸기 : 대칭군

- 회전+뒤집기 : 정이면체군

### 1) 순환군(循環群 : cyclic group) : $C_n$

- $C_n = \\{ 1, x, x^2, \cdots, x^{n-1} \\} : x^n = 1$

- 간단하게 $C_n = ⟨ x : n ⟩$ 으로 표시할 수 있다.

- 즉 주어진 원소를 반복연산하여 구성되는 집합이다.

- 예 : 앞뒤와 각 모서리를 구분하는 정육각형 종이를 <br>
 고정된 위치의 같은 크기 정육각형 틀에 <br> 
 앞면을 위로 하여 두는 방법들의 집합

    - 즉 회전만 고려함

### 2) 대칭군(對稱群 : symmetric group) : $S_n$

- 주어진 집합($S$)의 모든 일대일함수(bijectives <br>
 $f:S\rightarrow S$ )들을 원소로 가지는 집합

- 예: 주어진 대상들의 순서를 정하는 <br>
 방법(순열/치환 : permutation)들의 집합

    - 순서 바꾸기 개념임

### 3) 정이면체군(正二面體群 : dihedral group) : $D_n$

- 정다각형의 대칭군인 유한군

- 예 : 앞뒤는 구분 안하고 모서리는 구분하는 정삼각형 종이를 <br>
 고정된 위치의 같은 크기 정삼각형 틀에 두는 방법들의 집합

- 모든 이면군은 두 개의 기본 원소가 있다 : 즉 회전과 뒤집기

    - 회전(rotation) $r$ : $n$ 번 실행하면 원래 모양 된다.

    - 뒤집기(flip) $f$ : 2 번 실행하면 원래 모양 된다        

        - 뒤집어 회전 $fr$ : 2회 실행해도 원래가 된다

        - 회전 후 뒤집기 $rf$ : 2회 실행헤더 원래가 된다

- 따라서 다음과 같이 정의될 수 있다.

    - $D_n = ⟨ \; r,f \;:\; r^n = f^2 = (rf)^2 = (fr)^2 = 1 \; ⟩$

<br>

## 부분군(部分群 : subgroup)

- 주어진 군(G)의 부분집합(H)으로서 군의 성질을 만족하는 것

- 자명한 부분군(trivial subgroup) : $\\{ 1 \\}$

    - 항등원만으로는 구성되는 집합은 항상 군이 된다.

## 정규부분군(正規部分群 : normal subgroup)

- $N$ 이 $G$ 의 부분군일 때 ( $N<G$ ) <br> 다음이 성립하면 <br>
$N$ 을 $G$ 의 정규부분군이라 한다 ( $N \vartriangleleft G$ ).

- $aN = \\{ \; a \cdot n \;:\; \forall n \in N \; \\}$ 그리고 <br> $Na = \\{ \; n \cdot a \;:\; \forall n \in N \; \\}$ 로 정의하면

- TFAE : the following are all equivalent

    1. $ \; \forall a \in G  \; : \;  a N = N a$
    
    2. $ \; \forall a \in G  \; : \;  a N a^{-1} \subset N$

    3. $ \; \forall a \in G  \; : \;  a N a^{-1} = N$

<br>