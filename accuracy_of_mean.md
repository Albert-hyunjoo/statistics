# 평균의 정확성

## 표본분포와 표준편차

> `단순무작위표본`에서 구한 평균은 얼마나 **정확하고**, **모평균**과 다른가?

* `표본비율`을 통해 `모비율`을 추론하는 문제를 일반화하면    
  `표본평균`을 토대로 `모평균`을 추론하는 문제로 일반화시킬 수 있다.    
  (0과 1밖에 없는 표본의 평균을 구하면 그게 바로 비율이다)
* `표본평균`의 **기댓값**과 **표준오차**를 구해서 값의 신뢰성을 가늠할 수 있다.
> 예시)    
> 1~7부터 카드가 한 장씩 들어 있는 상자로부터 25회 무작위 복원추출 시,    
> 표본평균의 기댓값과 표준오차를 구하라.    
> 답안)    
> 상자의 평균은 *4*이고, 여기서 표본합의 기댓값은 *25 * 4 = 100*    
> 상자의 표준편차는 *2* √(편차 -- 편차제곱의 평균)므로 제곱근 법칙에 따라 √25 * 2 = *10*      
> 표본평균은 *표본합을 표본크기로 나누어* 얻는 경우로 100+-10 / 25 = *4 +- 0.4*에 해당한다.

* `상자모형` 상에서는 다음과 같이 용어를 구분한다:    
  * `표본평균`의 `기댓값`: 상자의 `평균`
  * `표본평균`의 `표준오차`: `표본합`의 `표준오차`/표본크기 = 상자의 `표준편차`/√표본크기
  * 상자의 `표준편차`와 `표본표준편차` (SD)
    * 상자의 `표준편차`는 상자에서 <span style = "color:red">하나의 값</span>을 추출할 때, <span style = "color:red">모평균</span>과 차이?
    * `표본표준편차`는 <span style = "color:red">표본 내 하나의 값</span>이 <span style = "color:red">표본평균</span>과 얼만큼 떨어져 있나?   
  여기서 이 `표본표준편차`는 상자의 `표준편차`에 대한 추정치가 된다.
  * 표본평균의 `표준오차 (SE)`: <span style = "color:red">표본평균</span>이 얼마나 <span style = "color:red">모평균</span>과 떨어져 있는가?
    * **표본평균이 아무래도 모평균과 가까**운데, 이는 **표본평균의 표준오차**가 **상자의 표준편차**보다 작게 된다.
  > [ 이를 종합하면 다음의 식이 도출된다 ]    
  > **표본평균의 표준오차 (SE)** = 상자의 표준편차 / √표본크기 =*유사*= 표본표준쳔파 / √표본크기
  
* **표본평균**을 히스토그램으로 정리하면 **정규분포**와 근사된다. (왜? *중심극한정리*)

> 예시 -- 제곱근 법칙)    
> 1~7부터 카드가 한 장씩 들어 있는 상자로부터 25->100회 무작위 복원추출 시,    
> 표본평균의 기댓값과 표준오차를 구하라.    
> 답안)    
> 상자의 평균은 *4*이고, 여기서 표본합의 기댓값은 *100 * 4 = 400*    
> 상자의 표준편차는 *2* √(편차 -- 편차제곱의 평균)므로 제곱근 법칙에 따라 √100 * 2 = *20*      
> 표본평균은 *표본합을 표본크기로 나누어* 얻는 경우로 400+-20 / 100 = *4 +- 0.2*에 해당한다.

## 표본평균으로 모평균 추정하기

* 통상적으로는 모집단과 관련된 정보를 알 수 없는 경우가 대다수이다.
* 이 경우에는 표본평균을 이용하여 상자의 평균을 추정하는 `통계적 추론`을 할 수 있다.
> 예시 -- 통계적 추론)    
> 어느 도시의 2만 5천 가구의 연평균소득을 알고 싶다고 가정한다.    
> 1000 가구를 무작위로 추출한 결과 그 가구의 연평균소득은 3240만원이고, 표편은 1900만원이다.    
> 이 도시 전체의 연평균소득은 어떻게 구할 것인가?    
> 해답)    
> 1000가구의 표본평균이 3240만원, 표준편차는 1900만원이라고 한다면,    
> 표본평균의 표준오차는 1900 / √1000 = 60만원 (유사값)이다.    
> 우리가 알고자 하는 부분은 모평균이므로 필요한 통계는 3240만원과 60만원 (모평균과의 오차)    
> 95% 신뢰범위로 계산하면 (-2SE, 2SE) (3120먼원, 3360만원)

## 어느 표준오차를 사용해야 하나?
* 추론의 목표에 맞는 표준오차를 사용하면 된다.
> 표본합의 표준오차 : 상자의 표준편차 x √표본크기    
> 표본평균의 표준오차 : 상자의 표준편차 / √표본크기    
> 표본개수의 표준오차 : 0-1 상자로부터의 표본합의 표준오차    
> 표본비율 (%)의 표준오차 : (표본개수의 표준오차/표본크기) * 100%

## 상기할 점
* 확률오차의 대략적인 크기는 `표준오차`로 측정된다.
* `편의표본`에 무작위표본의 표준오차 공식을 쓰지 않도록 주의해야 한다.

