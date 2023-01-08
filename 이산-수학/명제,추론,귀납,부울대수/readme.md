영상: https://www.youtube.com/playlist?list=PLD8rdlfZeJk7ijUM8ckwLLNyDKRD2aQa2

## [명제와 연산자](/이산-수학/이산수학-기초/명제와-연산자.md)

## 추론,연역법과 귀납법

### 추론

우리는 이미 "참"으로 알고 있는 명제(들)로부터 새로운 "참"인 명제를 찾아내려고 한다.
이러한 과정을 통해서 새로운 지식을 얻게 되는 과정을 추론이라고 한다.

올바른 추론의 규칙을 우리는 논리라고 부른다.

- 이미 T로 알고 있는 명제 -> 전제
- 우리가 알아내고자 하는 명제 -> 결론
- 추론의 방법
  - 연역법 (deduction)
  - 귀납법 (induction)

### 연역법 (deduction)

연역법은 형식 논리의 다음과 같은 명제의 틀에 기반을 두고 있다.

- P가 참이면 Q는 참이다.
  P는 참이다
  -> Q는 참
- 전제가 T이면 결론은 T이다.



### 귀납법 (induction)

개별적인 사실을 말하는 명제들로부터 일반적인 결론을 도출하는 방법

- 예시
  - 김철수, 이영희, 홍복동은 컴퓨터공학과 학생이다.
    김철수는 C언어를 수강한다.
    이영희는 C언어를 수강한다.
    홍복동은 C언어를 수강한다.
  - 따라서 모든 컴퓨터 공학과 학생들은 C언어를 수강한다.
    -> T?
  - 귀납법의 문제는 현실적으로 집합의 모든 원소에 대해서 참인 것을 밝힐 수 없다는 점이다. 따라서 도출된 결론은 기껏해야 확률적인 결론일 수 밖에 없다.

### 수학적 귀납법 (mathematical induction)

- 하지만, 수학적 귀납법은 이러한 귀납법의 한계를 극복
- 집합의 모든 원소에 대해서 명제가 성립하는 것을 보여준다.
- 따라서, 모든 경우에 명제가 성립하는 것을 증명할 수 있다.



- P(1)이 성립한다.
- P(k)가 성립하면, P(k+1)도 성립한다.

## [부울 대수(Boolean Algebra)](/이산-수학/명제,추론,귀납,부울대수/부울-대수.md)

### 논리회로 설계 과정

​	논리 회로 설계 문제 -> 입력, 출력 정의 -> 부울 함수 -> 부울식 -> 부울식 최소화 -> 논리회로

### 부울 대수 (Boolean Algebra)

- 공리 (Axiom)

  - 정의

- 보수 : '로 표시

  - 원소 0에 대하여 0' = 1, 원소 1에 대하여 1' = 0

- 합 : + 또는 OR로 표시

  - 1 + 1 = 1
  - 1 + 0 = 1
  - 0 + 1 = 1
  - 0 + 0 = 0

- 곱 : • 또는 AND로 표시, (•는 생략하여 표기하기도 한다.)

  - 1 • 1 = 1
  - 1 • 0.  0
  - 0 • 1 = 0
  - 0 • 0 = 0

- 연산 우선순서

  - 보수 >> 곱 >> 합

- 부울 변수

  - 집합 S = {0, 1}의 원소 값만을 갖는 변수

- 부울 함수

  - 0또는 1의 입력값을 에 대하여 0 또는 1의 출력값을 갖는 함수
  - F(x, y, z)

- 부울 식

  - 부울 함수는 부울 변수와 부울 연산자로 구성된 부울 식으로 표현할 수 있다.
  - xy + z

- 항등

  - 부울 함수 F와 G가 모든 입력값에 대해 같다면 부울 함수 F와 G는 동등하다.

