# remix tutorial

## directory 구조 및 파일들

### 🛠 빌드하면 생기는 디렉토리들 (`.gitignore`에 나열되어 있음)

- `.cache/`: remix가 내부적으로 사용하는 것
- `build/`: 서버측 코드
- `public/build/`: 모든 클라이언트측 코드 

### 🎁 `app`

- `app/`: 모든 remix 코드들
- `app/entry.client.tsx`: 앱이 브라우저에서 로드될 때 실행되는 javascript 첫번째 bit
- `app/entry.server.tsx`: 앱이 서버에 도달할 때 실행되는 javascript 첫번째 bit. 이 파일에서 react 앱을 `string/stream`으로 렌더링하고 클라이언트에 대한 응답으로 보냄
- `app/root.tsx`: 앱의 루트 구성 요소를 배치함. 여기서 `<html>` 요소를 렌더링함
- `app/routes/`: 모든 라우트 모듈들이 위치할 곳. remix는 이 디렉토리의 파일을 사용하여 파일 이름 기반으로 앱의 url 경로를 생성함

