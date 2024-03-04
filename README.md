

## 1. Static Site Generator 란?

SSG로 생성되는 웹사이트는 모든 웹페이지를 미리 모두 만들어놓고
요청이 들어오면 만들어 놓은 웹페이지를 그대로 응답만 해준다.

### 특징

- 서버와 클라이언트 측 모두 렌더링을 위해 할 일이 별로 없기 때문에 SSG로 생성된 웹사이트는 속도가 엄청 빠르다
- CDN(Content Delivery Network)을 활용하면 미리 만들어 놓은 웹페이지를 유저와 지리적으로 최대한 가까운 곳에 캐싱(caching)해놓을 수도 있다.
<br/>
정적 사이트 생성기로 번역할 수 있는 SSG(Static Site Generator)는 누가 접속하든 항상 동일한 내용을 보여주는 웹사이트를 만드는데 최적화된 방법이다.

-> 컨텐츠의 변경이 자주 일어나지 않는 비교적 소규모 웹사이트를 제작에 주로 사용
-> 제품 카탈로그, 개인 블로그 등

 

### SPA vs. SSG

SSG로 생성된 웹사이트는 하나의 웹페이지에서 돌아가는 SPA와 달리,
미리 만들어 놓은 수 많은 웹페이지로 이루어졌기 때문에 검색 엔진이 크롤링하기 매우 적합한 구조를 가진다.

→ 따라서 SEO(검색 엔진 최적화)가 중요한 마켓팅 웹사이트를 제작할 때는 SSG가 매우 보편적으로 사용되고 있다.

대표적인 정적 사이트 생성 도구 :  Gatsby, Hugo, Jekyll, Hexo 등

### 단점

build 시점에 웹사이트 전체를 매번 다시 만들기 때문에 컨텐츠가 자주 업데이트 되는 웹사이트에서는 큰 비효율이 발생한다.
(보통 웹사이트의 규모가 커지면 자연스럽게 build 시간이 길어지고, 변경된 컨텐츠가 웹사이트에 반영되는데에 시간이 점점 오래 걸리게 되기 때문)

<br/>

## 2. Static Site Generator 선택 과정
`https://jamstack.org/generators/` 해당 사이트 에서  Static Site Generator들을 한눈에 볼 수 있다.
가장 많이 사용하는 편인 Jekyll , Hexo, Hugo를 비교한 내용이다.

```

Jekyll
  - 루비 기반
  - 현재 가장 인기 있음(깃헙 별 수 제일 많음)
  - 한글 레퍼런스도 제일 많음
  - 느리다는 제보가 많음(몇 십개의 포스팅 뿐인데도 빌드 하는데 5분씩 걸린다고)
  - 윈도우 공식 지원 안됨

Hexo
  - 자바스크립트(Node.js) 기반
  - 한글 레퍼런스 꽤 많음
  - 메인 개발자가 손을 놓은 듯
  - 개발자가 중국인? 이라 구글링하면 중국어 글이 많이 나옴

Hugo
  - Golang 기반
  - 빌드 빠름
  - 문서화 잘돼있음
  - 깃헙 별 수가 헥소보다 많음
  - 한글 레퍼런스가 거의 없음

출처: http://tadakichi.tistory.com/188
```

