---
title: 군(group)의 기초 개념
categories: 
- Algebra
tags:
- group theory
- cyclic group
- symmetric group
- dihedral group
- subgroup
- normal subgroup

date: 2022-03-14 10:54:30
---

## 잉여류(coset)

군 $G$ 와 $G$ 의 부분군 $H$ 가 있을 때,  
임의의 $x \in G$ 에 대하여  
$H$ 의 $xG$ 에 대한 우잉여류(right coset)는  
다음과 같이 정의되는 집합이다 :

- $Hx \equiv \\{ \; h \cdot x \;:\; h \in H \; \\} $

마찬가지로 좌잉여류(left coset)는  
다음과 같이 정의되는 집합이다 :

- $xH \equiv \\{ \; x \cdot h \;:\; h \in H \; \\} $

잉여류(coset)
- 우잉여류와 좌잉여류가 같다

### Example

- $S_3 = \\{ \; 1, (1,2), (1,3), (2,3), (1,2,3), (1,3,2) \; \\}$

- 부분군 $A_3 = \\{ \; 1, (1,2,3), (1,3,2) \; \\}$

- 부분군 $H = \\{ \; 1, (1,2) \; \\}$ 

- 여기서 $G = S_3$ , 그리고 $N = A_3$ 이라고 하면

- $N$ 는 우잉여류와 좌잉여류가 같다

- 즉 $N$ 의 우잉여류는

    - $N1 = N(123) = N(132) = \\{ \; 1, (123), (132) \; \\}$
    
    - $N(12) = N(13) = N(23) = \\{ \; (12), (13), (23) \; \\}$

- $N$ 의 좌잉여류는

    - $1N = (123)N = (132)N = \\{ \; 1, (123), (132) \; \\}$
    
    - $(12)N = (13)N = (23)N = \\{ \; (12), (13), (23) \; \\}$

- 그러나 $H$ 는 다르다.

- $H$ 의 우잉여류는

    - $H1 = H(12) = \\{ \; 1, (12) \; \\}$
    
    - $H(13) = H(132) = \\{ \; (13), (132) \; \\}$

    - $H(23) = H(123) = \\{ \; (23), (123) \; \\}$

- $H$ 의 좌잉여류는

    - $1H = (12)H = \\{ \; 1, (12) \; \\}$
    
    - $(13)H = (123)H = \\{ \; (13), (123) \; \\}$

    - $(23)H = (132)H = \\{ \; (23), (132) \; \\}$

위에서 군의 모든 원소가 각 잉여류로 전부 분류되며(분할)  
각 잉여류는 해당 부분군과 원소의 개수와 같다.

- $H$ 의 원소 $x$ 를 $hx$ 에 대잉시키는 <br>
$H \rightarrow Hx$ 는 일대일대응이다
    
- $\| G \| = \| H \| \times \|G:H \|$
    - 단, $\| G \|$ 는 군 $G$ 의 원소의 개수(위수)이며
    - $\|G:H \|$ 는 부분군 $H$ 에 의한 잉여류의 개수인데,
    - 이를 $H$ 의 지수(index)라고 한다.

## 정규부분군(正規部分群 : normal subgroup)
 
- $N$ 이 $G$ 의 부분군일 때($N < G$) 다음이 성립하면 <br> $N$ 을 $G$ 의 정규부분군이라 한다($N \vartriangleleft G$). 

- TFAE : the following are all equivalent

    1. $\; \forall a \in G  \; : \;  a N = N a$
    
    2. $\; \forall a \in G  \; : \;  a N a^{-1} \subset N$

    3. $\; \forall a \in G  \; : \;  a N a^{-1} = N$

- 단, 위에서 $aN = \\{ an : \forall n \in N \\}$ <br> 그리고 $Na = \\{ na : \forall n \in N \\}$

- 앞의 예에서 $N$ 는 좌/우 잉여류가 같으므로 정규부분군이다

- 그러나 $H$ 는 좌/우 잉여류가 다르므로 정규부분군이 아니다.

<br>

## 잉여류 전체의 집합 : 몫군

군 $G$ 와 $G$ 의 정규부분군 $N$ 이 있을 때,  

잉여류 전체의 집합 $\\{ \; Nx \;:\; x \in G \; \\}$ 를

$G/N$ 으로 표시하며, 여기 적절한 연산을 적용하여

- 연산 : $(Nx)(Ny) = N(xy)$

상군 또는 몫군(quotient group)을 만들 수 있다.

- 예 : 정수 전체 집합을 "3" 으로 나눈 나머지로 구분한 집합
    - $Z/3Z = \\{ \; \bar{0}, \; \bar{1}, \; \bar{2} \; \\}$
        - $\bar{0} = \\{ \cdots , -6, -3, \; 0, \; 3, \; 6, \cdots  \\}$
        - $\bar{1} = \\{ \cdots , -5, -2, \; 1, \; 4, \; 7, \cdots  \\}$
        - $\bar{2} = \\{ \cdots , -4, -1, \; 2, \; 5, \; 8, \cdots  \\}$

<br>
