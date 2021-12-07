# 미션 - 자동차 경주 게임

🚀 기능 요구사항
초간단 자동차 경주 게임을 구현한다.

주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.
사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
전진하는 조건은 0에서 9 사이에서 무작위 값을 구한 후 무작위 값이 4 이상일 경우이다.
자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한 명 이상일 수 있다.
우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분한다.
사용자가 잘못된 값을 입력할 경우 IllegalArgumentException를 발생시키고, "[ERROR]"로 시작하는 에러 메시지를 출력 후 그 부분부터 입력을 다시 받는다.
아래의 프로그래밍 실행 결과예시와 동일하게 입력과 출력이 이루어져야 한다.
 
## 아이디어

n 대의 자동차를 가지고 경주하는 게임이다.

게임은 자동차를 가지고 있고 조건에 따라 차량을 전진시킨다.

자동차를 전진시키기위해 무작위로 티켓을 발행하고 유효한 티켓일 경우 전진시킨다.

게임은 사용자의 입력값에 따라 k번 자동차를 전진시키고 결과값을 출력한다.

모든 게임이 끝나면 최종 우승자를 출력한다.

## 프로젝트 구조

- domain
  
    게임을 진행하기 위해 필요한 단위 객체
- runner
	
    게임을 실행 시키기위한 객채
- utils
## 입력 예외 조건

이름 예외조건
- 이름의 길이는 최소 1글자 최대 5글자.
- 이름은 쉼표(,)로 구분한다.
- 이름은 비어있으면 안된다.
- 이름은 글자와 숫자만 허용한다.
- 중복된 이름은 허용하지 않는다.

실행 횟수 예외조건

숫자만 허용한다.

## 기능 목록

- 사용자 입력을 받는 기능.

- 예외입력을 처리하는 기능.

- 사용자 입력을 검증하는 기능.

  - 형식 검증
  - 글자 수 검증
  - 적절한 글자인지 검증
  - 중복된 이름이 있는지 검증

- n개의 자동차를 턴 마다 전진시키는 기능.

- 자동차를 전진시키기위해 조건을 만드는 기능.

- 자동차경주를 시키고 결과 메세지를 만드는 기능.

- 실행 결과 메세지 만드는 기능.

- 결과 메세지를 통합하고 출력하는 기능.
	