# markdown 문법 필기

## heading

h1 -> `#` 

h2 -> `##`

h3 -> `###`

h4 -> `####`

h5 -> `#####`

h6 -> `######`



## list

### unorderd list

* / ~
* a
  * df
    * df
      * dfafd

<ul></ul>

### ordered list : 숫자 + .

1. 순서 리스트1
2. 순서 리스트2



## text style

### bold

** 로 표현 / ctrl + b

안녕하세요. **송채은**입니다.

### italic

*기울기 * / ctrl + i

안녕하세요. *송채은*입니다.



* bold + italic
  * 안녕하세요. ***서울 8반***입니다.



## hyperlink

### link

[텍스트](내가 가고 싶은 url)

[구글](https://www.google.com)

[네이버](https://www.naver.com)



### img

![대체텍스트](내가 보여주고 싶은 url)

![동글이](C:\Users\SSAFY\Desktop\GIT\TIL\assets\FOzslYSVcAIqzOX.jpeg)



## Code Block

### inline code block

백킷을 활용해서 인라인 코드를 만들 수 있어요.

`글1, 글2, 코드1`

### code block

백킷을 세 번 입력, 코드 실행 불가

```java
// C://user/SSAFY/
// TIL/intro1.java
class Simple{
    public static void main(String args[]){
        
        System.out.println("Hello Java");
        
    }
}
```



## Table

바를 이용

| 이름 | 학년 | 기수 | 전공 | 연락처 |
| ---- | ---- | ---- | ---- | :----- |
|      |      |      |      |        |



## git

`origin` 

​	: local ---물줄기 stream---> github

​	: 통로의 별명, branch

`master(main)`

​	: 통로의 이름, 여러개 생길 수도 있음, branch의 이름

## git으로 작업할 때 빈번하게

`git status` : git으로 관리되고 있는 폴더의 현황 조회, 커밋 전 단계까지만 확인 가능

`git add` . : git에게 tracking을 요청= staging area 에 올려주라주

 	1. git add [파일이름.확장자]
 	2. git add [파일이름1.확장자] [파일이름2.확장자]
 	 * 띄어쓰기가 포함된 파일이면 ' / '" 따옴표로 감싸준다.
 	3. git add . 
 	 * 전체를 다 올려줘

`git commit -m '[커밋 메세지]'` 

`git log` : 커밋 남긴 후에만 커밋 메세지 확인 가능

​					커밋 전에는 git status로 상태 조회, 커밋 후에는 git log로 조회

`git log --oneline` : 커밋 메세지 한 줄로 확인, push 이후에도 조회 가능

`git push origin master` : github에 파일 모두 올리기

`git pull origin maser` : github에 있는 파일 내려받기

​	폴더 생성> 폴더에 드러가서 git init> 폴더 안에서 git remote

`git clone [나의 github repo 주소]`

​	폴더를 만들지 않고도 바로 내려받을 수 있다

​	A가 A꺼를 clone 받았다. > add commit push

​	B가 A꺼를 clone 받았다. > pull request = B의 코드를 A의 레포에 반영하고 싶을 때



## git 계정 설정 시 최초 1회

`git config --global user.email '[내 github email]'`

​	: 내 로컬 컴퓨터 전역에 github email 설정

​	git config --global user.email

`git config --global user.name '[내 github user 이름]'` 

​	: 내 로컬 컴퓨터 전역에 github username 설정

​	git config --global user.name



## git으로 폴더를 앞으로 관리할 때 최초 1회

`git init`  : git 시작하기, 이 특정 폴더를 git으로 관리

`git remote add origin [github repo 주소]` : remote 등록, 레포 이름 등록

`git remote -v` : git에 올라갔는지 확인



## HTML

Hyper Text Markup Language ⭐

### HTML Syntax

1. element
   - content의 type을 지정
   - Element_name은 표준으로 정의
2. attribute
   - 생략 가능
   - element의 속성 지정
   - attribute_name과 value set을 표준으로 정의
3. comments
   - <!-- -->
4. Block level element
   - 새로운 행에 표시
   - 좌우 양쪽으로 최대한 느러나 가능한 모든 너비를 차지함
   - ex) <div>, <p>, <hl>, <form>
5. Inline level element
   - 새로운 행에 표시되지 않음
   - 필요한 너비만 차지함
   - ex) <span>, <a>,  <img>, <input>



