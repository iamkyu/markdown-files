# 테스트 주도 개발로 배우는 객체 지향 설계와 실천
> 스티브 프리먼 외, 이대엽 역, 인사이트 출판, 2013 [[링크](http://www.yes24.com/24/Goods/9008455?Acode=101)]

<!-- TOC -->

- [테스트 주도 개발로 배우는 객체 지향 설계와 실천](#테스트-주도-개발로-배우는-객체-지향-설계와-실천)
    - [1장 서론](#1장-서론)
        - [변화를 돕는 실천법](#변화를-돕는-실천법)
        - [테스트주도개발의 핵심 주기](#테스트주도개발의-핵심-주기)
        - [테스트 수준](#테스트-수준)

<!-- /TOC -->

## 1장 서론
### 변화를 돕는 실천법
시스템 규모를 믿을 수 있는 방식으로 키우고, 늘 일어나는 예상치 못한 변화에 대처하기 위한 기술적 토대

1. 회귀 오류를 잡아 줄 꾸준한 테스트
2. 코드 베이스를 가능한 단순하게 유지

이해와 수정이 쉬운 단순한 코드를 위해 설계를 개선하고 단순화하고, 중복 제거 등 꾸준히 리팩터링을 하기 위해서는 테스트 코드가 필요 함.

하지만 테스트 작성을 개발자들은 따분해 함. TDD는 작업을 완료한 후 작업 결과를 검증하려고 테스트를 작성하는 것이 아니라 **설계 활동으로 전환**시킴.



### 테스트주도개발의 핵심 주기
> 테스트 작성  > 테스트가 동작하게 만들 코드 작성 > 코드를 가급적 테스트한 기능의 단순한 구현으로 리팩터링

TDD를 통해 시스템 구현(“시스템이 동작하는가?”)과 설계(“시스템이 잘 구조화돼 있는가?”)의 품질에 관한 피드백을 얻음.


### 테스트 수준
- 인수 테스트: 전체 시스템이 동작하는가?
- 통합 테스트: 변경할 수 없는 코드를 대상으로 코드가 동작하는가?
- 단위 테스트: 객체가 제대로 동작하는가? 객체를 이용하기가 편리한가?

단위 테스트만 있는 프로젝트는 TDD 프로세스가 주는 아주 중요한 혜택을 놓치고 있는 셈.

![TDD 내에서의 안팎 피드백 고리](https://user-images.githubusercontent.com/13076271/36789676-b6d0e48a-1cd5-11e8-8e44-46572ead4dbf.png)

어떤 기능을 구현할 때 인수테스트를 작성하는 것으로 시작한다. 여기서 인수테스트란 만들고자 하는 기능을 시험하는 테스트를 말함. 인수테스트 하에서는 단위 테스트 수준의 테스트, 구현, 리팩터링 주기를 따라 기능을 개발. 전체 주기는 위 그림과 같음.

> 여기서 기능의 범주는? 단순히 메서드가 동작하는, 객체 수준에서 메세지를 주고 받는 것이 아니라 외부에서 유입되는 시스템(end-to-end)과의 상호작용