## Ch2. 변수

### 2.2 상수와 리터럴

### 5. 변수, 상수, 리터럴

- 변수(variable): 하나의 값을 저장하기 위한 공간

  ```java
  int score = 100;
  	score = 200;
  ```

- 상수(constant): 한 번만 값을 저장 가능한 변수

  ```java
  final int MAX = 100; // MAX는 상수 상수는 앞에 final을 붙여줘야 한다.
  		  MAX = 200; // 에러
  ```

- 리터럴(literal): 그 자체로 값을 의미하는 것

  ```java
  100, 200, 'A', 'abc' 등을 의미한다
  변수 든 상수든 간에 그 값 자체를 의미하는 것
  ```

![](C:\Users\IBK\Desktop\Java\200108_자바변수\변수_상수_리터럴.PNG)

### 6. 리터럴의 접두사와 접미사

![](C:\Users\IBK\Desktop\Java\200108_자바변수\6.PNG)

### 7. 변수와 리터럴의 타입 불일치

![](C:\Users\IBK\Desktop\Java\200108_자바변수\7.PNG)

```java
// 숫자를 문자열로 바꾸고 싶을 때 숫자에 빈 문자열을 더해주면 된다.
"" + 7 => "" + "7" => "7"
"" + 7 + 7 = "77"
7 + 7 + "" => 14 + "" => "14"
```

![](C:\Users\IBK\Desktop\Java\200108_자바변수\8.PNG)

### 2.3 형식화된 출력 - printf()

![](C:\Users\IBK\Desktop\Java\200108_자바변수\9.PNG)

![](C:\Users\IBK\Desktop\Java\200108_자바변수\10.PNG)

### 이진수로 변환하는 것은 toBinaryString() 을 쓰며 자주 쓰진 않는다.

![](C:\Users\IBK\Desktop\Java\200108_자바변수\11.PNG)

![](C:\Users\IBK\Desktop\Java\200108_자바변수\12.PNG)

![](C:\Users\IBK\Desktop\Java\200108_자바변수\13.PNG)