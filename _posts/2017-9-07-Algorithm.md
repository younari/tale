---
layout: post
title: "자료구조와 알고리즘"
author: "younari"
---

# Reading Note - 알고리즘

> [그림으로 개념을 이해하는 알고리즘](http://www.kyobobook.co.kr/product/detailViewKor.laf?mallGb=KOR&ejkGb=KOR&barcode=9788968483547&orderClick=JAj), 저자: 아디트야 바르가바, 한빛 미디어

### 참고 자료
- [The Euclidean Algorithm](https://www.khanacademy.org/computing/computer-science/cryptography/modarithmetic/a/the-euclidean-algorithm)
- [Journey into cryptography](https://www.khanacademy.org/computing/computer-science/cryptography)
- [Algorithms, Khan Academy](https://www.khanacademy.org/computing/computer-science/algorithms)


# ✔️ 자료 구조 
- 프로그래밍에서 데이터를 구조적으로 표현하는 방식과 이를 구현하는 데 필요한 알고리즘에 대해 논하는 기초이론
- 컴퓨터의 메모리는 1차원 구조이기 때문에 현실 세계의 다차원 데이터를 다루기 위해서는 이것을 1차원인 선 형태로 바꾸는 것이 필요하다. 2차원 배열, 이진 트리, 그래프 등의 자료구조가 2차원 데이터를 1차원으로 욱여넣는 방법을 배우는 것이다. 더 나아가 3차원 데이터를 다루고, 더 지나면 3차원 데이터 이상의 다차원 데이터를 처리하는 자료구조를 만날 수 있다. 물론 B트리나 R트리의 경우처럼 같은 2차원 데이터도 어떻게 조직화하느냐에 따라 자료구조가 달라진다.

### Linked List
- 데이터 덩어리(노드 Node)를 저장할 때 그 다음 순서의 자료가 있는 위치를 데이터에 포함시키는 방식으로 자료를 저장한다.
- 배열에 비해 데이터의 추가/삽입 및 삭제가 용이하나 순차적으로 탐색하지 않으면 특정 위치의 요소에 접근할 수 없어 일반적으로 탐색 속도가 떨어진다. 즉 탐색 또는 정렬을 자주 하면 배열을, 추가/삭제가 많으면 연결 리스트를 사용하는 것이 유리하다. 
- 배열은 자기가 안 쓰는 공간까지 전부 예약해두고 있어야 하기 때문에 공간 낭비가 생긴다.

### Stack
- 후입선출(後入先出, Last In First Out; LIFO)
- 입력은 push, 출력은 pop

### Queue
- 선입선출(先入先出, First In First Out; FIFO), 대기열
- 입력 동작은 Enqueue, 출력 동작은 Dequeue
- 어떠한 작업/데이터를 순서대로 실행/사용하기 위해 대기시킬 때 사용한다.


# ✔️ 이진 탐색

# ✔️ 배열과 연결리스트
- 컴퓨터의 메모리는 거대한 서랍장과 같다.
- 여러개의 항목을 저장하고 싶을 때는 배열이나 리스트를 사용할 수 있다.
- 배열을 쓰면 모든 항목은 이웃하는 위치에 저장된다.
- 리스트를 쓰면 모든 항목이 흩어지지만, 각 항목은 다음 항목의 주소를 저장하고 있다.
- 배열은 읽기가 빠르다.
- 연결리스트는 삽입과 삭제가 빠르다.
- 배열의 모든 원소는 같은 자료형이어야 한다.

# ✔️ Stack
- 푸시(삽입)와 팝(떼어내고 읽기) 두가지 일만 할 수 있는 것

# ✔️ Call stack
- 여러개의 함수를 호출하면서 함수에 사용되는 변수를 저장하는 스택을 호출스택이라고 한다.

# ✔️ 재귀 함수
- 재귀함수에서의 스택 사용
- 재귀는 함수가 스스로를 호출하는 것이다.
- 모든 재귀 함수는 기본 단계와 재귀 단계라는 두 부분으로 나뉘어져 있다.
- 스택에는 푸시와 팝이라는 두가지 연산이 있다.
- 모든 함수 호출은 호출 스택을 사용한다.
- 호출 스택은 너무 커져서 메모리를 엄청나게 소비할 수 있다.
- 재귀 대신 반복문을 써서 코드를 작성할 수 있다.
- 배열을 포함하는 재귀 함수를 만들 때, 기본 단계는 보통 빈 배열이나 원소가 하나뿐인 배열이 된다.