## 측정오차
* `측정치`는 `참값`과 `확률오차`만큼의 차이를 보인다 (`측정오차`)
* 통상적으로 측정과정에 `확률오차`가 개입되며, 반복측정으로 이를 개선할 수 있다.
* 반복측정에서 측정값들은 참값은 변하지 않으며, `가우스모형`에 따라 오차상자의 평균은 0이다.
* 즉, **반복측정치들의 표준편차**와 **확률오차들의 표준편차**는 동일하다.
* 상자 모형이 아니면 굳이 표준오차를 구할 필요가 없다.

## 모집단과 표본의 관계

* 상자 내 카드 전체가 `모집단`이라면, 거기서 추출한 카드는 `표본`이다.
* 상자의 중심은 `모평균`이고, 상자의 표준편차가 `모표준편차`이다.
* 추출된 카드의 중심이 `표본평균`이고, 그 표본 안의 개개의 카드가 `표본평균`과 떨어진 정도가 `표본표준편차`
* `모평균`은 모집단으로부터 자료 하나를 추출할 때의 `기대값`과 동일하다.    
즉, 한 장 한 장이 Y1, Y2..라고 한다면
> **모평균 = E(Y1) = E(Y2)...이**다.
* 개별카드에 적힌 숫자를 `편차`로 표현하면 MSE했을 때 `모표준편차`는
> 모표준편차^2 = E(Yi-모평균)^2
* 표본의 경우에는 조금 달라지는데, 표본의 기댓값은 *E^hat*로 가정할 때,
> *Y_bar* = *E^hat* * Y1 = .... = (Y1+Y2+Y3..)/표본의 갯수    
> = E^hat * Yi = Y1 * (1/n) + Y2 * 1/n ...    
> = 이는 곧 표본 내 자료 분포 기댓값 *Y_BAR*는 관측치 각각에 **동일한 가중치**를 주어 **개별 관측치 값을 평균**하는 역할을 한 셈이다.
* 문제는 분산을 구할 때 `모평균`대신 `표본평균`을 쓰게 되는데,    
  이미 표본 내 잔차들이 `모평균` 대신 `표본평균`을 쓰게 된 만큼 값이 줄었으며,        
  자유도를 조정하지 않으면 (n-1) 이 과정에서 모분산의 체계적 과소평가 문제를 피할 수 있다.
* 이를 수식으로 표현하면 **E(표본분산) = 모분산**, **즉 표본분산은 모분산의 `불편추정량`이다.**    
  (단, 표본표준편차는 모표준편차의 불편추정량이라고 볼수는 없다 -- 젠슨의 부등식)

|구분|모집단|표본
|:---:|:---:|:---:|
|자료|상자에 든 카드 일체|상자로부터 추출한 카드 모음|
|자료 표기|Y1, Y2..., YN (N은 전체)|Y1, Y2...,Yn(n은 추출)|
|평균|모평균 = 전체 자료의 기댓값 -- 통상적으로 개수로 나눔|표본평균 = 표본의 기댓값|
|분산 (가상)|해당 없음|(모평균 값을 알 수 없으므로) 가상의 표본분산 = (표본과 모평균의 편차)^2의 표본 기댓값
|분산 (실제)|모분산 =편차의 기댓값^2|실표본분산 = (표본과 표본평균의 차이)^2(df = n-1)의 기댓값

## 표본평균의 기대값, 분산, 표준오차의 수학적 정리

### 기본적인 정리부터
어떤 상자로부터 무작위로 **n장의 카드**를 **복원 추출**했을 때,    
i번째로 꺼낸 카드에 적혀있는 숫자를 *Xi*라고 한다.    
그리고 뽑은 숫자의 합과 평균을 *S*, *X_bar*라고 한다.    
상자의 평균과 표준편차를 *mu*, *sigma*라고 한다.

1) *S* = X1 + X2 + X3... + Xn
2) *X_bar* = (X1 + X2 ... Xn) / n
3) *mu* = E(Xi) (i = 1,2...n)
4) *sigma*^2 = Var(Xi) = E(X-mu)^2 = E(Xi)^2 - mu^2 (i = 1,2,...n)

### 표본평균의 기댓값과 표준오차?

1)  표본평균의 기댒값 = E(X_bar)     
    = E(S/n)     
    = 1/n * E(S)     
    = 1/n * (_n_ * _mu_) = _**mu**_
2)  표본평균의 분산과 표준오차    
= Var(표본평균)    
= E(표본평균 - 표본평균의 평균 (= 표본평균의 기댓값 = 모평균))^2    
= E(S/n - mu)^2    
= E(1/n * (S-n*mu))^2    
= 1/n^2 * E(S-n*mu)^2 = (표본합 - 표본합의 기댓값)의 기댓값     
= 표본합의 표준편차^2
= 1/n^2 * 표본합의 분산 (= n * 모분산)    
= 1/n * 모분산    
= **표본평균의 표준오차는 모표준편차에서 표본크기를 나눈 것**

### 표본평균의 표본분포 -- 정규분포
* n이 커지면 **표본합 S의 분포**는 **Xi의 분포와 관계 없이** **정규분포**에 근사
* **표본평균**은 **표본합을 표본크기로 나눈 것**으로, 표본크기가 커지면 역시 정규분포에 근사한다.