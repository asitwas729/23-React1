# 23-React1

# 5주차
2023-03-30



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
