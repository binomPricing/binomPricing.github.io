---
title: 대칭다항식 symmetric polynomial
categories: 
- algebra
tags:
- 대칭다항식 
- 대수학
- algebra
- symmetric polynomial
date: 2022-03-27 10:20:10
---

### 대칭다항식 symmetric polynomial
- 임의의 치환 $\sigma \in S_n$ 에 대하여  
$$f(x_1, x_2, \cdots, x_n) = f(x_{\sigma(1)}, x_{\sigma(2)}, \cdots, x_{\sigma(n)})$$
- 예 : $\quad x_1 + x_2 + x_3 - 7 x_1 x_2 x_3$
  - $\; x_1$ 과 $x_2$ 와 $x_3$ 를 바꾸어도 식이 변하지 않는다
- 예 : $\quad \alpha^2 + \beta^2$
  - $\;\alpha$ 와 $\beta$ 를 바꾸어도 식이 변하지 않는다

### 기본대칭다항식 elementary symmetric polynomial
- 2 변수 다항식은 2개
  - $\quad x_1 + x_2$
  - $\quad x_1 x_2$     
- 3 변수 다항식은 3개
  - $\quad x_1 + x_2 + x_3$
  - $\quad x_1 x_2 + x_2 x_3 + x_3 x_1$
  - $\quad x_1 x_2 x_3$
- 4 변수 다항식은 4개
  - $\quad x_1 + x_2 + x_3 + x_4$
  - $\quad x_1 x_2 + x_1 x_3 + x_1 x_4 + x_2 x_3 + x_2 x_4 + x_3 x_4$
  - $\quad x_1 x_2 x_3 + x_1 x_2 x_4 + x_1 x_3 x_4 + x_2 x_3 x_4$
  - $\quad x_1 x_2 x_3 x_4$  
- 5 변수 다항식은 5개

  $\vdots$

<br>

### 모든 대칭다항식은 기본대칭다항식의 다항식으로 표현된다
- 친절한 [증명]은 "대칭 : 갈루아 이론" by 신현용,신기철(2017) p.193 이하
- 예
  - $\alpha^2 + \beta^2 = (\alpha + \beta)^2 - 2\alpha\beta$
  - $ x_1^3 + x_2^3 + x_3^3 \;\;=$  
  $\quad (x_1 + x_2 + x_3)^3 \;+\; 3 x_1 x_2 x_3 \;\;-$  
  $\quad \quad 3(x_1 + x_2 + x_3)(x_1 x_2 + x_2 x_3 + x_3 x_1)$

<br>

### 방정식 근의 공식과의 관계
- 2차 방정식 $x^2 + a x + b \;=\; 0$ 의 두 근을  
$\alpha$ 와 $\beta$ 라고 하면
    - $x^2 + a x + b \;=\; (x-\alpha)(x-\beta) \;=\; 0$ 이므로
      - $\alpha + \beta \;=\; -a$
      - $\alpha\beta \;=\; b$    
- 3차 방정식 $x^3 + a x^2 + b x + c \;=\; 0$ 의 세 근을  
$\alpha$ 와 $\beta$ 와 $\gamma$ 라고 하면
    - $x^3 + a x^2 + b x + c \;=\; (x-\alpha)(x-\beta)(x-\gamma)$
      - $\alpha + \beta + \gamma \;=\; -a$
      - $\alpha\beta + \beta\gamma + \gamma\alpha \;=\; b$    
      - $\alpha\beta\gamma \;=\; -c$

  $\vdots$

- 즉 다항방정식 근들의 대칭다항식들은 모두  
    다항방정식 계수들의 다항식으로 표현된다
- 주의 : 이러한 관계식만으로는 근을 구할 수 없다
  - 원래의 방정식으로 환원됨(동어반복)
  - 그러나 추가적인 관계식을 찾아내면 구할 수 있다
  - 단, 4차 이하 방정식의 경우에만 가능하다
  - 5 차 이상 방정식의 경우에는  
  계수들의 거듭제곱근으로 표현되는  
  근의 공식을 도출할 수 없다

<br>    
    