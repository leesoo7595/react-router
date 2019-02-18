
참고 : https://velopert.com/3417

# 1-1. 프로젝트 구성하기
## 프로젝트 생성 및 라이브러리 설치
먼저 create-react-app 으로 프로젝트를 생성하세요.

```
$ create-react-app react-router-tutorial
```
그 다음엔, 해당 프로젝트 디렉토리로 이동하여 리액트 라우터를 설치하세요.
```
$ yarn add react-router-dom
$ yarn add cross-env --dev
```
- react-router-dom: 브라우저에서 사용되는 리액트 라우터 입니다.
- cross-env: 프로젝트에서 NODE_PATH 를 사용하여 절대경로로 파일을 불러오기 위하여 환경 변수를 설정 할 때 운영체제마다 방식이 다르므로 공통적인 방법으로 설정 할 수 있게 해주는 라이브러리입니다.
## 프로젝트 초기화 및 구조 설정
### 파일 제거
- src/App.js
- src/App.css
- src/App.test.js
- src/logo.svg
### 디렉토리 생성
- `src/components`: 컴포넌트들이 위치하는 디렉토리입니다.
- `src/pages`: 각 라우트들이 위치하는 디렉토리 입니다.
- `src/client`: 브라우저 측에서 사용할 최상위 컴포넌트 입니다. 우리가 추후 서버사이드 렌더링을 구현 할 것이기 때문에 디렉토리를 따로 구분하였습니다. (서버사이드 렌더링을 할 때에는 서버 전용 라우터를 써야합니다.) 여기서 라우터를 설정합니다.
- `src/server`: 서버측에서 사용 할 리액트 관련 코드를 여기에 넣습니다.
- `src/shared`: 서버와 클라이언트에서 공용으로 사용되는 컴포넌트 App.js 가 여기에 위치합니다.
- `src/lib`: 나중에 웹 연동을 구현 할 때 사용 할 API와 코드스플리팅 할 때 필요한 코드가 여기에 위치합니다.
