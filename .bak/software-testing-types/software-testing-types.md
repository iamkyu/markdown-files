# software-testing-types

## Sanity Test
Sanity는 사전적 의미로 온전한 정신 또는 상태를 뜻한다. 위키백과에서 [소프트웨어 테스팅](https://en.wikipedia.org/wiki/Software_testing#Smoke_and_sanity_testing) 문서를 보면 Sanity 테스트에 대해 '추가 테스트를 진행하는 것이 타당한지 검증한다' 라고 간략하게 정리한다. 이 문장만 놓고 보자면 굉장히 작은 부분에 대한 테스트라고 짐작 된다.
관련 자료 중 가장 참고가 된 자료는 장진우님이 번역하신 [Smoke 테스트와 Sanity 테스트의 차이](http://ultrasparc.tistory.com/145)이다. 글에서 Sanity 테스트의 목표는 '제안된 기능이 대충 예상대로 동작하는지 확정하는 것이다.' 라고 한다.
그렇다면 단위 테스트 보다는 좀 더 고수준의 테스트이며 내가 기능을 추가한 부분만을 대상으로 하여 예상대로 동작하는지 확인하는 것이라고 볼 수 있을 것 같다. 
API만 개발하는 것이 아니라 E2E를 직접 개발할때면 수시로 브라우저와 같은 G.U.I. 환경에서 작성된 코드를 바탕으로 기능들이 작동하는지 확인하는데 이런 활동들이 Sanity 테스트의 범주에 속한다고 생각 된다.
