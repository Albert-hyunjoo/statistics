# 상관관계

## 산포도에 대해서
* 두 변수 사이의 관계는 `산포도`를 통해서 알 수 있다.
* `산포도`의 전반적 모양이 오른쪽 위를 향하면 **양의 관계**, 우하향이면 **음의 관계**
* 하지만 45도선 기준으로 퍼져 있으면 그 정도는 약하다고 볼 수 있다.
* `상관관계`는 `독립변수`가 `피설명변수`에 어떤 영향을 미치는지를 보여준다.

## 상관계수 -- 관계의 강도
* 일반적으로 두 변수로 이루어진 자료들은
  1) `x값의 평균과 표준편차` (세로),
  2) `y값의 평균과 표준편차` (가로),
  3) 그리고 `상관계수`로 그 관계가 표현된다.
* `상관관계`는 반드시 **-1과 1 사이**의 수치를 유지하게 된다.

## 상관계수 구하기
* 변수 X, Y에 대해서 
    1) `(x1, y1), (x2, y2)..`가 있으며,
    2) X의 표본평균은 `bar^x`, Y의 표본평균은 `bar^y`이며,
    3) 표본표준편차는 `SDx`, `SDy`라고 가정한다.
* 이 경우에서 `상관계수`는 `r` =  `X 편차와 Y 편차의 곱의 합`/`X편차 합의 제곱근`*`Y편차 합의 제곱근`
* 이 식을 자유도를 뺀 값으로 나누면 `상관계수`의 식은 `Cov(x,y)`/`두 변수의 표편 곱`이 된다.
  * `공분산 (Cov(x,y))`를 곱할 때 두 편차를 곱하는 이유는, 두 변수 사이의 관계가 **편차들의 곱에 반영**되기 때문이다.
    * 만약 편차가 x,y 둘 다 **평균보다 크면** 양의 관계가 우세, **반대**면 음의 관계가 우세
* `상관계수`는 **측정단위가 기존 데이터에 무관**하며 **방향성**이 없어 유용하게 쓰인다.
* (참고) 사분면에서 어떤 부분에 점이 많아야 그 정도를 가늠할 수 있는가? **1,3 사분면**

## 상관관계 및 계수 사용 유의!
* `상관계수`는 **배수의 관계가 아니다**. 즉, r = 0.8이 r = 0.4보다 정확히 두 배 강한게 아니다.
* **표준편차의 변화**는 상관관계에 크게 영향을 끼치지 않는다.
* 만약 두 변수의 관계가 **`이탈값`이 많고, `비선형`인 경우** 상관관계의 효과는 크게 떨어진다. (필요시 로그변환)
* 비율과 평균의 자료를 갖고 구하는 상관계수는 **실제의 관계**를 과장할 수도 있다.
* 지역이나 국가 등 `집단 단위의 상관계수`는 `개개인에게 적용되는 관계`를 과장할 수 있으므로 주의해야 한다.
* `상관관계`는 절대 곧바로 `인과관계`로 해석되어서는 안된다! 절대!

## 상관관계의 성질
* (*`코시-슈바르츠 부등식` 증명에 따라*) `상관계수`는 언제나 **-1에서 1사이**이다.
* `상관계수` **r의 절대값**이 커질 수록, **`선형관계`의 강도**는 커진다.
* 두 변수의 **순서를 바꾸어도** `상관계수`는 변하지 않는다.
* `상관계수`는 `선형변환`에 의하여 그 절대값이 **변하지 않는다**.