### HTML Sections

1.  article
   - 문서의 독립적인 부분을 구성하는 섹션
   - 위젯 등 독립적인 아이템
   - ex) news, blog post, article
   - article 요소를 중첩할 경우 외부 article 요소와 연관된 내용
2. section
   - 일반적인 문서 또는 프로그램의 섹션
   - 제목으로 시작하는 컨텐츠의 의미적 그룹
3.  nav
   - 네비게이션 링크로 구성된 섹션
   - 다른 페이지 또는 동일 페이지의 다른 섹션 연결
4. aside
5. putter



### HTML Grouping

1. pre

   - preformatted text

   - block level element

   - 공백 문자와 줄 바꿈 문자를 보존

2. ol

   - ordered list

   - block level element

   - attributes

     start = number

     type = (1 | A | a)

   - ol 태그 안 순서는 li 태그 사용 > ul 태그도 동일하게 li 태그를 사용하여 번호를 매김

3. div

   - block level element
   - grouping block level elements
   - no visual changes
   - 같은 기능을 한 곳에 묶어 놓음 > 구별이 되어 있어 보기 편하지만 depth가 깊어짐



### HTML Text Level

1. a
   - anchor
   - hyper link에서만 사용, 나머지는 span태그 사용
2. span



### HTML Embedded < />

1. img
   - 크기 조절 가능
2. audio
3. video
4. source



### HTML Forms < />

1. form
2. input



## CSS

Cascading Style Sheets

HTML Element의 시각적 표현 정의



### CSS 사용 방법

1. External Style Sheet <link>

   - 가장 많이 사용
   - head 태그 속 meta 데이터에 css 파일이 속함

2. Internal Style Sheet <style>

   - 실습에서 가장 많이 사용

   - head 태그 속 style 태그를 넣는 방법

3. Inline Style

   - 태그 안에 속성을 넣음



### CSS Syntax

- Selector 선택자, declaration {property: value;} 로 구성
- 중괄호, 속성 뒤 세미콜론 잊지 않기!
- 주석 /* */



### CSS Selector

- ID Selector : #id, 1개만 만들 수 있음
- Class Selector: .class, 여러개 만들 수 있음
- Descendant Selector: 조상 선택자, 자식 선택자보다 범위가 넓음, 모든 요소 변경
- Child Selector: 자식 선택자, 바로 아래에 있는 요소 변경
  - 조상> 부모> 자식
- Link pesudo class
  - hover : 마우스를 올렸을 때의 변화
  - focus :  hover 적용 범위



## JAVA

* 추천 폰트: D2Coding / Fira Code

* eclipse 2018 / zulu8.33.0.1-jdk8.0.192-win_x64 설치



### 변수(Variable)

- 한 칸의 메모리, 변수를 담아두는 상자

  

#### 변수 선언

```java
자료형 변수명;	// 생성
변수명 = 값;	// 할당(assign)

자료형 변수명 = 값;
```



#### 변수 작명 규칙

* $ _
  * -(하이픈) 절대 사용 금지!
* 알파벳 문자나 숫자, 한글(비추)
  * 알파벳으로 시작
  * $ _ 로 시작 가능
* 중간에 공백 X
* dummy var 일 때 주로 언더바로 시작해서 설정
* 대소문자 구별
  * ascii 코드 때문
* java 내장 함수, 키워드 사용 금지
  * max, min, sum -> my_max 와 같이 사용



#### Data type

##### Primitive Data Type(기초형)

* (일반적인 값을 기억, 저장)하는 변수의 type
* **논리형 (boolean)**
  * 0, 1
  * false, true

* **문자형(char)**
  * 16비트 유니코드, 수치로는 0 ~ 65535
  * 비트 bit
    * 0, 1
    * 8 bit = 1 byte
    * n bit -> 2^n
*  정수형 == 숫자
  * byte : 사용 잘 x
  * short : 사용 잘 x
  * **int** : 정수, 음수, 양수
  * long

