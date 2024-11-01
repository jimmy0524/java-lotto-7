## 구현할 기능 목록

- 입력
    - 로또 구입 금액
    - 당첨 번호 6개 입력 
    - 보너스 번호 입력
- 출력
    - 입력 받기 위한 프롬포트 출력
    - 발행한 로또 수량 및 번호 출력 (오름차순)
    - 당첨 내역 출력
    - 수익률 출력
    - 예외 상황 시 에러 문구 출력 ("[ERROR]"로 시작해야 함)
- 로또 기능
    - 구입 한 로또 객체 생성
    - 당첨 판별
    - 수익률 계산
- 예외 처리 (IllegalArgumentException)
    - 구입 금액 입력받는 상황
        - 아무것도 입력하지 않았을 경우
        - 1000 단위가 아닐 경우 
        - 양의 정수가 입력되지 않은 경우
    - 당첨 번호 입력받는 상황
        - 아무것도 입력하지 않았을 경우
        - 1-45 사이의 숫자가 아닐 경우
        - 6개의 숫자가 주어지지 않았을 경우
        - 양의 정수가 입력되지 않은 경우
        - 중복되는 숫자가 있을 경우
    - 보너스 번호 입력받는 상황
      - 1-45 사이의 숫자가 아닐 경우
      - 양의 정수가 입력되지 않은 경우
      - 아무 것도 입력되지 않은 경우 

## 개발 방식

- **TDD(테스트 주도 개발) 방식**을 사용하여 기능을 구현합니다. 기본적으로 다음의 세 단계로 진행합니다.

    1. **테스트 코드 작성**: 구현하고자 하는 기능에 대한 테스트 코드를 작성합니다. 이 단계에서 테스트는 실패하게 됩니다.

    2. **기능 구현**: 작성한 테스트를 통과할 수 있도록 최소한의 기능을 구현합니다.

    3. **리팩토링**: 구현한 코드를 정리하고 최적화합니다.


- 테스트 코드가 명확할 경우, 3단계로 나누지 않고 2단계로 진행하겠습니다.
- 입출력 기능은 요구사항에 따라 테스트를 따로 작성하지 않겠습니다.