- 부울대수 법칙

  ![부울 대수 법칙](https://mblogthumb-phinf.pstatic.net/MjAyMTA0MTZfMTYg/MDAxNjE4NTgzODQwMDA0.-nv0wpH5ZAeM0mrue8fTLvW3ewtvvPs3FH8lMKXkFkcg._Xb1mKvOenKy5jkh3U5dawDNf_Jt-I7DNRVfL4SKSSMg.PNG.brinson/%EB%B6%80%EC%9A%B8_%EB%8C%80%EC%88%98%EC%9D%98_%EC%A0%95%EB%A6%AC%EC%99%80_%EB%B2%95%EC%B9%99.png?type=w800)

- 문제
  x(x+y) = x를 증명하라.

  - x(x+y)
    = (x+0)(x+y) : 항등 법칙
    = x + 0y : 분배 법칙
    = x + y0 : 교환 법칙
    = x + 0 : 지배 법칙
    = x

- 증명 방법

  1. 정의 -> 진리값
  2. 이미 증명된 명제 (규칙)

- 쌍대성의 원리

  - x + 0 = x, x • 1 = x
  - 이러한 쌍을 쌍대라고 한다.
  - 부울식으로 표현된 함수들 사이에 항등성이 유지되면, 이들의 쌍대도 항등성을 유지한다.
  - +와 •을 교환하고, 0과 1을 교환할 수 있다. 

- 최소항

  - 함수의 모든 변수에 대하여 부울 곱을 취한 것으로 변수는 변수 문자 또는 변수 문자의 보수 형태가 한번씩만 나타난다.

- 논리합 형식 : 곱들의 합

  - 부울 하수를 최소항들의 부울 합으로 나타내는 형식
  - 부울 함수의 부울식은 함수의 값이 1이 되는 변수값의 조합들에 대하여 최소항들을 구하고 그 최소항들의 부울 합을 취하면 구할 수 있다.
  - 예시
    x y F(x,y)
    1 1 1 -> xy
    1 0 0
    0 1 1 -> x'y
    0 0 0 -> x'y'
    F(x, y) = xy + x'y + x'y'

  ### 카르노 맵

  부울 함수의 간단한 논리합 형식을 찾아내는 방법

  1. 두 변수 x, y를 갖는 부울식을 위한 카르노 맵은 사각형에서 2 x 2개의 칸으로 구성된다. 각 칸은 부울 함수의 최소항을 의미한다.

     |      | x    | x'   |
     | ---- | ---- | ---- |
     | y    | xy   | x'y  |
     | y'   | xy'  | x'y' |

     

  2. 부울 함수에서 해당 최소항이 있으면 그 칸을 1로 표시한다.

     |      | x    | x'   |
     | ---- | ---- | ---- |
     | y    | 1    |      |
     | y'   | 1    | 1    |

  

  - 예시

    1. x'y'

       |      | x    | x'   |
       | ---- | ---- | ---- |
       | y    |      |      |
       | y'   |      | 1    |

    2. xy + xy' + x'y + x'y'

       |      | x    | x'   |
       | ---- | ---- | ---- |
       | y    | 1    | 1    |
       | y'   | 1    | 1    |

- 부울식의 최소화

  - 하나의 변수만이 다른 최소항들은 서로 인접한다고 한다.

- 세 개의 변수를 가진 카르노 맵

  - 인접하는 네 개의 칸에 1이 있으면 네 개의 최소항은 공통변수 하나의 최소항으로 합성될 수 있다.

  - 예) xyzzy, xy'z, xyz', xy'z' -> x

    |      | xy   | xy'   | x'y' | x'y  |
    | ---- | ---- | ----- | ---- | ---- |
    | z    | xyz  | xy'z  |      |      |
    | z'   | xyz' | xy'z' |      |      |

  

- 카르노 맵을 만들 때

  1. 변수가 2개면 2x2, 변수가 3개면 4x2, 변수가 4개면 4x4
  2. 인접하는 칸들은 동일한 변수를 갖고 있어야 한다.
     그리고 인접되는 칸들은 원통처럼 연결되어 있다.
  3. 인접하는 칸들을 붂을 때는 2^n, 2^(n-1),,, 순으로 묶는다.
     예를 들면 변수가 3개일 때 2^2, 2^1순서로 인접하는 항을 묶는다.

  

## 논리회로 설계

### 게이트와 부울 연산

전자 장치의 입력과 출력은 0 또는 1이기 떄문에 전자 회로를 설계하는데 부울 대수를 사용할 수 있다.

게이트(gate): 회로의 기본 요소

- 인버터 - 보수

- OR게이트 - 부울 합

- AND게이트 - 부울 곱

  ![논리게이트 : 네이버 블로그](data:image/png;base64,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)

