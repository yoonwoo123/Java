

## Ch7. 자바 객체지향 2

### 1.1 상속의 정의와 장점

- 상속이란?

  - 기존의 클래스를 재사용해서 새로운 클래스를 작성하는 것.

  - 두 클래스를 조상과 자손으로 관계를 맺어주는 것.

  - 자손은 조상의 모든 멤버를 상속받는다.(생성자, 초기화블럭 제외)

  - 자손의 멤버개수는 조상보다 적을 수 없다.(같거나 많다.)

    ```java
    class 자손클래스 extends 조상클래스 {
        // ...
    }
    ```

    ```
    class Point { // 조상
        int x;
        int y;
    }
    
    class Point3D extends Point { // 자손
        int z;
    }
    ```


### 1.2 클래스간의 관계 - 상속관계

- 공통부분은 조상에서 관리하고 개별부분은 자손에서 관리한다.
- 조상의 변경은 자손에 영향을 미치지만, 자손의 변경은 조상에 아무런 영향을 미치지 않는다.

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\1.PNG)

- 포함이란 ?
  - 한 클래스의 멤머변수로 다른 클래스를 선언하는 것

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\2.PNG)



### 1.3 클래스간의 관계결정하기 - 상속 vs 포함

- 가능한 한 많은 관계를 맺어주어 재사용성을 높이고 관리하기 쉽게 한다.
- 'is-a'와 'has-a'를 가지고 문장을 만들어본다.

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\3.PNG)

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\4.PNG)


### 1.4 단일상속

- Java는 단일상속만을 허용한다.(C++은 다중상속 허용)

  ```java
  class TVCR extends TV, VCR { // 이와 같은 다중 상속 표현은 허용x 
      //...
  }
  ```

  ![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\5.PNG)



### 1.5 Object클래스 - 모든 클래스의 최고조상

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\6.PNG)

### 2.1 오버라이딩이란?

- 조상클래스로부터 상속받은 메서드의 내용을 상속받는 클래스에 맞게 변경하는 것을 오버라이딩이라고 한다.

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\7.PNG)



### 2.2 오버라이딩의 조건

1. 선언부가 같아야 한다. (이름, 매개변수, 리턴타입)

2. 접근제어자를 좁은 범위로 변경할 수 없다.
   - 조상의 메서드가 protected라면, 범위가 같거나 넓은 protected나 public으로만 변경할 수있다.
3. 조상클래스의 메서드보다 많은 수의 예외를 선언할 수 없다.

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\8.PNG)



### 2.3 오버로딩 vs 오버라이딩

- 오버로딩 - 기존에 없는 새로운 메서드를 정의하는 것 (new)
- 오버라이딩 - 상속받은 메서드의 내용을 변경하는 것 ( change, modify )

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\9.PNG)



### 2.4 super - 참조변수

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\10.PNG)



![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\11.PNG)



### 2.5 super() - 조상의 생성자

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\12.PNG)



![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\13.PNG)



### 3.1 패키지

- 서로 관련된 클래스와 인터페이스의 묶음.

- 클래스가 물리적으로 클래스파일인 것처럼, 패키지는 물리적으로 폴더이다. 패키지는 서브패키지를 가질 수 있으며 '.'으로 구분한다.

- 클래스의 실제이름은 패키지명이 포함된 것이다.

  String클래스의 full name은 java.lang.String)

- rt.jar는 Java API의 기본 클래스들을 압축한 파일

  (JDK설치경로\jre\lib에 위치)

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\14.PNG)



### 3.2 패키지의 선언

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\15.PNG)

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\16.PNG)

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\17.PNG)



### 3.4 import문

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\18.PNG)



### 3.5 import문의 선언

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\19.PNG)

![](C:\Users\IBK\Desktop\Java\200121_자바객체지향2\capture\20.PNG)

