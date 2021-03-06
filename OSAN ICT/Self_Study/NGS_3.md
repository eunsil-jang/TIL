종류/연산자/설명
산술 연산자 + - * / % 사칙연산과 나머지 연산(%)
비교 연산자 > < >= <= == != 크고 작음과 같고 다름을 비교
논리 연산자 && || ! '그리고(AND)' 와 또는 '(OR)'으로 조건을 연결
대입 연산자 = 우변의 값을 좌변에 저장
기          타 (type) ?: instanceof 형변환 연산자, 삼항 연산자, instanceof연산자

* 피연산자 : 연산자의 연산 수행 대상
  * <b>4</b>*<b>5</b> bold처리된 숫자가 피연산자에 해당.

### 3-3 연산자의 우선순위
* 하나의 식(expression) 에 연산자가 둘 이상 있을 때, 
어떤 연산을 먼저 수행할지를 자동으로 결정하는것.

### 3-4 연산자의 결합규칙
* 우선순위가 같은 연산자가 있을 때 어떤것을 먼저 써야하는가?
→ 산술연산자는 왼-오 방향
→ 대입,단항 연산자는 오-왼 방향
결론 : 대입과 단항 연산자를 제외하면, 모두 왼쪽→오른쪽방향.

### 연산자 종합정리
1.산술>비교>논리>대입. 대입은 제일 마지막에 수행된다.
2. 단항(1)> 이항(2) > 삼항(3). 단항 연산자의 우선순위가 이항 연산자보다 높다.
3. 단항 연산자와 대입 연산자를 제외한 모든 연산의 진행 방향은 왼쪽에서 오른쪽이다.


### 3-5 증감 연산자
* 증가 연산자(++) 피연산자의 값을 1 증가시킨다.
* 감소 연산자(--) 피연산자의 값을 1 감소시킨다.
  * 증감 연산자가 독립적으로 사용된 경우, 전위형과 후위형의 차이가 없다.

타입   설명 예
전위형 값이 참조되기 <b>전에</b> 증가시킨다. j = ++i;
후위형 값이 참조된 <b>후에</b> 증가시킨다.   j= i++;


### 3-6 부호 연산자
'-' 는 피연산자의 부호를 반대로 변경
'+' 는 아무런 일도 하지 않는다.(실제 사용x)

## 와 3-7 이해안간다. 너모 어렵다.
### 3-7 형변환 연산자 
* 형변환 이란? 
  * 변수 또는 상수의 타입을 다른 타입으로 변환하는것.
	▶(타입) 피연산자
	ex) double d = 85.4;
	int score = (int)d;
	→ int score = (int)85.4;
	→ int score = 85;

### 3-8 자동 형변환
float f = 1234; // int 타입의 값을 float 타입의 변수에 저장
float f = (float)1234; // 컴파일러가 자동으로 형변환을 해줌 -> 자동형변환

int i = 3.14f; // 값손실이 발생할 수 있음. 컴파일러가 자동변환을 하지 못함.
int i = (int)3.14f; //  ok

<!-- 졸려서 더 못듣겠다 와우 3-8강 13:56 --> 
