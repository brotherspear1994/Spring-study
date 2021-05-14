# ArgsConstructor 시리즈 



## @NoArgsConstructor, @RequiredArgsConstructor, @AllArgsConstructor

> 생성자 자동 생성 어노테이션

| 구분                     | 설명                                                         |
| :----------------------- | :----------------------------------------------------------- |
| @NoArgsConstructor       | 파라미터가 없는 기본 생성자를 생성 `Student std = new Student();` |
| @RequiredArgsConstructor | `final`이나 `@NonNull`인 필드 값만 파라미터로 받는 생성자 `Student std = new Student(1L);` |
| @AllArgsConstructor      | 모든 필드 값을 파라미터로 받는 생성자 생성 `Student std = new Student(1L, "홍길동", 20);` |

## 생성자란?

### 생성자(Constructor) 

### 역할

객체를 생성할 때 항상 실행되는 것으로, 객체를 초기화해주기 위해 맨 처음 실행되는 메소드이다.

### 특징

- **반환값이 없는 메소드는 생성자가 유일하다.**
  생성자는 인스턴스를 생성해주는 역할을 하는 특수한 메소드라고 할 수 있다. 반환값이 없기 때문에
  return도 사용하지 않고, 반환 값 타입을 메소드 정의 포함시키지도 않는다.

  

- **클래스에는 반드시 생성자가 존재해야 한다.
  **

- **인스턴스 생성시 딱 한번 호출 된다.
  **

- **인스턴스 변수의 초기화가 목적이다.**

- **클래 이름과 동일한 이름을 가진 메소드이다.**

- **반환형이 존재하지 않는다. 즉 return이 없다.**

### 사용방법

- **클래스명 참조변수=new 클래스명(초기화 변수)**