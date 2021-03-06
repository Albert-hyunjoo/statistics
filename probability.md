# 확률에 대해서 (Probability)

## 가능성과 확률
* 확률을 보는 관점은 크게 `도수이론`과 `주관적 견해`가 있다,
* 이중에서 `도수이론`은 하나의 시행을 독립적이고 동일하게 여러번 할 때 수렴하는 상대도수에 대해 논하는 것,

### 확률의 대표적인 특성
1) 확률은 0%부터 100%만 적용된다.
2) 만약 어떤 A 사건이 일어날 확률이 x%면, 일어나지 않을 확률 (여사건)은 무조건 (100-x)% 이다.

## 복원추출과 비복원추출
* **복원추출**은 추출 후에 다시 이를 되돌려놓으므로, 매 시행이 **독립적**이다.
* **비복원추출**은 추출 후에 이를 **되돌려놓지 않으므로**, 매 시행이 전 시행에 **영향을 받는다** (종속)

## 덧셈법칙에 대해서
* 어떤 사건 A과 B가 **동시에 일어날 수 없으면,** A과 B는 `상호 배반적 사건`이다.
* `덧셈법칙`은 어떠한 사건들이 **적어도 한 번**은 일어날 수 있는 확률의 계산법에 해당한다.
> `P(A or B)` = `P(A) + P(B) - P(A and B)`

## 조건부확률에 대해서
* `조건부확률`은 어떠한 `사전 정보`가 주어진 시점에서 **변동되는 확률**이다.
> 만약 어떠한 사건 A가 먼저 일어난 시점에서 B가 일어날 확률을 구하고자 한다면,    
> `P(A and B)` = `P(A) * P(B|A)` or `P(B) * P(A|B)`로 표현한다.    
> ⁂ 어떠한 사건 A,B가 동시에 일어나는 확률을 구하는 것은 `곱셈법칙`이라고 한다.

## 분할과 베이즈 정리
* 통계적인 `분할`은 어떤 사건 확률의 집합이 한 사건을 `MECE`하게 커버하는 경우이다.    
  (동전을 던지는 사건의 경우에는 앞면, 뒷면이라는 사건 외에는 존재하지 않음)
* 이를 수식화한 것이 `베이즈 정리`로, **어떤 사건 중에 특정 조건부 확률 사건이 일어날 확률**을 구한다.
> `P(A|B)` = `P(A and B)/P(B)` = `P(A)P(B|A)/(P(A)P(B|A) + P(A^c|B))`

> 베이즈 정리의 예시 Q:    
> 어느 학생이 사지선다 객관식 문제를 풀었는데 맞았다.    
> 선생님은 이 학생이 이 문제를 실력으로 알고 맞혔는지, 아니면 찍었는지가 궁금하다.    
> 이 학생이 알고 맞췄을 확률은 무엇인가?    
> (선생님의 경험상 아이들이 보통 알고 맞추는 확률은 1/2이다.)    
> ----------    
> 해답:    
> 1. 문제를 맞추는 사건은 B, 그 지식을 안다는 사건은 A라고 가정한다.
> 2. 선생님이 알고 싶은 목표는 `P(A|B)`, 즉 정답을 맞췄을 때 (B) 알고 맞췄을 확률이다 (A)
> 3. `P(A|B)`는 달리 풀면 `P(A)*P(B|A)/P(A)*P(B|A) + P(A^c|B)`이다.
> 4. 일단 정해진 확률은 다음과 같다:
>   * P(A) = 1/2 (아이들이 지식을 아는 경우는 1/2)
>   * P(B|A) = 1 (지식을 알고 맞히는 경우는 무조건 1)
>   * P(A^c|B) = 아이들이 맞췄을 때, 지식을 모를 확률 -- 찍어서 맞춘다 = 1/4 (사지선다)
> 5. (1/2*1)/(1/2+1/4) = (1/2)/(5/8) = **4/5**

* `베이즈 정리`를 일반화한다면 식을 조금 더 확장시킬 수 있다.
> 어떤 사건 **A1 ~ Am**이 **전체 S의 분할**을 형성하고, 그 안에 **B 사건**이 있다면,    
> `P(A1|B)` = `B 사건이 벌어졌을 때 A1이 일어날 확률` = `P(A1 and B)/P(B)` = `P(A1)*P(B|A1)/P(A1 and B) + P(A2 and B)...` = `P(A1)*P(B|A1)/P(A1)*P(B|A1)+P(A2)*P(B|A2)...`

## 독립, 그리고 배반과의 차이
* `독립`은 **어떠한 사건 A의 확률**이 다른 사건 B의 확률에 **영향을 미치지 않는** 경우다.
* 만약 사건 A,B가 `독립`인 경우에는 `P(A|B) = P(A)`, 즉 B의 존재가 A에 영향을 끼치지 않는다.
* `독립`과 `배반`이 다른 점은 두 사건의 **동시 발생 가능 여부**이다.