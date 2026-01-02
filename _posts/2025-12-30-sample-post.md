---
layout: post
title: 수식과 그래프 테스트
date: 2025-12-30 14:30:00
description: MathJax 수식과 Mermaid 그래프 렌더링 예제
tags: math diagram
categories: sample
mermaid:
  enabled: true
  zoomable: true
---

## 수식 예제

인라인 수식: 피타고라스 정리는 $$a^2 + b^2 = c^2$$로 표현됩니다.

블록 수식:

$$
\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}
$$

행렬:

$$
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
\begin{bmatrix}
x \\
y
\end{bmatrix}
=
\begin{bmatrix}
ax + by \\
cx + dy
\end{bmatrix}
$$

## Mermaid 그래프 예제

### 플로우차트
```mermaid
graph TD
    A[시작] --> B{조건 확인}
    B -->|참| C[작업 수행]
    B -->|거짓| D[종료]
    C --> E[결과 저장]
    E --> D
```

### 시퀀스 다이어그램
```mermaid
sequenceDiagram
    participant 사용자
    participant 시스템
    participant 데이터베이스
    
    사용자->>시스템: 로그인 요청
    시스템->>데이터베이스: 인증 정보 조회
    데이터베이스-->>시스템: 결과 반환
    시스템-->>사용자: 로그인 성공
```

### 클래스 다이어그램
```mermaid
classDiagram
    Animal <|-- Dog
    Animal <|-- Cat
    Animal: +String name
    Animal: +int age
    Animal: +makeSound()
    
    class Dog{
        +String breed
        +bark()
    }
    
    class Cat{
        +Boolean indoor
        +meow()
    }
```

## 복잡한 수식

오일러 공식:

$$
e^{i\pi} + 1 = 0
$$

미분방정식:

$$
\frac{dy}{dx} = ky \implies y = Ce^{kx}
$$

합 표기:

$$
\sum_{n=1}^{\infty} \frac{1}{n^2} = \frac{\pi^2}{6}
$$

## 마무리

이 포스트는 al-folio 테마의 수식과 그래프 렌더링 기능을 테스트하기 위한 예제입니다.
