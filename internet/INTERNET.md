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







