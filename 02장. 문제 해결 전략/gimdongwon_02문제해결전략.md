# 문제 해결 전략

## 2.1 도입

프로그래밍 대회는 문제 해결 능력을 수련하기에 무척 좋은 화녁이지만 무작정 알고리즘을 외우고 문제를 푸는 것은 좋은 방법이 아니다. 좋은 문제 해결자가 되기 위해서는 좀더 높은 차원의 수련이 필요하다. 이 수련의 목표는 문제를 푸는 것이 아니라 `문제를 푸는 기술을 연마`하는것이다. 이를 위해서 자신의 어느 점이 부족하고 어떤 방시긍로 해결하는지를 의식하고 개선해야 할 부분을 파악하는 것이 중요하다. 이 장에서는 문제 해결 과정을 여러 단계로 나눠 보고 각 단계를 더 잘하기 위한 기술들을 살펴보자.

## 2.2 문제해결과정

현재 인류에게 알려진 가장 강력한 일반적 문제 해결 알고리즘인 파인만 알고리즘을 살펴보자.

1. 칠판에 문제를 적는다.
2. 골똘히 생각한다.
3. 칠판에 답안을 적는다.

이 알고리즘은 강력하고 우아할 뿐만 아니라 문제 해결에 필수적인 요소들을 모두 담고 있다. 그 첫번째는 바로 `문제 해결 과정을 단계 별로 나누었다`는 것이다. 문제를 해결하기 위해 거쳐가야 하는 과정들을 세분화함으로써 어디가 부족하고 어디를 개선해야 하는지 판단할 수 있다. 또다른 교훈은 `문제를 적는 단계가 있다`라는 점이다. 문제를 다시 적기 위해서는 자기자신의 언어를 이용해 재정의해야 하기 때문에 이 단계는 아주 중요하다.

문제 해결 연구의 고전인 "How to Solve it"에서는 문제 해결 과정을 다음과 같이 네단계로 나눠서 소개한다.

1. 문제를 이해한다.
2. 어떻게 풀지 계획을 세운다.
3. 계획을 수행해서 문제를 해결한다.
4. 어떻게 풀었는지 돌아보고, 개선할 방법이 있는지 찾아본다.

파인만 알고리즘의 골똘히 생각하는 단계를, 계획을 세우는 단계와 계획을 수행하는 단꼐로 나눴으며, 문제를 푼 다음에도 개선할 방법을 찾는 회고 단계가 추가된 것을 알수 있다. 작가가 추천하는 6 단계 알고리즘을 살펴보자.

```md
1. 문제를 읽고 이해한다.
2. 문제를 익숙한 용어로 재 정의한다.
3. 어떻게 해결할지 계획을 세운다.
4. 계획을 검증한다.
5. 프로그램을 구현한다.
6. 어떻게 풀었는지 보고, 개선할 방법이 있는지 찾아본다.
```

### 1 단계 : 문제를 읽고 이해하기

문제 해결 알고리즘의 첫 번째 단계는 문제를 읽고 이해하는 것이다. 많은 사람들이 이 단계는 당연히 잘할 수 있는 것으로 생각하지만 이 단계의 중요성은 아무리 강조해도 지나치지 않는다. 초심자 부터 챔피언 까지 공통으로 하는 실수가 있다면 문제를 잘못 읽는 실수이기 때문이다.

성급한 행동은 큰 대가를 치룬다. 문제 설명을 공격적으로 읽으며 문제가 원하는 바를 완전히 이해하는 과정이 반드시 필요하다. 문제의 궁극적인 목적을 롷게 이해하더라도 사소한 제약 조건을 잘못 이해하면 풀 수 없게 되는 문제들이 흔하고 대회에서는 이를 용납되지 않기 때문이다.

### 2 단계 : 재정의와 추상화

우리의 문제 해결 알고리즘의 두 번째 단계는 자신이 다루기 쉬운 개념을 이용해서 문제를 자신의 언어로 풀어 쓰는 것이다. 이 과정은 `문제가 요구하는 바를 직관적으로 이해`하기 위해 꼭 필요하며 요구하는 바가 복잡할 수록 그 중요성이 더해진다.

이 과정에서는 `추상화` 라는 중요한 일이 일어난다. `추상화란 현실 세계의 개념을 우리가 다루기 쉬운 수학적 / 전산학적 개념으로 옮겨 표현하는 과정이다.` 현실 세계의 개념들은 너무 복잡하기 때문에, 현실 세계를 다루기 위해서는 어느 정도 현실의 본질만을 남겨두고 축약하여 다루기 쉽게 표현해야 한다. 우리에게 익숙한 문제 해결 도구들을 문제에 적용하기 위해서 사용한다. 문제를 어떤 방식으로 재구성하느냐에 따라 어려운 문제도 쉽게, 쉬운 문제도 어렵게 만들 수 있다. 그러므로 어떻게 문제를 재 정의하는 벙법들에 대한 고찰은 `좋은 프로그래머가 되기 위한 필수적인 과정`이다.

