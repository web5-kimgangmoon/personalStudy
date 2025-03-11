## react

1. **React 16.x (2017)**: 기능 추가

   - **Error Boundaries**: 컴포넌트에서 오류가 발생했을 때 애플리케이션이 크래시 되는 것을 방지하기 위해, 오류를 잡을 수 있는 ErrorBoundary 컴포넌트를 추가했습니다.

   - **Fiber Architecture**: 리액트는 내부적으로 Fiber 아키텍처로 변경되었습니다. 비동기 렌더링을 지원하여 UI가 더 부드럽고 반응성이 좋습니다.

   - **Fragments**: 여러 자식을 반환할 수 있는 <Fragment>를 도입하여, 불필요한 DOM 노드를 추가하지 않고 여러 자식 요소를 묶을 수 있게 되었습니다.

   - **Portals**: ReactDOM.createPortal을 사용해 자식 요소를 DOM 트리의 다른 위치로 이동할 수 있게 되었습니다. 이를 통해 모달, 툴팁 등의 UI 구성 요소를 만들 때 유용합니다.

2. **React 17.x (2020)**: 안정성 위주

   - **새로운 JSX Transform**: React.createElement 호출을 자동으로 삽입하는 대신, import React from 'react' 구문을 제거할 수 있게 해주는 새로운 JSX 변환 방식이 도입되었습니다. 이 덕분에 JSX 문법을 사용하는 데 React를 명시적으로 가져올 필요가 없어졌습니다.

   - **타입스크립트 지원 개선**: 리액트 17은 타입스크립트와의 호환성을 높이기 위해 많은 개선이 있었습니다.

   - **이벤트 핸들링 개선**: 이벤트 처리 방식이 조금 개선되었고, 기존의 리액트 이벤트 시스템에서 발생할 수 있는 문제들을 해결했습니다.

3. **React 18.x (2022)**: 동시 렌더링

   - **Concurrent Mode (동시 렌더링 모드)**: 새로운 ReactDOM.createRoot와 Suspense 기능을 도입하여 애플리케이션이 더 반응성 있게 렌더링될 수 있도록 했습니다.

   - **Automatic Batching**: 여러 상태 업데이트를 묶어서 한번에 렌더링하는 자동 배칭 기능이 도입되었습니다. 여러 번의 상태 변경을 하나의 렌더링 작업으로 합쳐 성능을 개선할 수 있습니다.

   - **useId Hook**: 서버 측 렌더링(SSR) 환경에서 고유한 ID 값을 안전하게 생성할 수 있는 useId 훅이 도입되었습니다.

   - **Suspense for Data Fetching**: Suspense는 데이터 로딩 중에 컴포넌트를 지연시킬 수 있는 기능으로, 이제 Suspense를 데이터 페칭에 사용할 수 있게 되었습니다.

4. **React 19.x (2023)**: 기능 확장 및 최적화

   - **React Server Components**: 서버에서만 렌더링되는 컴포넌트를 사용할 수 있는 기능이 실험적으로 도입되었습니다. 이는 클라이언트와 서버 간의 데이터와 렌더링을 효율적으로 처리하는 데 큰 도움이 됩니다.

   - **React Suspense for Data Fetching의 개선**: React 18에서 도입된 Suspense의 데이터 페칭 기능이 더욱 개선되어, 더 많은 라이브러리와 통합이 가능해졌습니다.

   - **Server-side Streaming 개선**: React 19에서는 서버 측 스트리밍이 개선되어, 서버에서 빠르게 HTML을 클라이언트로 보내는 것이 더욱 효율적으로 처리됩니다.

   - **향상된 개발자 도구**: 새로운 개발자 도구가 추가되어, 컴포넌트 트리, 상태 관리 및 렌더링 흐름을 추적하는 데 유용한 기능들이 제공됩니다.

5. 버전별 추가된 주요 기능들

   - **React 16.x**: Fiber 아키텍처, Error Boundaries, Fragments, Portals

   - **React 17.x**: JSX Transform, 타입스크립트 지원 개선, 이벤트 핸들링

