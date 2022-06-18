# 백준(baekjoon) 2557번 문제 Hello World 문제풀이(python, c, c++, c#, java)

---

문제: Hello World!를 출력하시오

.

입력: 없음

출력: Hello World!를 출력하시오.

---

## **python**

```
print("Hello World!")
```

파이썬은 간단하게 print만 사용하면 원하는 문장을 출력할 수 있다.  
컴파일 없이도 바로 실행하고 확인할 수 있어서 편리하다.

---

## **c**

```
  #include <stdio.h>

  main()
  {
      printf("Hello World!");
  }
```

-   헤더파일(위에서는 stdio.h)은, main()보다 먼저 작성한다.
-   보통 헤더 파일은 #include<기본 라이브러리 헤더>의 기본형식을 가지고 있다.
-   stdio – 표준 입출력(standard input output)의 약자로 입력과 출력에 관련된 라이브러리 함수들이 포함되어 있다.
-   헤더파일에는 라이브러리 함수(위에서는 printf())들이 포함되어 있다.
-   모든 C 프로그램에는 main이라는 이름을 지정해야 하는 기본(main) 함수가 있다.
-   main()함수에는 프로그램의 시작부터 종료까지 실행되는 내용들이 작성되어 있다.
-   문장의 마지막엔 세미콜론(;)을 사용해야 한다.
-   실행되는 문장이 2줄 이상일 경우 중괄호{ }를 사용하여 묶어주는데, 이를 코드블록(code block)이라고 한다.

[참고](https://opentutorials.org/module/3921/23496), [참고2](https://opentutorials.org/module/3921/23498)

---

## **c++**

```
#include <iostream>

main() 
{
   std::cout << "Hello World!" << std::endl;
   return 0;
}
```

-   '#'은 전처리기이다. 전처리기는 컴파일을 시작하면, 우선적으로 처리된다.
-   iostream은 cout, cin, cndl등 기본 입출력과 관련된 객체들을 정의한 헤더파일이다.
-   iostream은 표준 라이브러리 디렉토리에 존재한다.
-   표준라이브러리에 있는 변수나 함수는 std 표준 네임스페이스에 포함되어 있다.
-   그래서 표준라이브러리를 사용할 때 std::접두어를 붙여야 한다
-   cout: 화면에 데이터를 출력한다. '<<' 기호를 사용한다
-   endl: 한 줄 띄운다.
-   cin: 데이터를 입력받는다.
-   return이 없으면 오류가 발생한다.

[참고](https://hongku.tistory.com/72), [참고2](https://y-min.tistory.com/8)

```
#include<stdio.h>

main()
{
    printf("Hello World!");

}
```

-   물론 c에서 사용한 방법 그대로 사용할 수 있다.

---

## **c#**

```
Console.WriteLine("Hello World!");
```

-   콘솔(console)클래스는 사용자 인터페이스를 구현할 수 있는 속성과 함수를 제공한다.
-   WriteLine은 현재 줄 종결자를 표준 출력 스트림에 쓰는 역할의 method이다.

[참고](https://docs.microsoft.com/ko-kr/dotnet/api/system.console?view=net-6.0), [참고2](https://developer-talk.tistory.com/320)

```
using System;

namespace Baekjoon2557
{
    class Solution
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
        }
    }
}
```

---

## **java**

```
// 클래스 블록
class main {
    // 메소드 블록
    public static void main(String[] args) {
        // 명령문(statement)
        System.out.println("Hello World!");
    }
}
```

-   자바 역시 컴파일러 언어이기 때문에, 컴파일 하는 과정이 필요하다.
-   class 이름이 파일 명과 같아야 하는데, 위의 코드는 백준에서 제출하기 위해 class 이름을 main으로 하였고, 로컬에서는 관리를 위해0 파일명을 baekjoon\_2557\_java.java로 하였기 때문에 아래 코드와 같이 작성하였다.
-   이를 지키지 않으면, 컴파일에러가 발생한다.
-   일반적으로 자바의 소스코드는 클래스 블록과 메소드 블록으로 구성된다.
-   public class main으로 작성할 수도 있는데, public은 자바의 접근제어자로 어디서든 이 클래스에 접근할 수 있음을 의미한다.
-   위의 메소드명은 main이며,
-   static - 메소드에 static 키워드가 붙을 경우 이 메소드는 클래스 메소드가 되어 객체를 만들지 않아도 "클래스명.메소드명" 형태로 호출이 가능하다.
-   void - 메소드의 리턴타입 중 하나로 void는 리턴값이 없음을 의미한다.
-   String\[\] args - 메소드의 매개 변수이다. args 변수는 String\[\] 배열 자료형임을 의미한다. args라는 이름은 인수를 의미하는 arguments의 약어로 관례적인 이름이다. args 대신 다른 이름을 사용해도 상관없다.
-   컴퓨터에 무언가 일을 시키는 문장을 명령문(Statement)이라고 한다. 명령문은 반드시 세미콜론(;)을 붙여 문장의 끝을 표시해야 한다. 메소드 블록 안에는 여러개의 명령문이 있을 수 있다.

[참고](https://wikidocs.net/278)

---

python 이외의 언어는 거의 다뤄보지 않았기 때문에, 간단하지 않았다.  
  
5개의 언어에서 어떤 방식으로 문제를 풀 수 있는지 이해해보고자 한다.