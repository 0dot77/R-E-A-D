# TIL 2022.05.16

✏️ 오늘 읽은 범위 : 2장 실용주의 접근법

```
💭 책에서 기억하고 싶은 내용을 적기
```

- 좋은 설계는 나쁜 설계보다 바꾸기 쉽다. p.39
  - ETC 원칙을 따른다. 바꾸기 더 쉽게 Easier to Change. ETC. 이게 전부다.
  - 왜 단일 책임 원칙 *single responsibility principle*이 유용한가? 요구 사항이 바뀌더라도 모듈 하나만 바꿔서 반영할 수 있기 때문이다.
  - 왜 이름 짓기가 중요한가? 이름이 좋으면 코드가 읽기 쉬워지고, 코드를 바꾸려면 코드를 읽어야 하기 때문이다.
  - '내가 방금 한 일이 전체 시스템을 바꾸기 쉽게 만들었을까, 어렵게 만들었을까?' 파일을 저장할 때마다 물어보라.
- 모든 코드를 교체할 수 있게 작성해야 한다. 교체 가능하게 작성하라는 말은 코드의 결합도를 낮추고 응집도를 높이라는 이야기일 뿐이다. p.40
- 엔지니어링 일지에 현재 상황과 여러분의 선택, 그리고 변경 사항에 대한 추측을 정리해 둬라. 그리고 소스 코드에 이에 대한 표시를 남겨 둬라.

> 모든 지식은 시스템 내에서 단 한 번만, 애매하지 않고, 권위 있게 표현되어야 한다. p.43

- 함수 이름이 함수가 하는 일을 알려준다. p.48
- 개발자 간의 중복을 대처하려면 크게는 의사소통을 잘하는 튼튼하고 유대가 돈독한 팀을 만들어야 한다. p.53
- 일상적으로든 코드 리뷰를 통해서든 다른 사람의 소스 코드와 문서를 반드시 읽어라. <mark>다른 사람의 것을 기웃거리는 게 아니고, 거기서 배우는 것이다.</mark> 그리고 기억하라. 접근은 상호적이다. 다른 사람이 여러분의 코드를 들여다보고 건드린다고 해서 기분 나빠하지 말 일이다.
- 하나가 바뀌어도 나머지에 어떤 영향도 주지 않으면 서로 직교한다고 할 수 있다. 잘 설계된 시스템에서는 데이터베이스 코드가 사용자 인터페이스와 서로 직교할 것이다. 데이터베이스에 영향을 주지 않으면서 인터페이스를 바꿀 수 있고, 또한 인터페이스를 바꾸지 않으면서 데이터베이스를 교체할 수 있다. p.55
  > 관련 없는 것들 간에 서로 영향이 없도록 하라 p.56
- 컴포넌트들이 각기 격리되어 있으면 어느 하나를 바꿀 때 나머지 것들을 걱정하지 않아도 된다. 해당 컴포넌트 외부 인터페이스를 바꾸지 않는 한 전체 시스템으로 퍼져 나가는 문제를 일으키지는 않으리라고 확신할 수 있다. 직교적인 시스템을 작성하면 두 가지 큰 장점이 있다. 바로 생산성 향상과 리스크 감소다. p.57
- 시스템은 서로 협력하는 모듈의 집합으로 구성되어야하고, 각 모듈은 다른 부분과 독립적인 기능을 구현해야 한다. p.58
- '특정 기능에 대한 요구 사항을 대폭 변경하는 경우 몇 개의 모듈이 영향을 받는가?' 직교적인 시스템에서는 답이'하나'여야 한다. p.59
  > 자신의 힘으로 제어할 수 없는 속성에 의존하지 마라. p.60
- '부끄럼쟁이' 코드를 작성하라. 즉, 불필요한 것은 다른 모듈에 보여 주지 않으며, 다른 모듈의 구현에 의존하지 않는 코드를 작성하라. p.61
- <mark>자신이 작성하는 코드를 항상 비판적으로 바라보는 습관을 길러라.</mark>
- 여러분이 할 수 있는 것은 바꾸기 쉽게 만드는 것이다. 외부의 API를 여러분이 만든 추상화 계층 뒤로 숨겨라. p.69
- 예광탄 코드는 한 번 쓰고 버리려고 만드는 것이 아니다. 앞으로도 계속 사용할 코드다. 예광탄 코드도 다른 제품 코드와 마찬가지로 오류 검사, 올바른 구조, 문서화, 자체 검사를 갖추어야 한다. p.75
- 소프트웨어 프로토 타입은 위험 요소를 분석하고 노출시킨 후, 이를 매우 저렴한 비용으로 바로잡을 기회를 얻는 것이다.
  - 사용자 인터페이스 프로토타입은 화이트보드에 그림을 그려서 만들 수도 있고, 그림판 프로그램, 인터페이스 빌더 등을 이용해 기능은 구현하지 않고 만들어볼 수도 있다. p.80
    > 코드와 함께 일정도 반복하며 조정하라. p.101

```
🧐 오늘 읽은 소감은? 떠오르는 생각을 가볍게 적기
```

- 아직 코드 한 줄 쓰는데에 급급한 수준이기 때문에, ETC나... 여타 좋은 패턴들을 사용할 가능성을 스스로 저버리고 있는 경우가 많았던 것 같다. 코드를 작성하면서 최소한으로 적용해볼 수 있는 것들부터 천천히 연습해보고자 한다.

```
🔎 궁금한 내용이 있거나, 잘 이해되지 않는 내용이 있다면?
```

- 도메인 언어
  - RSpec
  - Cucumber
  - Phoenix router
  - Ansible
