# CH4. 조건문과 반복문

## 4.3.2 while문

### WhileKeyControlExample.java

1, 2, 3 중 입력 받아서 if 문으로 분기실행

```java
package chap04;

public class WhileKeyControlExample {

	public static void main(String[] args) throws Exception {
		// TODO Auto-generated method stub
		boolean run = true;
		int speed = 0;
		int keyCode = 0;
		
		while(run) {
			if(keyCode != 13 && keyCode != 10) {
				System.out.println("-------------------");
				System.out.println("1. 증속 | 2. 감속 | 3. 중지");
				System.out.println("-------------------");
				System.out.println("선택: ");
			}
			
			keyCode = System.in.read();
			
			if (keyCode == 49) {
				speed++;
				System.out.println("현재 속도=" + speed);
			} else if (keyCode == 50) {
				speed--;
				System.out.println("현재 속도=" + speed);
			} else if (keyCode == 51) {
				run = false;
			}
		}
		
		System.out.println("프로그램 종료");
		
	}

}
```



### 확인문제

```java
// Ex03.java

package chap04;

public class Ex03 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int answer = 0;
		for (int i = 1; i <= 100; i++) {
			if (i % 3 == 0) {
				answer += i;
			}
		}
		
		System.out.println(answer);
	}

}
```



```java
// Ex04.java
package chap04;

public class Ex04 {
	public static void main(String[] args) {
		while (true) {
			int a = (int) (Math.random() * 6) + 1;
			int b = (int) (Math.random() * 6) + 1;
			
			System.out.printf("(%d, %d)\n", a, b);
			
			if (a + b == 5) break;
		}
	}
}
```



```java
// Ex05.java

```

