# internet

---
[1.how does the internet work?](#how-does-the-internet-work)

[2.what is http?](#what-is-http)

[3.browser and how they work?]()

***
## how does the internet work?

---

```인터넷의 작동원리```

인터넷이란 한마디로

컴퓨터들이 서로 통신이 가능한 거대한 네트워크이다.

또한 모든 컴퓨터를 하나의 통신망 안에 연결하고자 하는 의도를 지니고 있다.


![image](https://developer.mozilla.org/ko/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-1.png)


간단하게 두개의 컴퓨터가 연결이 되려면 위와 같이 물리적으로(케이블) 혹은 <br>
무선(WiFi, Bluetooth 등) 으로 연결이 되어야 한다.<br>

위와 같은 방식으로 연결을 할 수는 있다. 하지만 여러대 이상의 컴퓨터가 연결이 되면 너무도 복잡해진다.

![image](https://developer.mozilla.org/ko/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-2.png)

10대의 컴퓨터를 연결하려고만 해도 9개의 플러그가 달린 45개의 케이블이 필요하다

그러므로 이 문제를 해결하기 위해 우리는 라우터라는 특수한 소형 컴퓨터에 연결을 한다.

![image](https://developer.mozilla.org/ko/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-3.png)

이 라우터를 시스템에 추가하게 된다면 각 컴퓨터마다 1개의 단일 플러그와 10개의 플러그가 있는 하나의 라우터만이 필요하게 된다.
(아까에 비해서 매우 편리해짐)

하지만 이 라우터도 수백, 수천, 더 나아가서 수십억개의 컴퓨터와 연결은 힘들것이다.

물론 단일 라우터는 그 정도로 확장이 힘들지만

아까 말했던 것 처럼 라우터도 컴퓨터다.

그렇다면? 라우터끼리 연결도 가능한것 아닌가?

![image](https://developer.mozilla.org/ko/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-4.png)

컴퓨터에서 라우터로, 라우터에서 라우터로

우리는 무한히 확장 할 수 있게 되었다.

![image](https://developer.mozilla.org/ko/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-5.png)

하지만 이걸로는 인터넷이라 할 수 없다.

우리가 처음에 말했던 모든 컴퓨터가 속해야 인터넷이라 했는데

결국 라우터를 사용하는것은 물리적인 연결이기 때문에

너무 멀리있는 컴퓨터와의 연결이 불가능 하다는 문제가 생긴다.

하지만 이 문제도 정말 간단히 해결될 수 있었다.

전력 및 전화와 같이 집에 연결된 케이블이 있기 때문에

우리가 원하던 네트워크는 이미 구현이 되어있던 것이었다.

따라서 우리가 원하는 전화 네트워크와 우리의 네트워크를 연결하기 위해서는

모뎀이라는 장치가 필요하다.

![image](https://developer.mozilla.org/ko/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-6.png)

이 모뎀을 통해 우리 네트워크의 정보를 전화 시설에서 처리할 수 있는 정보로 바꾸며 그 반대의 경우도 마찬가지이다.

이제는 우리의 네트워크는 전화시설에 연결이 되어 어디로든 데이터를 보낼 수 있고 어디서든 데이터를 받을 수 있다.

하지만 그걸 위해 ISP 라는 인터넷 서비스 제공업체에 연결을 해야한다.

ISP는 모두 함께 연결 되는 라우터를 관리하며, 다른 ISP 의 라우터에도 접근할 수 있는 회사이다.

(예를 들어 우리나라의 LG U+, KT, SKT 등)

이렇게 우리 네트워크의 메시지는 ISP 의 네트워크 속의 네트워크를 통해 다른 네트워크로 전달이 된다.

인터넷은 이러한 인프라로 구성이 된다.

![image](https://developer.mozilla.org/ko/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-7.png)

참고<br>
[mozilla developer](https://developer.mozilla.org/ko/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work)


---

# what is http

```http 란```

HTTP(HyperText Transfer Protocol)

- 텍스트 기반의 통신 규약

- 이 통신 규약을 통해 모든 프로그램이 이 규약에 맞춰 개발을 하여 정보를 주고 받을 수 있다.

먼저 http 를 설명하기 전 www 에 대해 알고 가자.

www(world wide web)

- www 란 웹 페이지를 네트워크 상에서 이용하기 위한 구조를 말한다.

- www 에서는 http 라는 통신 방식에 기초하여 주고 받기가 실행된다.

- www 의 발명으로 http 프로토콜이 개발되었고 또 발전되었다.

web은 www의 약자로 인터넷에 연결된 사용자들이 서로의 정보를 공유할 수 있는 공간을 의미한다.

하지만 인터넷과 동의어는 아니며, 웹 브라우저를 통해 서버와 클라이언트가 통신하는 방식의 인터넷 서비스중 하나이다.


### HTTP의 구조

1. [클라이언트와 서버](#클라이언트와-서버)
2. [무상태 프로토콜 (stateless)](#무상태-프로토콜)
3. [비 연결성(connectionless)](#비-연결성)

#### 클라이언트와 서버

클라이언트가 서버에 요청을 보내면 서버는 그에 응답을 보내는 클라이언트 - 서버 구조로 되어있다.

![image](https://velog.velcdn.com/post-images%2Fsurim014%2Fe0aa5520-2d59-11ea-86da-fb3b00230640%2Fimage.png)



#### 무상태 프로토콜

서버가 클라이언트의 상태를 보존하지 않는 무상태 프로토콜이다.

- 장점 : 
<br><br>
    서버 확장성이 높다.
<br><br>
- 단점

    클라이언트가 추가 데이터를 전송해야 한다.

```
무상태의 한계

로그인과 같이 유저의 상태를 유지해야하는 서비스라면 브라우저 쿠키, 서버 세션, 토큰 등을 이용해야 한다.
```

#### 비 연결성

### ```연결 지향```

- TCP/IP 의 경우 기본적으로 연결을 유지한다.
- 연결을 유지하는 경우 클라이언트가 요청을 보내지 않아도 서버는 계속 연결을 유지해야 한다.
- 이러한 경우 연결을 계속 유지하는데에 서버의 자원이 소모된다.

### ```비 연결성```

- 비 연결성을 가지는 HTTP 에서는 실제로 요청을 주고 받을때를 제외하고 응답을 주고나면 TCP/IP 연결을 끊는다.
- 이를 통해 최소한의 자원으로 서버 유지를 가능하게 한다.

하지만 위와 같은 방식의 비 연결성은 
- TCP/IP 연결을 새로 맺어야 하므로 3 way handshake 시간이 추가된다.
    
    [TCP 의 연결방식](https://mindnet.tistory.com/entry/네트워크-쉽게-이해하기-22편-TCP-3-WayHandshake-4-WayHandshake)
- 웹 브라우저로 사이트를 요청하면 HTML, CSS, JavaScript, 추가 이미지 등 수많은 자원이 함께 다운로드 되는데,<br>
이러한 자원들을 각각 보낼 때마다 연결을 끊고 다시 연결하고를 반복하는 것은 매우 비효율적이다.

이러한 문제들은 HTTP/2, HTTP/3 와 같은 높은 버전에서 해결을 하였다.

#### ```비 연결성 극복```
- HTTP 초기 - 각각의 자원을 다운로드하기 위해 연결과 종료를 반복해야 했다.


- HTTP 지속연결 - 지속연결을 하고 난 후 연결이 이루어지고 난 뒤 각각의 자원들을 요청하고<br> 모든 자원에 대한 응답이 돌아온 후에 연결을 종료한다.

---

# browser and how they work?

```브라우저 그리고 브라우저의 작동 방식```

먼저 브라우저가 무엇인지에 대해 알아보자.

브라우저란?

웹에서 정보를 탐색하고 HTML 문서, 이미지 등 여러 콘텐츠를 우리에게 표현해주는 소프트웨어이다.

우리에게 익숙한 구글의 크롬, 애플의 사파리, 마이크로소프트 엣지, 모질라의 파이어폭스 등이 있다.

### 브라우저의 기본 구성요소

1. 사용자 인터페이스 : 주소 표시줄, 이전/다음 버튼, 북마크 등 페이지 뷰 이외의 다른 부분
2. 브라우저 엔진 : 사용자 인터페이스와 렌더링 엔진 사이 동작을 제어
3. 렌더링 엔진 : HTML, CSS를 파싱해 화면에 요청한 컨텐츠를 표시
4. 통신 : HTTP 요청과 같은 네트워크 호출에 사용됨
5. UI 백엔드 : 기본적인 위젯(콤보 박스 등)을 그림
6. 자바스크립트 인터프리터 : 자바스크립트 코드를 해석하고 실행
7. 테이터 스토리지 : 자료를 저장하는 계층으로 쿠키 등을 저장하는 웹 데이터 베이스

![image](https://web.dev/static/articles/howbrowserswork/image/browser-components-9cd8ff834cc9c_1920.png)

### 렌더링 엔진

렌더링 엔진은 위에서 설명한것과 같이 요청받은 내용을 브라우저 화면에 표시해주는 역할을 한다.

브라우저마다 사용하는 렌더링 엔진이 다르기에 같은 페이지가 다르게 보이는 경우가 있다.

렌더링 엔진의 종류는 다음과 같다.

| 브라우저  | 렌더링 엔진  |
|-------|---------|
|IE|Trident|
|Edge|EdgeHTML, Blink|
|Chrome|Webkit, Blink(버전 28 이후)|
|Safari|Webkit|
|FireFox|Gecko|

각각의 렌더링 엔진들은 웹 표준에 따라서 개발자들이 작성한 문서를 브라우저에 보여주지만,

개발 진척도나 별도 규칙에 따라 지원하는 표준이 다르거나 렌더링 알고리즘과 방식에 차이가 있을 수 있다.

### 렌더링 엔진 동작 과정

![image](https://velog.velcdn.com/images%2Fthyoondev%2Fpost%2Fcef4b5a9-41d7-4681-9a83-5e85784fc83c%2F1608995710399render-min.png)

위 과정이 렌더링 엔진의 기본 동작 과정이다.

1. 렌더링 엔진은 HTML 문서를 파싱하여 DOM 트리를 구축한다.<br><br>
2. 그 다음 외부 CSS 파일과 함께 포함된 스타일 요소를 파싱한다.<br><br>
3. DOM 트리와 2번의 결과물을 합쳐 렌더 트리를 구축한다.<br><br>
4. 렌더 트리 각 노드에 대해 화면 상에서 배치할 곳을 결정한다.<br><br>
5. UI 백엔드에서 렌더 트리의 각 노드를 그린다.

이 과정을 하나씩 살펴보자.

아래 그림은 렌더링 엔진 중 하나인 웹킷 엔진에 나타낸 그림이다.

![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Flaupf%2Fbtrb2k8Jd5L%2FuqmWtkHRlnZg3DwXyyMND1%2Fimg.png)

동작 과정의 순서는 위에서 설명한 기본 동작 과정과 유사하다.

### 1.HTML 문서를 파싱하여 *[DOM](document/DOM.md#dom-이란)(Docoument Object Model) *[트리](document/Tree.md#트리란)를 구축한다.

DOM 은 마크업과 1:1 관계를 성립한다

![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fdye6Tm%2Fbtrb7yZhbxh%2FNEXpIkMMV0Aqk3e5OSXU41%2Fimg.png)

브라우저는 서버로부터 HTML 문서를 모두 전달받고 HTML 파서를 통하여 파싱 하고 파싱 트리를 생성한다.

생성된 파싱 트리를 기반으로 DOM 트리를 생성한다.

### 2.CSSOM(Css Object Model) 을 생성한다.

![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbKJnUb%2Fbtrb8f6gRKU%2FDn4wpPKW6FVseOKdgGdZQK%2Fimg.png)

CSS 파일은 스타일 시트 객체로 파싱 되고 각 객체는 CSS 규칙을 포함한다. CSS 규칙 객체(CSSOM)은 선택자와

선언 객체, 그리고 SCC 문법과 일치하는 다른 객체를 포함한다.

### 3.렌더 트리(DOM + CSSOM)를 생성합니다.

DOM 트리가 구축되는 동안 브라우저는 DOM 트리를 기반으로 렌더 트리를 생성합니다.

렌더 트리는 문서를 시각적인 구성 요소로 만들어주는 역할을 합니다.

웹킷은 이 구성 요소를 "렌더러(rendere)" 또는 "렌더 객체(render object)"라는 용어를 사용합니다.<br>
렌더러는 자신과 자식 요소를 어떻게 배치하고 그려내야 하는지 알고 있습니다.

렌더러는 DOM 요소에 부합하지만 1:1로 대응하는 관계는 아니다. 그 이유는 <head>, display:'none'과 같은<br>
사용자가 볼 수 없는 DOM 요소는 렌더 트리에 추가되지 않습니다. (visibility 속성에 "hidden" 값이 할당된 요소는 트리에 나타납니다.)

