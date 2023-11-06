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