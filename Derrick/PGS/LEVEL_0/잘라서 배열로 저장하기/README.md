# 프로그래머스 (PGS)

## Level 0

### [잘라서 배열로 저장하기]()
- 배운 내용, 문제 해결에 필요한 지식
	- 먼저 String으로 받는 매개변수를 Array String으로 변환 시켜야 한다.
		- map 고차함수를 사용
	- 해당 문제는 매개변수로 받는 n 값을 통해 String 값을 n만큼씩 잘라서 배열로 만드는 것이다.
	- n 만큼 짜르기 위해선 Array String의 총 개수를 먼저 구한다.
	- 총 개수 / n = 총 구해야 하는 배열의 수다.
		- for문 0...총 개수 / n 만큼이 우리가 구할 배열의 개수다.
	- 상위 for문 안에 또 다른 for문을 만든다
		- 해당 for문은 결과 값으로 나와야 하는 Array의 개수에 맞게 n의 배수로 첫 시작 0부터 n개까지의 값을 `결과 변수`에 넣는다. 
		- String 매개변수의 총 개수 - 1 값이 안의 for문 index보다 작으면 해당 for문은 break 한다.