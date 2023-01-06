## int 와 Integer의 차이점

- ### int

  - Primitive type.
  - 산술 연산이 가능
  - null로 초기화가 불가함. (0으로 초기화 가능.)
  - cf) Primitive type(기본형) & Reference type(참조형)
    1. 기본형 : boolean, char, byte, short, int ,long float, double
    2. 참조형 : 배열(array[]), 열거(enum), 클래스(class), 인터페이스(interface)...

- ### Integer

  - Wrapper class; 기본형을 객체로 다루기 위해 사용하는 클래스
    - 매개변수로 객체를 필요로 할 때
    - 기본형 값이 아닌 객체로 저장할 때
    - 객체 간 비교가 필요할 때
  - null값 처리 가능
  - ex
    |primitive | - | Wrapper |
    | :---: | :----: | :------: |
    |double |- |Double|
    | float| -|Float |
    |long |- | Long|
    |int |- |Integer|
    | short|- | Short|
    |byte |- |Byte |
    | char|- | Character|
    | boolean|- |Boolean |

- ### int <-> Integer 간의 변환

  - Boxing : Primitive 자료형 -> Wrapper 클래스

    - ex
      // Integer (integer) 를 int (i) 로 변환
      int i = integer.intValue();

  - Unboxing : Wrapper 클래스 -> Primitive 자료형
    - ex
      // int (i) 를 Integer (integer) 로 변환
      Integer integer = new Integer(i);

- ### valueOf() 와 parseInt() 의 차이

  - Integer.valueOf(String) : Integer 클래스를 리턴하기 때문에 산술 연산이 불가능하다.
  - Integer.parseInt(String) : int 형을 리턴하기 때문에 산술 연산이 가능하다.

- ### Auto boxing & unboxing
  - java에선 대부분의 경우 자동으로 boxing과 unboxing을 해준다.
  - ex
    Integer integer = i; // int > Integer 로 Auto boxing
    int i2 = integer; // Integer > int 로 Auto unboxing

> > [참고블로그 : int와 Integer는 무엇이 다른가](https://velog.io/@hadoyaji/int%EC%99%80-Integer%EB%8A%94-%EB%AC%B4%EC%97%87%EC%9D%B4-%EB%8B%A4%EB%A5%B8%EA%B0%80) , [참고블로그 : 9. int 와 Integer 의 차이](https://lhwn.tistory.com/entry/9-int-%EC%99%80-Integer-%EC%9D%98-%EC%B0%A8%EC%9D%B4)
