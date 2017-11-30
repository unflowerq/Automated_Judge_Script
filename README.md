# Automated_Judge_Script

자동 심사 스크립트(Automated Judge Script)

자동 심사를 진행하기 위해서 제출된 풀이를 심사하는 자동화된 심사 스크립트를 작성하라.
- 심사 방법은 다음과 같다
1. 제출된 프로그램에 의한 출력 결과가 정답과 완벽하게 일치하는가?
    일치 한다면 Accepted 로 심사한다
2. 제출된 프로그램에 의한 출력 결과중 정답에서 숫자와 숫자가 나온 순번만 일치 하는가?
    일치 한다면, Presentaion Error 로 심사한다
3. 1번과 2번이 아닐경우, Wrong Answer 로 심사한다

input
- 프로그램은 먼저 몇 라인의 정답을 받을 것인지 양의 정수 100 미만의 수 N을 입력 받는다.
N 라인 만큼 정답을 입력 받는다.
- 3번까지 되었다면, 5번으로 넘어 간다.
- 심사를 거칠 프로그램이 출력할 결과를 몇라인을 받을 건지 양의 정수 100 미만의 수 M을 입력 받는다.
- M 라인 만큼 결과를 입력 받는다.

output
- 6번까지 되었다면, 자동 심사 스크립트(Automated Judge Script)가 출력할 결과를 출력한다.
- 결과를 출력 할 때 printf("Run #%d: %s", 입력 세트, 심사 결과) 로 출력 한다.

주의 사항
- Presentaion Error 의 경우, 숫자의 위치가 고려 된다.
- 예를 들어 정답 "15 0" 과 프로그램의 결과 "150" 를 심사하면, Presentaion Error 로 간주 한다.
   하지만 "15 0" 과 "1 0" 은 Wrong Answer 로 간주한다.

input example
- 2
- The answer is: 10
- The answer is: 5
- 2
- The answer is: 10
- The answer is: 5
- 2
- The answer is: 10
- The answer is: 5
- 2
- The answer is: 10
- The answer is: 15
- 2
- The answer is: 10
- The answer is: '5
- 2
- The answer is: 10
- The answer is: 5
- 3
- Input Set #1: YES
- Input Set #2: NO
- Input Set #3: No
- 3
- Input Set #0: YES
- Input Set #1: NO
- Input Set #2: NO
- 1
- 1 0 1 0
- 1
- 1010
- 1
- The judges are mean!
- 1
- The judges are good!
- 0

output example
- Run #1: Accepted
- Run #2: Wrong Answer
- Run #3: Presentataion Error
- Run #4: Wrong Answer
- Run #5: Presentation Error
- Run #6: Presentation Error
