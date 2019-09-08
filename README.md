# Number Guesser

- 우리는 랜덤으로 숫자를 생성한 뒤 그 숫자가 컴퓨터가 만든 타겟 숫자와 얼마나 가까운지에 따라 컴퓨터와의 승패를 결정하는 게임을 만들것입니다. 
- 여기에서 대부분의 코드는 이미 작성이 된 상태이고 우리는guess.js 의 몇가지 코드만을 통해서js 함수를 공부할 것입니다.



## guess.js 만 사용

0. 3가지의 변수를 선언합니다. 사용자의 스코어, 컴퓨터의 스코어, 그리고 현재 라운드 넘버를 저장할 변수를 선언해야 합니다. 이 변수는 값이 달라질 수 있습니다.

 

1. generateTarget() 이라는 함수를 만들어야 합니다. 이 함수는 매번 새로운 라운드가 시작될때마다 불려야 하며 새로운 타겟 숫자를 생성해야 합니다. 이 함수는 리턴값으로0 ~ 9 까지의 정수값을 리턴해야 합니다.

* MDN 참고(Math.floor(), Math.random() 써야함.)

 

2. compareGuesses() 이라는 함수를 만들어야 합니다. 이 함수는 매 턴마다 내가 추측한 숫자가 타겟 숫자와 가까운지 컴퓨터가 추측한 숫자가 타겟 숫자와 가까운지를 판단합니다. 이 함수는3개의 인자를 받습니다. User guess, computer guess, 그리고target number. 그리고 유저와 컴퓨터중에서 누가taget guess에 가까운지를 판단하여 누가 이겼는지를 가려내야 합니다. 만약 유저가 이겼으면true를, 아니라면flase 를 리턴합니다.

* 절대값, MDN

 

3. updateScore() 함수를 만들어야 합니다. 이 함수는 승자의 스코어를 증가시켜야 합니다. 이 함수는 하나의 인자를 받는데 이 인자는String 으로서 승자를 나타냅니다. 앞서0 번에서 선언했던 변수(사람or 컴퓨터 점수) 중 하나를 인자로서 전달받은 승자에 기반하여1증가시킵니다. 아무값도 리턴하지 않아도 됩니다.

 

4. advanceRound() 함수를 만들어야 합니다 이 함수는 매 라운드가 끝날때마다 라운드 횟수를 증가시켜야 합니다. 0에서 선언했던 라운드 횟수를 세는 변수의 값을1증가시킵니다. 





# Arrow Function 연습

##1. agreeOrDisagree()라는arrow function 을 만듭니다. 

- 인자로는2개의String을 받아서 두개의String 이 같다면'똑같다' 라고 리턴하고 다르다면'다르다' 라고 리턴합니다.

##2. finalGrade()라는arrow function 을 만듭니다.

-  인자로는number type 3개를 받고 세 숫자의 평균을 구합니다. 

- 평균값에 따른 학점을 리턴합니다. 

- 만약0 - 100 사이의 숫자가 입력값으로 들어가지 않는다면 에러 메세지를 출력해야 합니다.

  70-79 should return: ‘C’

  80-89 should return: ‘B’

  90-100 should return: ‘A’

##3. tipCalculator()라는arrow function 을 만듭니다. 

- 인자로는String, number 를 받아서String의 값에 따라 팁을 리턴합니다. 

- 조건은

  ‘bad’ should return a 5% tip

  ‘ok’ should return a 15% tip

  ‘good’ should return a 20% tip

  ‘excellent’ should return a 30% tip

  all other inputs should default to 18%

  ```javascript
  tipCalculator('good', 100) // Should return 20
  ```

  



 