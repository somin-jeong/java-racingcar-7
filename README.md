# java-racingcar-precourse
## 기능 요구사항
- 초간단 자동차 경주 게임을 구현한다.

- 주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
- 각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
- 자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.
- 사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
- 전진하는 조건은 0에서 9 사이에서 무작위 값을 구한 후 무작위 값이 4 이상일 경우이다.
- 자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한 명 이상일 수 있다.
- 우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분한다.
- 사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시킨 후 애플리케이션은 종료되어야 한다.

## 기능 목록
- [x] 경주할 자동차 이름을 입력받는 기능
- [ ] 이동을 시도할 횟수를 입력받는 기능
- [ ] 각 자동차에 대해 전진하는 조건을 만족할 경우 자동차가 전진하는 기능 -> 이동을 시도할 횟수만큼 반복
- [ ] 매 라운드 자동차가 얼마나 전진했는지 기록하는 기능
- [ ] 가장 많이 전진한 사람을 찾는 기능
- [ ] 우승자를 출력하는 기능

## 예외처리
### 이름 입력
1. 입력 값이 공백 혹은 비어있는 문자열인 경우 예외
2. 쉼표로 구분된 자동차 이름의 길이가 1~5자가 아닌 경우 예외
3. 자동차 이름에 중복이 있는 경우 예외

### 시도 횟수 입력
1. 입력 값이 공백 혹은 비어있는 문자열인 경우 예외
2. 입력 값이 숫자가 아닌 경우 예외
3. 입력 값이 음수인 경우 예외