### 3 단계 : 계획 세우기

`이 과정에서는 문제를 어떤 방식으로 해결할지 결정하고, 사용할 알고리즘과 자료구조를 선택한다.` 사실상 가장 중요한 단계라고 할 수 있다. 물론 자신이 당장 알고있는 알고리즘과 자료구조라면 쉽게 해결하겠지만 문제를 보고 어떻게 해결해야 할지 곧장 떠오르지 않는 어려운 문제의 겨웅 이 과정에서 가장 많은 고민을 하게 된다.

### 4 단계 : 계획 검증하기

계획을 세웠다고 곧장 키보드를 잡을 수 있는 것은 아니다. 구현을 시작하기 전에 계획을 검증하는 과정을 거쳐야한다. 이 과정에서는 우리가 설계한 알고리즘이 `모든 경우에 요구 조건을 정확히 수행하는지를 증명하고 수행에 걸리는 시간과 사용하는 메모리가 문제의 제한 내에 들어가는지 확인 해야한다.`

### 5 단계 : 계획 수행하기

이와 같은 복잡한 과정을 거치고 나서 코딩을 할수가 있다. 아무리 천재적인 알고리즘이더라도 그 구현이 부정확하거나 비효율적이면 프로그램은 정확히 동작하지 않는다.

### 6 단계 : 회고하기

문제 해결에 당장 직접적인 영향은 없지만 장기적으로 가장 큰 영향을 미치는 단계가 바로 회고이다. 회고란 자신이 문제를 해결한 과정을 돌이켜보고 개선하는 과정을 말한다.

한 번 푼 문제를 다시 본다고 해서 배우는 것이 있을까 하지만 `오히려 문제를 한번만 풀어서는 그 문제에서 배울 수 있는 것들을 다 배우지 못하는 경우가 더 많다.` 두번째로 풀때 더 효율적인 알고리즘을 찾을 수 있고 더 직관적인 방법을 찾을 수도 있다. 특히 이 장에서 다루는 문제 해결 기술은 외워야 할 의사코드도, 엄밀한 증명도 없는 추상적인 기술이기 때문에, 이들은 연마하기 위해서는 끊임없이 자신이 이 기술들을 어떻게 사용하고 있는지를 돌아보고 개선해야 한다. 효과적으로 회고를 수행하는 가장 좋은 방법은 `문제를 풀 때마다 코드와 함께 자신의 경험을 기록으로 남기는 것` 이다. `이때 문제의 간단한 해법과 함께 어떤 방식으로 접근했는지, 그리고 문제의 해법을 찾는데 결정적이었던 깨달음은 무엇이었는 지를 기록하면 좋다.`

`반대로 한번에 맞추지 못하는 경우에는 오답 원인도 꼭 적는것이 좋다.` 과거의 실수에서 배우기란 매우 어렵기 때문에 대개 한 실수를 반복하는데 반복적으로 틀리는 부분을 알게되고 결과적으로 실수를 줄일 수 있다.