6. 개선

   - **React 18.x**: Concurrent Mode, Automatic Batching, useId Hook, Suspense 개선

   - **React 19.x**: Server Components, 개선된 Suspense, 서버 측 스트리밍 개선

7. 결론

   리액트는 버전이 올라갈수록 성능 최적화, 개발자 경험 개선, 서버 사이드와 클라이언트 사이의 흐름 제어에 많은 집중을 하며, **동시 렌더링(Concurrent Rendering)**이나 **자동 배칭(Auto Batching)**과 같은 중요한 개념들이 도입되었습니다. 각 버전의 주요 기능을 파악하고, 최신 버전의 새로운 기능을 활용하면 더 빠르고 효율적인 애플리케이션을 만들 수 있습니다.

## next

넥스트.js는 주요 버전 업데이트가 자주 이루어진다.

1. **Next.js 9.x (2019)**

   - **정적 사이트 생성(SSG) 지원**: getStaticProps와 getStaticPaths 함수가 도입되어, 정적 페이지를 사전 렌더링할 수 있게 되었습니다.

   - **동적 라우팅(Dynamic Routing)**: getStaticPaths를 사용하여 동적 라우트를 위한 정적 페이지 생성이 가능해졌습니다.

   - **API 라우트(API Routes)**: Next.js 내에서 API를 만들 수 있는 기능이 추가되었습니다. 이를 통해 백엔드 서버 없이 프론트엔드에서 직접 API를 처리할 수 있습니다.

   - **Image Component**: Next.js는 기본적으로 이미지 최적화를 제공하는 next/image 컴포넌트를 도입하여 이미지 로딩 성능을 개선했습니다.

   - **개선된 CSS와 Sass 지원**: Next.js는 이제 CSS 및 Sass의 내장 지원을 제공하여, 별도의 설정 없이 CSS와 Sass 파일을 쉽게 사용할 수 있습니다.

2. **Next.js 10.x (2020)**: 성능과 개발자 경험을 위한 많은 기능들이 추가되었습니다.

   - **자동 이미지 최적화**: next/image 컴포넌트가 이미지의 크기, 형식 등을 자동으로 최적화해줍니다.

   - **새로운 next/script 컴포넌트**: 외부 스크립트를 추가할 때 성능 최적화를 위한 next/script 컴포넌트가 도입되었습니다.

   - **서버 측에서 지원되는 Web Vitals**: 웹 성능 지표(Core Web Vitals)를 자동으로 수집하고 분석할 수 있는 기능이 도입되었습니다.

   - **인터내셔널리제이션 (i18n) 지원**: Next.js 10은 다국어 웹사이트를 만들 수 있도록 내장된 국제화(i18n) 지원을 추가했습니다.

   - **스크롤 복원(Scroll Restoration)**: 페이지를 새로 고침 후 이전 위치로 스크롤을 복원하는 기능이 추가되었습니다.

   - **이미지 최적화**: next/image는 이미지 최적화와 관련된 여러 가지 자동화 기능을 제공하며, 레이지 로딩(lazy loading)을 기본으로 지원합니다.

3. **Next.js 11.x (2021)**: 개발자 경험을 대폭 향상시키는 기능들이 도입되었습니다.

   - **Webpack 5 기본 지원**: Next.js는 Webpack 5를 기본적으로 지원하며, 더 빠른 빌드 시간과 향상된 성능을 제공합니다.

   - **Script Optimization**: \<Script \/\> 컴포넌트를 사용하여 스크립트 로딩을 최적화하고, 비동기/지연 로딩을 지원합니다.

   - **스타일드 컴포넌트 지원**: Next.js 11은 스타일드 컴포넌트와 Emotion을 기본적으로 지원하여 스타일링을 더욱 쉽게 할 수 있도록 했습니다.

   - **Live Editing**: Next.js 11에서는 실시간 편집이 가능하며, 웹팩 핫 리로드(Hot Reloading) 기능이 개선되었습니다.

   - **Middleware**: 미들웨어를 사용하여 요청을 가로채고, 서버 측에서 처리를 할 수 있는 기능이 추가되었습니다. 예를 들어, 요청 헤더에 따라 응답을 변경하는 등의 작업을 할 수 있습니다.

   - **Conformance**: Next.js 11은 ESLint와 Prettier 설정을 통해 코드 품질과 일관성을 유지하는 데 도움을 주는 기능들을 강화했습니다.

