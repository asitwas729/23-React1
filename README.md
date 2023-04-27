# 23-React1

# 9주차
2023-04-27

### Chapter.08 이벤트 핸들링(p.246)
<이벤트 처리하기>
- DOM의 이벤트<br>
: 이벤트의 이름을 모두 소문자로 표기<br>
: 이벤트를 처리할 함수를 문자열로 전달<br>
- 리액트의 이벤트<br>
: 이벤트의 이름을 카멜 표기법으로 표기<br>
: 이벤트를 처리할 함수를 그대로 전달<br>
- 이벤트 핸들러<br>
: 이벤트가 발생했을 때 해당 이벤트를 처리하는 함수<br>
: 이벤트 리스너라고 부르기도 함<br>
: 클래스 컴포넌트<br>
&nbsp;&nbsp;&nbsp; : 클래스의 함수로 정의하고 생성자에서 바인딩해서 사용<br>
&nbsp;&nbsp;&nbsp; : 클래스 필드 문법도 사용가능<br>
- 함수 컴포넌트<br>
: 함수 안에 함수로 정의하거나 arrow function을 사용해서 정의
<br><br>
### Chapter.09 조건부 렌더링(p.266)
: 소괄호안에 있는 것
- 조건부 렌더링<br>
: 조건에 따라 렌더링의 결과가 달라지도록 하는 것<br>
- 엘리먼트 변수<br>
: 리액트 엘리먼트를 변수처럼 저장해서 사용하는 방법<br>
- 인라인 조건<br>
: 조건문을 코드 안에 집어넣는 것<br>
: 인라인 If<br>
- If문을 필요한 곳에 직접 집어넣어서 사용하는 방법<br>
: 논리 연산자 &&를 사용 （AND 연산）<br>
- 앞에 나오는 조건문이 tr니e일 경우에만 뒤에 나오는 엘리먼트를 렌더링<br>
: 인라인 If-Else<br>
: If—else문을 필요한 곳에 직접 집어 넣어서 사용하는 방법<br>
- 삼항연산자 ?를 사용<br>
- 앞에 나오는 조건문이 true면 첫 번째 항목을 리턴 false면 두 번째 항목을 리턴<br>
: 조건에 따라 각기 다른 엘리먼트를 렌더링하고 싶을 때 사용<br>

# 7주차
2023-04-13

### Chapter.07 훅(p.208)

1. Hook<br>
: 원래 존재하는 어떤 기능에 마치 갈고리를 거는 것처럼 끼어 들어가 같이 수행되는 것<br>
: 리액트의 state와 생명주기 기능에 갈고리를 걸어 원하는 시점에 정해진 함수를 실행되도록 만든 것
<br><br>

2. side effect(=부작용)<br>
useEffect(effect function, an array of dependencies);<br>
의존성 배열 없이 사용한다면? 'DOM이 변경된 이후에 해당 이펙트 함수를 실행하라'는 의미로 리액트는 받아들인다.
- useEffect()에서 리턴하는 함수는 컴포넌트가 마운트 해제될때 호출됩니다.<br><br>

3. useMemo() Hook<br>
: Memoized value를 return하는 Hook
- useMemo()로 전달된 함수는 렌더링이 일어나는동안 실행된다는 점
<br><br>

4. useCallback() Hook<br>
: useMemo()과 유사한 역할을 함<br>
: 차이점) 값이 아닌 함수를 반환<br>
<br>

5. Memoization(최적화)<br>
- 함수 호출 결과를 저장해 두었다가, 같은 입력값으로 함수를 호출하면 이전에 저장해놨던 호출 결과를 바로 반환하는 것<br><br>

6. useRef() Hook<br>
: Reference를 사용하기 위한 Hook<br>
: 변경가능한 .current라는 속성을 가진 하나의 상자<br>
Reference(=특정 컴포넌트에 접근할 수 있는 객체)
- 매번 랜더링될 때마다 항상 같은 ref객체를 반환한다<br><br>

7. Hook의 규칙
- 무조건 최상위 레벨에서만 호출
- 반복문, 조건문, 중첩된 함수 안에서 호출X
- 컴포넌트가 렌더링될 때마다 매번 같은 순서로 호출
- 리액트 함수 컴포넌트에서만 호출
- 직접 만든 커스텀 훅에서만 호출가능<br><br>

<시험범위> 
~ Chapter.07 훅까지<br>
A4지시서, 순서대로 만들어라!, 오픈북+인터넷검색 가능<br>
(카톡X, 옆사람이랑 말하기X, 챗GPT X, node모듈만 올리지 말기)<br>
시험시간 : PM 1:00~1:50


# 6주차
2023-04-06

실행방법

1. npm start
2. index.js변경
```jsx
import Comment from './chapter_05/Comment';

<React.StrictMode>
    <Comment />
  </React.StrictMode>
```

State

1. 리액트 컴포넌트의 상태를 의미(컴포넌트의 변경가능한 데이터)

<특징>

1. 자바스크립트 객체일뿐...,
2. 함수형에서는 useState()라는 함수 사용


# 5주차
2023-03-30

질병결석함

Element

리액트 엘리먼트는 JS 객체 형태로 존재한다.
컴포넌트, 속성 및 내부의 모든 children을 포함하는 일반 JS 객체.
리액트 엘리먼트의 가장 큰 특징은 불변성
즉, 한 번 생성된 Children이나 속성을 바꿀 수 없다.


# 4주차
2023-03-23

1. README.md 백업
2. local에 있는 저장소 이름 바꾸기 or 삭제
3. 새 프로젝트 생성(23-React1)
4. README.md 덮어쓰기
5. GitHub 23-React 삭제하기
6. 로컬에서 23-React1 push하기
7. GitHub 저장소 확인하기

ReactJS

```jsx
const element = <h1>Hello, World!</h1>;
```

jsx이란?

- 자바스크립트의 확장 문법
- JSX 코드를 자바스크립트 코드로 변환하는 역할을 하는 것
Ex)React의 createElement()함

```jsx
// JSX사용
const element =(
	<hl className="greeting">
		Hello, world!
	</hl>
)

// JSX사용안함 
const element = React.createElement(
	'hl',
	{ className： 'greeting' },
	'Hello, world!'
)
```

jsx 장점

- 코드 간결해짐
- 가독성↑
- 생산성↑
- 해킹 방법을 보안하여 보안성이 높아짐
Injection Attack: 입력창에 소스코드를 입력하여 실행되는 해킹 방법

jsx 사용법

- HTML과 자바스크립트가 섞인 형태로 코드를 작성
- HTML 코드를 사용하다가 중간에 자바스크립트 코드를 사용하고 싶으면 중괄호 사용




# 3주차
2023-03-16

요청하는 페이지를 DB에서 데이터를 받아서 T라는 페이지가 생기고 

동기식 : 바꾼 페이지를 고대로 가져옴, 밑장 모두 가지고있음(인스타)

비동기식 : 바꾼 부분만 보내줌, 밑에 몇장까지만 가지고있음(인스타)

리액트 네이티브 → 크로스 플랫폼

CDN 링크 배포할때는 min탭을 사용(줄바꿈을 없앤버전)

# 2주차
2023-03-09

cmd - git version확인 

```jsx
git --version

git -v
```

vscode github연동
