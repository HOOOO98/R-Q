# 💁‍♂️리액트 100문 100답
리액트를 공부하면서 생기는 궁금증과 난해한 개념을 질문하고<br>
이를 해결함으로써 온전한 개념을 습득하는 것이 이 페이지의 목표입니다.

- 두괄식으로 답변하기
- 질문의 의도를 파악하고 답변과 연관된 주제 서사적으로 풀어내기
- 정의+문제점+해결책
- 정의+연관된주제

# 목차
| 번호 | 질문 |
| --- |---|
|  1  | [리액트가 어떻게 작동하는지 간단히 설명해주세요.](#리액트가-어떻게-작동하는지-간단히-설명해주세요) |
|  2  | [상태(State)와 속성(Props)의 차이는 무엇이며 언제 어떻게 사용하나요?](#상태state와-속성props의-차이는-무엇이며-언제-어떻게-사용하나요) |
|  4  | [JSX란 무엇이며 왜 사용하나요?](#jsx란-무엇이며-왜-사용하나요) |
|  5  | [라이프사이클 메서드(Lifecycle Methods)의 종류와 언제 사용하고 어떤 역할을 하는지 설명해보세요.](#라이프사이클-메서드lifecycle-methods의-종류와-언제-사용하고-어떤-역할을-하는지-설명해보세요) |
|  6  | [React Hooks가 무엇이며 어떻게 사용하나요]() |
|  7  | [상태 관리 라이브러리인 Redux 또는 MobX는 어떻게 동작하며 언제 사용하나요?]() |
|  8  | [리액트 컴포넌트의 키(key) 역할은 무엇이며 왜 중요한가요?]() |
|  9  | []() |
|  10  | []() |
|  11  | []() |
|  12  | []() |
|  13  | []() |
|  14  | []() |
|  15  | []() |
|  16  | []() |
|  17  | []() |
|  18  | []() |
|  19  | []() |
|  20  | []() |
|  21  | []() |
|  22  | []() |
|  23  | []() |
|  24  | []() |
|  25  | []() |
|  26  | []() |
|  27  | []() |
|  28  | []() |
|  29  | []() |
|  30  | []() |
|  31  | []() |
|  32  | []() |
|  33  | []() |
|  34  | []() |
|  35  | []() |
|  36  | []() |
|  37  | []() |
|  38  | []() |
|  39  | []() |
|  40  | []() |
|  41  | []() |
|  42  | []() |
|  43  | []() |
|  44  | []() |
|  45  | []() |
|  46  | []() |
|  47  | []() |
|  48  | []() |
|  49  | []() |
|  50  | []() |
|  51  | []() |
|  52  | []() |
|  53  | []() |
|  54  | []() |
|  55  | []() |
|  56  | []() |
|  57  | []() |
|  58  | []() |
|  59  | []() |
|  60  | []() |
|  61  | []() |
|  62  | []() |
|  63  | []() |
|  64  | []() |
|  65  | []() |
|  66  | []() |
|  67  | []() |
|  68  | []() |
|  69  | []() |
|  70  | []() |
|  71  | []() |
|  72  | []() |
|  73  | []() |
|  74  | []() |
|  75  | []() |
|  76  | []() |
|  77  | []() |
|  78  | []() |
|  79  | []() |
|  80  | []() |
|  81  | []() |
|  82  | []() |
|  83  | []() |
|  84  | []() |
|  85  | []() |
|  86  | []() |
|  87  | []() |
|  88  | []() |
|  89  | []() |
|  90  | []() |
|  91  | []() |
|  92  | []() |
|  93  | []() |
|  94  | []() |
|  95  | []() |
|  96  | []() |
|  97  | []() |
|  98  | []() |
|  99  | []() |
|  100  | []() |


### 리액트가 어떻게 작동하는지 간단히 설명해주세요
리액트는 페이스북에서 개발한 JavaScript 라이브러리로, 사용자 인터페이스를 만들기 위한 도구입니다.<br>
리액트는 컴포넌트라는 작은 조각들로 구성되며, 이러한 컴포넌트들은 UI를 표현하고 이벤트 처리, 데이터 상태 관리를 담당합니다. <br>
리액트는 Virtual DOM이라는 가상의 문서 객체 모델을 사용하여 화면 갱신을 효율적으로 처리하며, 변경된 부분만 실제 DOM에 업데이트하여 성능을 향상시킵니다. <br>
이렇게 함으로써 사용자 경험을 개선하면서도 개발자에게 유연한 개발 환경을 제공합니다.

[맨 위로 올라가기](#목차)

---

### 상태(State)와 속성(Props)의 차이는 무엇이며 언제 어떻게 사용하나요
상태(State)는 컴포넌트 내부에서 관리되는 데이터를 나타냅니다.<br>
이 데이터는 컴포넌트가 렌더링되고 상호작용하는 동안 변경될 수 있습니다.<br>
주로 컴포넌트 내에서 동적인 데이터를 저장하고 관리할 때 사용됩니다. <br>
예를 들어, 사용자 입력, API 요청 결과, 컴포넌트 내부의 토글 상태 등을 관리하는 데 상태를 사용합니다.<br>
상태는 클래스형 컴포넌트에서는 this.state로, 함수형 컴포넌트에서는 useState 훅을 사용하여 정의하고 업데이트합니다.<br>

속성(Props)은 컴포넌트로 전달되는 데이터를 나타냅니다.<br>
다른 컴포넌트에서 이 데이터를 설정하고, 부모 컴포넌트로부터 자식 컴포넌트로 전달됩니다.<br>
주로 컴포넌트 간의 데이터 전달에 사용됩니다. <br>
부모 컴포넌트는 자식 컴포넌트에게 데이터를 전달하거나, 자식 컴포넌트가 동일한 속성을 다르게 렌더링하도록 할 때 속성을 사용합니다.<br>
속성은 컴포넌트를 사용할 때 JSX 요소의 속성으로 전달하며, 컴포넌트 내부에서는 props 객체로 접근할 수 있습니다.<br>

올바르게 상태(State)와 속성(Props)를 활용하면 코드가 더 모듈화되며, 컴포넌트의 재사용성이 향상됩니다.<br>
또한, 애플리케이션의 데이터 흐름이 더 명확해지고 유지보수가 쉬워집니다.

[맨 위로 올라가기](#목차)

---

### JSX란 무엇이며 왜 사용하나요
JSX는 자바스크립트 코드 내에서 HTML과 유사한 문법을 사용하여 UI 요소를 작성할 수 있게 해주는 문법입니다.<br>
이를 통해 개발자는 컴포넌트와 UI 요소를 더 직관적으로 정의하고 조합할 수 있습니다.<br>

JSX에서 여러 요소를 래핑하지 않고 반환하기 위해 <></>(프래그먼트)를 사용할 수 있습니다.<br>
이는 불필요한 DOM 요소를 생성하지 않고 컴포넌트를 깔끔하게 구성하는 데 도움이 됩니다.<br>

[맨 위로 올라가기](#목차)

---

### 라이프사이클 메서드(Lifecycle Methods)의 종류와 언제 사용하고 어떤 역할을 하는지 설명해보세요
리액트의 라이프사이클 메서드는 컴포넌트가 생성, 업데이트, 제거되는 과정 중에 호출되는 메서드들로, 이들을 통해 컴포넌트의 동작을 제어할 수 있습니다.<br>
리액트 16.3 버전부터는 일부 라이프사이클 메서드가 더 이상 권장되지 않으며, 대신 React Hooks를 사용하는 것이 좋습니다. <br>

componentDidMount는 컴포넌트가 생성된 후(render 메서드 이후) 호출되며, 초기화 및 데이터 가져오기와 같은 작업에 적합합니다.<br>
컴포넌트가 화면에 렌더링된 직후에 호출됩니다.<br>

componentDidUpdate는 컴포넌트가 업데이트된 후(render 메서드 이후) 호출되며, 업데이트 이후의 작업을 처리하는 데 사용됩니다. <br>
이전 상태 및 속성과 현재 상태 및 속성을 비교하여 변경 사항을 감지할 수 있습니다.<br>
컴포넌트가 업데이트되었을 때 호출됩니다.<br>

componentWillUnmount는 컴포넌트가 파괴되기 전에(clean up) 호출되며, 리소스 해제나 이벤트 리스너 제거와 같은 정리 작업을 수행하는 데 사용됩니다.<br>
컴포넌트가 파괴되기 직전에 호출됩니다.<br>

shouldComponentUpdate는 컴포넌트가 업데이트되기 전(render 메서드 호출 전)에 호출되며, 컴포넌트가 리렌더링되어야 하는지 여부를 결정하는 작업에 사용됩니다. <br>
이 메서드에서 true를 반환하면 업데이트가 허용되고, false를 반환하면 업데이트가 거부됩니다.<br>
컴포넌트가 업데이트되기 전에 호출됩니다.<br>

static getDerivedStateFromProps는 컴포넌트의 속성(props)이 변경될 때 호출되며, 새로운 상태(state)를 반환하거나 null을 반환하여 상태 업데이트를 수행합니다.<br>
컴포넌트의 속성(props)이 변경될 때 호출됩니다.<br>

componentDidCatch는 컴포넌트 내부에서 발생한 예외를 처리하며, 에러 경계(error boundary)를 설정하여 애플리케이션 전체의 오류 처리를 관리합니다.<br>
하위 컴포넌트에서 오류가 발생했을 때 호출됩니다.<br>

[맨 위로 올라가기](#목차)