또 다른 좋은 방법은 `같은 문제를 해결한 다른 사람의 코드를 보는 것이다.` 같은 문제를 해결한 사람의 코드도 백이면 백 모두 다르다. 다른 사람의 코드는 이해하기 어렵지만 자신이 생각하지 못했던 통찰을 얻을 수도 있다. `따라서 혼자서만 문제를 풀지 말고 그룹 스터디나 인터넷을 통해 다른 사람과 함께 공부하는 것이 매우 중요하다.

- 문제를 풀지 못할 때
  - 초보시절에는 한 문제에 너무 매달려 있는 것은 좋지 않다. 일정 시간이 지나도록 고민해도 답을 찾지 못할 때는 다른 사람의 소스코드나 풀이를 참조한다는 원칙을 세우고 이를 지키는 것이 좋다. 단 `다른 사람의 소스코드나 풀이를 참조할 때는 반드시 복기를 도압해야 한다` 처음 보는 기술이나 접근을 한번만에 자신의 것으로 만드는 것은 어렵지만 2,3 번 반복되면 내것이 된다.
- 주의
  - 물론 문제를 풀 때 항상 여기에서 설명한 단계에 하나하나 맞추어 가며 생각을 전개하라는 말은 아니다. 경험에 쌓임에 따라 따로 의식하지 않고 수행할 수 있도록 수행한다.

## 2.3 문제 해결 전략

쉽고 단순한 문제는 상관없지만 어려운 문제일 수록 다양한 방법을 시도해 답안을 찾아야 한다. 우리가 사용할 수 있는 `가장 일반적인 전략들을 살펴보자`

### 1. 직관과 체계적인 접근

문제 해결 전략에서 `가장 먼저 강조해야 할 것은 문제와 답의 구조에 대한 직관의 중요성이다.` 직관은 해당 문제를 해결하는 알고리즘이 대략적으로 어떤 형태를 가질지를 짐작할 수 있게 해준다. 물론 어떤 문제건 보자마자 바로 감을 잡을 수 있다면 이 책을 읽을 필요가 없지만 `직관 또한 시간이 지나면서 발달하는 것이고`, `직관을 발달시키기 위해서는 결국 막막한 문제들을 해결하며 경험을 차곡차곡 쌓아햐 하기 때문이다.` 우리는 막막한 문제를 해결하기 위해서 체계적인 방법을 택해야 한다. 여기서 `체계적인 방법이란 백지에서부터 시작해 문제를 해결하기 위한 기반을 차근차근 쌓아올리면서 점진적으로 전진하는 것을 의미한다.` 다음 문제 접근 방법들은 문제의 해법으로 직접 연결될 수도 있고 문제를 푸는데 필수적인 직관을 제공할 수도 있다.

### 2. 체계적인 접근을 위한 질문들

다음은 문제를 해결할 때 유용한 질문들의 목록으로, 많은 문제에 적용될 수 있다. 강력한 질문들부터 그 사용처가 제한되는 질문들의 순서대로 배열되어 있다.

1. 비슷한 문제를 풀어본 적이 있던가?

형태가 비슷하거나 관련된 문제를 풀어 본 적이 있다면 이전에 적용했던 방법과 비슷한 접근 방법을 사용할 거라고 예측할 수 있다. 이 때문에 대회에서 많은 문제를 푼 경험이 중요한 것이다. 물론 단순히 문제를 많이 푼다고 해서 좋은 것은 아니다. 풀어본 문제와 완전히 같은 문제를 만날 확률은 거의 없기 때문이다. 따라서 `기존에 접했던 문제가 온전히 경험이 되려면 그 원리를 완전히 이해하고 변형할 수 있어야 한다.` 예를 들어 다음 문제들을 살펴보자

```md
- 한 도시를 2 번 방문하지 않으면서 가장 긴 경로를 찾는 문제.
- 기차를 4 번 이하로 갈아타면서 가장 짧은 경로를 찾는 문제.
- 역 간 운행거리 중 가장 긴 구간이 가장 짧은 경로를 찾는 문제.
- 역 간 운행 거리 중 가장 짧은 구간이 가장 긴 경로를 찾는 문제.
- 가장 긴 구간과 가장 짧은 구간의 길이 차이가 가장 적은 경로를 찾는 문제
```

이들을 구분하려면 최단 경로 알고리즘을 단순히 알고 있는 것에 멈추지 않고 그 동작 과정과 원리를 완전히 이해해야 한다.

꼭 형태가 비슷하지 않더라도 문제의 목표가 같은 경우 또한 이런 사례에 속한다. `문제의 목적을 보고 적절한 접근 방법을 선택하기 위해서는 어떤 문제가 최적화 문제인지, 경우의 수 문제인지, 검색 문제인지 등을 분류하는 방법을 익히는 등 체계적인 방법으로 공부해야한다.`

2. 단순한 방법에서 시작할 수 있을까?

비슷한 문제를 본 적이 없거나, 해법이 곧장 적용되지 않는다면 어디서부터 시작해야 할까? `이 책은 "무식하게 풀 수 있을까?" 라는 질문으로 시작한다. 다시 말해 일단 시간과 공간 제약을 생각하지 않고 문제를 해결할 수 있는 가장 단순한 알고리즘을 만들어 보는것이다.`
이 전략의 일차적 목표는 간단하게 풀 수 있는 문제를 너무 복잡하게 생각해서 어렵게 푸는 실수를 방지하는 것이다. 컴퓨터는 생각보다 계산속도가 빠르기 때문에 복잡한 알고리즘을 쓰는 것보다 간단하고 느린 알고리즘으로도 충분하다는 것을 깨닫는 순간이 올것이다.

물론 단순한 방법으로 모든 문제들이 풀리진 않지만 이 방법이 `유용한 진짜 이유는 효율적인 알고리즘이라도 단순한 알고리즘을 기반으로 구성된 경우가 많기 때문이다.` 이런경우는 좀 더 효율적인 자료구조를 사용하거나, 계산 과정에서 같은 정보를 두 번 중복으로 계산하지 않는 등의 최적화를 적용해서 충분히 빨라질 때까지 알고리즘을 개선하는 식으로 문제를 풀 수 있다. 이 문제 해결 방법은 굉장히 강력하면서도 사고 과정의 큰 도약이 필요하지 않으므로, 어려운 문제를 접했을 때 한번쯤 시도해 볾 만하다.

단순한 방법은 효율성의 기준이 되어 적당히 빠르지 않더라도 개선 알고리즘이 얼마나 개선되었는지를 확인할 때 척도로 사용되기도 한다.

3. 내가 문제를 푸는 과정을 수식화할 수 있을까?

공부를 하다 보면 처음에 생각한 것과 완전히 다른, 새로운 방향에서 접근해야 풀리는 문제들도 있다. 이렇게 번뜩이는 영감이 필요한 문제를 만났을 때 시도할 수 있는 방법 중 하나는 손으로 여러 간단한 입력, 예를 들어 문제에 주어진 예제 입력을 직접 해결해 보는 것이다. 자신이 문제를 해결한 과정을 공식화해서 답을 만드는 알고리즘을 만들 수 있고, 그렇지 못하더라도 이 과정에서 알고리즘이 어떤 점을 고려해야 하는지를 알게 되기 때문이다.
`손으로 문제를 풀어보는 습관은 어떻게 문제를 풀어야 할지 감이 올 때도 유용하다`

4. 문제를 단순화할 수 없을까?

또 다른 강력한 문제 해결 도구는 주어진 문제의 좀더 쉬운 변형판을 먼저 풀어 보는 것이다. 문제의 제약 조건을 없앨 수도 있고, 계산해야 하는 변수의 수를 줄일 수도 있으며, 다차원의 문제를 1 차원으로 줄여서 표현할 수도 있다. 이것을 직접적으로 이용해 원래 문제를 풀어낼 수도 있다.

5. 그림으로 그려볼 수 있을까?

문제의 해법에 대한 직관을 얻을 수 있는 또 다른 방법은 문제에 관련된 그림을 그려 보는 것이다. `많은 사람들의 사고 체계는 숫자의 나열보다 기하학적 도형을 더 직관적으로 받아들이기 때문`이다. 이런 접근이 항상 통하는 것은 아니지만 문제를 해결할 결정적인 직관을 주는 경우가 많다.

6. 수식으로 표현할 수 있을까?

가능한 직관을 얻기 좋은 방향으로 사고를 전개하는 다른 접근 방식과 반대로, `평문으로 쓰여 있는 문제를 수식으로 표현하는 것도 도움이 되는 경우가 있다. 수식을 전개하거나 축약하는 등의 순수한 수학적 조작이 문제를 해결`하는데 큰 도움을 줄 수 있다.

7. 문제를 분해할 수 있을까?

또 다른 중요한 접근 방식은 더 다루기 쉬운 형태로 문제를 변형하는 것이다.
이 기술의 대표적인 예로 문제의 제약 조건을 분해하는 방법이 있다. 이 방법은 문제에 주어진 복잡한 조건을 더 단순한 형태를 갖는 조건의 집합으로 분해한다. `한개의 복잡한 조건보다 여러개의 단순한 조건을 다루는 것이 더 쉽다.`

8. 뒤에서부터 생각해서 문제를 풀 수 있을까?

또 다른 유용한 문제 변형 기법은 문제에 내재된 순서를 바꿔보는 것이다. (ex: 사다리 게임)

9. 순서를 강제할 수 있을까?

순서를 뒤집는 방법의 연정선으로, 순서가 없는 문제에 순서를 강제해서 문제를 푸는 방법도 있다.

10. 특정 형태의 답 만을 고려할 수 있을까?

순서를 강제하는 기법의 연장선으로 정규화 기법이 있다. `정규화란 우리가 고려해야 할 답들 중 형태가 다르지만 결과적으로는 똑같은 것들을 그룹으로 묶은 뒤, 각 그룹의 대표들만을 고려하는 방법이다.

## 2.4 느낀 점

다양한 문제 해결 전략들이 있다. 전략들을 소개하면서 여러가지 예시들을 책에서 들었는데 상당히 어려워서 파악하기가 까다롭고 제대로 이해하고 푼 문제가 거의 없다. 조금 더 실력을 체계적으로 쌓아보도록 하자.
