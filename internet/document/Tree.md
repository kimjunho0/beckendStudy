# 트리란?

먼저 트리(Tree)란

![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FeeoNuG%2Fbtq1Eo7t7Xk%2F0bPk7BzhiruKSsgtiubvK0%2Fimg.png)

위와 같이 나무를 뒤집어 놓은 모양과 같은 비선형 계층적 자료구조이다.

트리는 트리 내에 다른 하위 트리가 있고, 또 그 트리 안에 또 다른 하위 트리가 있는

*[재귀적](#어떤-사건이-자신을-포함하고-다시-자기-자신을-사용하여-정의될-때-재귀적-이라-한다) 자료구조이다.

컴퓨터의 directory 구조가 트리 구조의 대표적인 예가 될 수 있다.

![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fbl6Ecy%2Fbtq1yFCmshK%2F4uvfvvAxqX3TYlEN2P2eX1%2Fimg.png)

트리 구조에 사용되는 기본 용어들

![image](https://gmlwjd9405.github.io/images/data-structure-tree/tree-terms.png)

위 사진을 예로 들어 설명함

#### 노드 (Node)

* 트리를 구성하고 있는 기본 요소
* 노드에는 키 또는 값과 하위 노드에 대한 포인터를 가지고 있음
* 위 사진의 A~J 까지 모두 노드임

#### 간선 (Edge)

* 노드와 노드 간의 연결선

#### 루트 노드 (Root Node)

* 트리 구조에서 부모가 없는 최상위 노드
* EX : A 노드

#### 부모 노드 (Parent Node)

* 자식 노드를 가진 노드
* H,I 의 부모 노드는 D

#### 자식 노드 (Child Node)

* 반대로 부모 노드를 가진 노드
* H,I 는 자식노드

#### 형제 노드 (Sibiling Node)

* 같은 부모를 가지는 노드
* H,I 는 형제 노드

#### 외부 노드 (External Node, Outer Node) or 단말 노드 (Terminal Node) or 리프 노드 (Leaf Node)

* 자식 노드가 없는 노드
* H,I,J,F,G

#### 내부 노드 (Internal Node, Inner Node) or 비 단말 노드 (Non-Terminal Node) or 가지 노드 (Branch Node)

* 자식 노드를 하나 이상 가진 노드
* A,B,C,D,E

#### 깊이 (Depth)

* 루트에서 어떤 노드까지의 간선 수

* 루트 노드의 깊이 : 0
* D의 깊이 : 2

#### 높이 (Height)

* 어떤 노드에서 리프 노드까지 가장 긴 경로의 간선 수

* 리프 노드의 높이 : 0
* A 노드의 높이 : 3

![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FMJU7c%2Fbtq1EoyuITO%2FNzwbe1WYQ4WlcY17cEENYk%2Fimg.png)

#### Level

* 루트에서 어떤 노드까지의 간선 수

#### Degree

* 노드의 자식 수
* 리프 노드의 Degree : 0; A 의 Degree : 2

#### Path

* 한 노드에서 다른 한 노드에 이르는 길 사이에 놓여있는 노드들의 순서
* A-H 경로 : A-B-D-H

##### Path Length

* 해당 경로에 있는 총 노드의 수
* A-H Path Length : 4

#### Size

* 자신을 포함한 자손의 노드 수
* 노드 B 의 Size : 6

#### Width

* 레벨에 있는 노드 수
* Level 2 Width : 4

#### Breadth

* 리프 노드의 수
* Breadth : 5

#### Distance

* 두 노드 사잉의 최단 경로에 있는 간선 수
* D 와 J 의 Distance : 3

#### Order

* 부모 노드가 가질 수 있는 최대 자식 수
* Order 3 : 부모 노드는 최대 3개의 자식 노드를 가질 수 있음

[Tree 구조 정리, 특징, 트리 종류](https://yoongrammer.tistory.com/68)



-----

###### 어떤 사건이 자신을 포함하고 다시 자기 자신을 사용하여 정의될 때 재귀적 이라 한다.<br>