* 실수형 == 숫자(소수점)

  * **float** = 소수점
  * double 

  

#### Type Casting ⭐

##### Automatic promotions (Implicit Type Casting)

- 작은 크기 -> 큰 크기

- 사용자가 대입 했을 때, 자동으로 알아서 바꿔준다

- 정수형은 실수형으로 자동 변환 된다

  ```java
  long var = 100;
  float fvar = var;
  int kvar = 'A';
  ```

  

##### Explict Type Casting

* 큰 크기 -> 작은 크기

* 실수형을 정수형의 타입으로 변경한다

  ```java
  //identifier = (target_value) value;
  
  float fvar = 100;
  long var = (long) fvar;
  ```



### Operator (연산자)

1. 1순위 

- `[]` : 배열 요소 지정할 때

  - [1, 3, 5, 7, 9]

- `++` `--` 

  - 정수형 값을 증가, 감소

- `+` `-`

  - 정수, 실수

- `~` (비트)

  - 0 -> 1
  - 1 -> 0

- `!` (논리)

  - true -> false
  - false -> true

- `new`

  - 객체를 만들 때 사용

- `(type)`

  - 캐스팅 연산자
  - explicit casting

  

2.  2순위

* `*` : 곱셈
* `/` : 나누기(몫)
* `%` : 나머지



3. 3순위

* `+` `-`



4. 4순위

* `<<` `>>` `>>>`
  * 비트 연산 사용 시

5. 5순위

* `<` `>` : 값 대소 비교
* `<=` `>=` : 이상, 이하



6. 6순위

- `==` `!=` : 동일한지 비교(값),



7. 7순위

- `&` : AND 연산자, 비교 대상이 둘다 true -> true



8. 8순위

- `^` : 배타논리



9. 9순위

- `|` : OR 연산자, 하나가 false -> true



10. 10순위

- `&&` : 조건 AND



11. 11순위

- `||` : 조건 OR



12. 12순위

- `? :` : 조건 삼향



### Conditional(조건문)

`()` - 소괄호 `{}` - 중괄호 `[]` - 대괄호 `들여쓰기` - indent

#### if

* if(조건)

  * 조건 - boolean_expression

  * boolean_exprssion1 이 true일 때 statement1이 실행된다

    ```java
    if (boolean_expression1) {
        statement1
    } else if (boolean_expression2) {
        statement2
            if (boolean_expression2_1) {
                statement2_1
            } // else 그 외.. 모든 것
    } else {
        statement_3
    }
        
    ```

  - boolean expression
    - `if` `else if` O
    - `else` X
  - statement
    - `if` `else if` `else` O



#### switch

- expr 타입은
  - `int` `byte` `short` `char`

```java
switch (expr) {
    case 값1:
        statemen1t;
        break;
        
    case 값2:
        statemnet2;
        break;
        
    case 값3:
        statement3;
        break;
        
    default : 
        statement
}
```



### Loop (반복문)

#### for

```java
for (init_expr; boolean_testexpr; alter_expr) {
    statement or block;
}
```

```java
int[] nums = {1, 2, 3, 4, 5, 6};

for (int i=0; i < nums.length; i++) {
    System.out.println(nums[i]);
}
```

```java
for (type item: items) {
    statement or block;
}
```

```java
int nums = {1, 2, 3, 4, 5, 6};
int idx = 0;

// 멤버스 연산자
for (int n: nums){
    System.out.println(n);
    continue;	// 내 밑에는 처리하지 말고 다음 순서로 넘어가주세요
    break;		// 1만 출력되고 끝난다
    System.out.println(nums[idx]);
    idx++;
}
// 1
// 1
// 2
// 2
// 3
// 3
// 4
// 4
// 5
// 5
// 6
// 6
```

- index 접근이 필요하지 않을 때는 멤버스 연산자 사용



#### while

- while (범위x)

- boolean <- 거짓이 될 때까지!

- 무한반복

- runtime error 발생

  ```java
  while (boolean){
      statement or block;
  }
  ```



#### do ~ while

- 일단 고

```java
do {
    statemnet or blcok;
} while();
```















