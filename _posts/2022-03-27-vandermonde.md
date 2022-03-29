---
title: 방데르몽드 행렬 Vandermonde matrix
categories: 
- algebra
tags:
- 대수학
- algebra
- 선행대수
- 행렬식
- 방데르몽드
date: 2022-03-26 10:10:10
---

### 방데르몽드 행렬 Vandermonde matrix
- Alexandre-Théophile Vandermonde : 1735 – 1796
- 각 행이 등비수열  
a geometric progression in each row

$$V =
\left(\begin{array}{cc} 
1 & \alpha_1 & \alpha_1^2 & \cdots & \alpha_1^{n-1} \\
1 & \alpha_2 & \alpha_2^2 & \cdots & \alpha_2^{n-1} \\
1 & \alpha_3 & \alpha_3^2 & \cdots & \alpha_3^{n-1} \\
\vdots & \vdots &  \vdots &        & \vdots         \\
1 & \alpha_m & \alpha_m^2 & \cdots & \alpha_m^{n-1} \\
\end{array}\right)
$$ 

<br>

###  방데르몽드 행렬식 Vandermonde determinant
- 정방 방데르몽드 행렬의 행렬식

$$\displaystyle \det(V) = \prod_{1\le i\le j\le n}(\alpha_j - \alpha_i)$$

- 따라서 같은 공비를 가진 행이 있는 경우 행렬식 = 0
  - 이 경우 선형종속이 발생하기 때문이다
- 예시

  $$
  \begin{align*}
  \begin{vmatrix}
  \;1 & \alpha_1 \; \\ 
  \;1 & \alpha_2 \; \\ 
  \end{vmatrix} \;&=\;\; 
  \alpha_2 - \alpha_1 \\ \\
  \begin{vmatrix}
  \;1 & \alpha_1 & \alpha_1^2 \; \\
  \;1 & \alpha_2 & \alpha_2^2 \; \\
  \;1 & \alpha_3 & \alpha_3^2 \; \\
  \end{vmatrix} \;&=\; 
  (\alpha_3 - \alpha_2)(\alpha_3 - \alpha_1)(\alpha_2 - \alpha_1)
  \end{align*}
  $$

<br>

### 3차 방정식 복소수 근의 응용

- $x^3=1$ 의 복소수 근을 $\omega$ 라고 하면  
$1+\omega+\omega^2=0$ 이므로

$$
\begin{align*}
W = &\left(\begin{array}{cc} 
1 & 1 & 1 \\ 
1 & \omega & \omega^2 \\
1 & \omega^2 & \omega^4 \\
\end{array} \right) \\ \\
= &\left(\begin{array}{cc} 
1 & 1 & 1 \\ 
1 & \omega & \omega^2 \\
1 & \omega^2 & \omega \\
\end{array} \right) \\ \\
W^{-1} =\; \frac{\;1\;}{3} 
&\left(\begin{array}{cc} 
1 & 1 & 1 \\ 
1 & \omega^2 & \omega \\
1 & \omega & \omega^2 \\
\end{array} \right)
\end{align*}$$ 

<br>

### 4차 방정식 복소수 근의 응용

- $x^4=1$ 의 복소수 근을 $\omega$ 라고 하면  
$1+\omega+\omega^2+\omega^3=0$ 이므로  
또는 $\omega = \pm \;i$ 이므로, 

$$
\begin{align*}
W = &\left(\begin{array}{cc} 
1 & 1        & 1        & 1        \\ 
1 & \omega   & \omega^2 & \omega^3 \\
1 & \omega^2 & \omega^4 & \omega^6 \\
1 & \omega^3 & \omega^6 & \omega^9 \\
\end{array} \right) \\ \\
= &\left(\begin{array}{cc} 
1 & 1        & 1        & 1        \\ 
1 & \omega   & \omega^2 & \omega^3 \\
1 & \omega^2 & 1        & \omega^2 \\
1 & \omega^3 & \omega^2 & \omega   \\
\end{array} \right) \\ \\
W^{-1} =\; \frac{\;1\;}{4} 
&\left(\begin{array}{cc} 
1 & 1        & 1        & 1        \\ 
1 & \omega^3 & \omega^2 & \omega   \\
1 & \omega^2 & 1        & \omega^2 \\
1 & \omega   & \omega^2 & \omega^3 \\
\end{array} \right)
\end{align*}
$$ 


- Note : $x^4=1$ 의 실수근($\pm 1$)의 경우는  
방데르몽드 행렬식 = 0 으로 역행렬 없음

<br>

### 5차 방정식 복소수 근의 응용

- $x^5=1$ 의 복소수 근을 $\omega$ 라고 하면  
$1+\omega+\omega^2+\omega^3+\omega^4=0$ 이므로

$$
\begin{align*}
W = &\left(\begin{array}{cc} 
1 & 1        & 1        & 1        & 1        \\ 
1 & \omega   & \omega^2 & \omega^3 & \omega^4 \\
1 & \omega^2 & \omega^4 & \omega^6 & \omega^8 \\
1 & \omega^3 & \omega^6 & \omega^9 & \omega^{12} \\
1 & \omega^4 & \omega^8 & \omega^{12} & \omega^{16} \\
\end{array} \right) \\  \\ 
=\; &\left(\begin{array}{cc} 
1 & 1        & 1        & 1        & 1        \\ 
1 & \omega   & \omega^2 & \omega^3 & \omega^4 \\
1 & \omega^2 & \omega^4 & \omega   & \omega^3 \\
1 & \omega^3 & \omega   & \omega^4 & \omega^2 \\
1 & \omega^4 & \omega^3 & \omega^2 & \omega   \\
\end{array} \right) \\ \\ 
W^{-1} =\; \frac{\;1\;}{5} 
&\left(\begin{array}{cc} 
1 & 1        & 1        & 1        & 1        \\ 
1 & \omega^4 & \omega^3 & \omega^2 & \omega   \\
1 & \omega^3 & \omega   & \omega^4 & \omega^2 \\
1 & \omega^2 & \omega^4 & \omega   & \omega^3 \\
1 & \omega   & \omega^2 & \omega^3 & \omega^4 \\
\end{array} \right)
\end{align*}$$
