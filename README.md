# 23-React1

# 7주차
2023-04-13

### Chapter.07 훅(p.208)

1. Hook
: 원래 존재하는 어떤 기능에 마치 갈고리를 거는 것처럼 끼어 들어가 같이 수행되는 것
: 리액트의 state와 생명주기 기능에 갈고리를 걸어 원하는 시점에 정해진 함수를 실행되도록 만든 것

2. side effect(=부작용)
useEffect(effect function, an array of dependencies);
의존성 배열 없이 사용한다면? 'DOM이 변경된 이후에 해당 이펙트 함수를 실행하라'는 의미로 리액트는 받아들인다.
- useEffect()에서 리턴하는 함수는 컴포넌트가 마운트 해제될때 호출됩니다.

3. useMemo() Hook
: Memoized value를 return하는 Hook
- useMemo()로 전달된 함수는 렌더링이 일어나는동안 실행된다는 점

4. useCallback() Hook
: useMemo()과 유사한 역할을 함
: 차이점) 값이 아닌 함수를 반환

5. Memoization(최적화)
- 함수 호출 결과를 저장해 두었다가, 같은 입력값으로 함수를 호출하면 이전에 저장해놨던 호출 결과를 바로 반환하는 것

6. useRef() Hook
: Reference를 사용하기 위한 Hook
: 변경가능한 .current라는 속성을 가진 하나의 상자
Reference(=특정 컴포넌트에 접근할 수 있는 객체)
- 매번 랜더링될 때마다 항상 같은 ref객체를 반환한다

7. Hook의 규칙
- 무조건 최상위 레벨에서만 호출
- 반복문, 조건문, 중첩된 함수 안에서 호출X
- 컴포넌트가 렌더링될 때마다 매번 같은 순서로 호출
- 리액트 함수 컴포넌트에서만 호출
- 직접 만든 커스텀 훅에서만 호출가능

<시험범위> 
~ Chapter.07 훅까지
A4지시서, 순서대로 만들어라!, 오픈북+인터넷검색 가능(카톡X, 옆사람이랑 말하기X, 챗GPT X, node모듈만 올리지 말기)
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