4. **Next.js 12.x (2022)**: 성능 최적화와 서버 측 렌더링(SSR), Edge 기능 강화에 중점을 둔 버전입니다.

   - **Middleware on the Edge**: Next.js는 서버의 엣지(Edge) 환경에서 미들웨어를 실행할 수 있는 기능을 추가했습니다. 이를 통해 더 빠른 응답을 제공할 수 있습니다.

   - **Rust Compiler**: Rust로 작성된 Webpack 5 빌드 최적화 컴파일러가 도입되어 빌드 속도가 획기적으로 향상되었습니다.

   - **React 18 지원**: Next.js 12는 React 18의 새로운 기능을 지원합니다. 특히 동시 렌더링(Concurrent Rendering) 및 서버 측에서의 Suspense와 같은 기능을 지원합니다.

   - **URL Imports**: 이제 웹에서 바로 URL로부터 JavaScript 모듈을 가져오는 기능을 사용할 수 있습니다.

   - **SWC 컴파일러**: SWC(Speedy Web Compiler)가 Webpack과 Babel을 대체할 수 있게 되어 빌드 성능을 크게 향상시켰습니다.

   - **ES Modules**: ES 모듈을 더 나은 지원을 제공하여, 특히 코드 분할 및 트리 쉐이킹(tree-shaking)에서 더 큰 효율성을 얻을 수 있습니다.

5. **Next.js 13.x (2023)**:앱 디렉터리(App Directory)와 React Server Components를 중심으로 한 큰 변화를 도입했습니다.

   - **App Directory**: Next.js는 이제 /app 디렉터리를 도입하여, React의 새로운 Server Component와 함께 작동하는 방식으로 애플리케이션을 구성할 수 있게 되었습니다.

   - **React Server Components**: 서버에서만 렌더링되고 클라이언트 측에는 전달되지 않는 서버 컴포넌트를 지원하여 서버와 클라이언트의 역할을 명확히 구분할 수 있습니다.

   - **서버 측의 Suspense 개선**: Suspense를 서버 측에서 더 잘 활용할 수 있도록 개선되었습니다. 이로 인해 서버에서 비동기 작업을 더 잘 처리할 수 있습니다.

   - **next/font**: 글꼴 최적화를 위한 next/font가 도입되어, 웹 폰트의 로딩 성능을 개선할 수 있게 되었습니다.

   - **라우팅 개선**: 새로운 파일 기반 라우팅 시스템이 개선되었으며, 더 많은 동적 라우팅 기능을 지원합니다.

6. 넥스트.js 버전별 주요 기능 요약

   1. **Next.js 9.x**: 정적 사이트 생성(SSG), API 라우트, 이미지 최적화
   2. **Next.js 10.x**: 자동 이미지 최적화, Script 최적화, 국제화(i18n) 지원
   3. **Next.js 11.x**: Webpack 5 기본 지원, Script 최적화, Live Editing, Middleware
   4. **Next.js 12.x**: Rust 컴파일러, Edge 미들웨어, React 18 지원, SWC 컴파일러
   5. **Next.js 13.x**: App Directory, React Server Components, 서버 측 Suspense 개선

7. 결론

   넥스트.js는 버전마다 성능 최적화, 개발자 경험 개선, 서버 사이드 렌더링 및 정적 사이트 생성 등의 기능을 개선하고 확장해왔습니다. 각 버전에서 도입된 주요 기능들을 잘 활용하면 더욱 효율적이고 빠른 웹 애플리케이션을 개발할 수 있습니다. 최신 버전에서는 서버 측 렌더링과 동적 라우팅뿐만 아니라, React Server Components와 엣지 미들웨어 같은 고급 기능들이 추가되어 더욱 강력한 프레임워크가 되었습니다.
