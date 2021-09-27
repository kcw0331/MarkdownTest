# testrepository
연습용 리퍼지토리입니다.

## subtitle

  - 첫번째 : ㅌㅌ
  - 두번째 : ㄴㄴ
  - 

![a cat](http://icons.iconarchive.com/icons/google/noto-emoji-animals-nature/256/22221-cat-icon.png)

# Markdown 사용방법.

# 1. 마크다운에 관하여

1.1. 마크다운이란?
*Markdown*은 텍스트 기반의 마크업언어로 2004년 존그루버에 의해 만들어졌으며 쉽게 쓰고 읽을 수 있으며 HTML로 변환이 가능합니다. 특수기호와 문자를 이용해서 매우 간단한 구조의 문법을 사용하여 웹에서도 보다 빠르게 컨텐츠를 작성하고 보다 직관적으로 인식할 수 있습니다. 마크다운이 최근 각광받기 시작한 이유는 [github](http://github.com)덕분이다. 깃헙의 저장소 Repository에 관한 정보를 기록하는 README.md는 깃헙을 사용하는 사람이라면 누구나 가장 먼저 접하게 되는 마크다운 문서였습니다. 마크다운을 통해서 설치방법, 소스코드 설명, 이슈 등을 간단하게 기록하고 가독성을 높일 수 있다는 강점이 부각되면서 점점 여러 곳으로 퍼져가게 되었습니다.

1.2. 마크다운의 장점-단점.

1.2.2. 장점
> 1. 간결하다. 
> 2. 별도의 도구없이 작성가능하다.
> 3. 다양한 형태로 변환이 가능하다. 
> 4. 텍스트(Text)로 저장되기 때문에 용량이 적어 보관이 용이하다.
> 5. 텍스트파일이기 때문에 버전관리시스템을 이용하여 변경이결을 관리할 수 있다.
> 6. 지원하는 프로그램과 플랫폼이 다양하다.

1.2.2. 단점
> 1. 표준이 없다.
> 2. 표준이 없기 때문에 도구에 따라서 변환방식이나 생성물이 다르다.
> 3. 모든 HTML 마크업을 대신하지 못한다.

***

# 2. 마크다운 사용방법
------------------
2.1 헤더 Headers
---
***

* 큰 제목: 문서 제목
> This is a H1
> ============

***

* 작은 제목: 문서 부제목
> This is and H2
> --------------

* 글머리: 1~6까지만 지원
> # This is a H1
> ## This is a H2
> ### This is a H3
> #### This is a H4
> ##### This is a H5
> ###### This is a H6

2.2 BlockQuote
---------------

이메일에서 사용하는 > 블럭인용문자를 이용합니다.

> This is a first blockqute.
>   > This is a second blockqute.
>   >   > This is a third blockqute.

이 안에서는 다른 마크다운 요소를 포함할 수 있습니다.

> code

2.3 목록
--------

* 순서있는 목록(번호)
순서있는 목록은 숫자와 점을 사용한다.

> 1. 첫번째
> 2. 두번째 
> 3. 세번째 

현재까지는 어떤 번호를 입력해도 순서는 내림차순으로 정의됩니다.

> 1. 첫번째
> 2. 세번째 
> 3. 두번째 

* 순서없는 목록(글머리 기호: *, +, - 지원)

> * 빨강
>   *녹색
>     *파랑

> + 빨강
>   + 녹색 
>     + 파랑

> - 빨강
>   - 녹색
>     - 파랑

혼합해서 사용하는 것도 가능합니다. 

> * 1단계
>   - 2단계
>     +3단계
>       +4단계

2.4 코드
---------
4개의 공백 또는 하나의 탭으로 들여쓰기를 만나면 변환되기 시작하여 들여쓰기 않는 행을 만날때까지 변환이 계속됩니다.

*2.4.1. 들여쓰기*
> This is a normal paragraph:
 
>   This is a code block.
   
> end code block.

2.4.1. 코드블럭 
----------------
코드블럭은 다음과 같이 2가지 방식을 사용할 수 있습니다.
* <pre><code>{code}</code></pre> 이용방식
<pre>
<code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
     }
     
}
<\code>
<\pre>

public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}

* 코드블럭코드("```")을 이용하는 방법

```
public class BootSpringBootApplication {
  public static void main(String[]  args) {
    System.out.println("Hello, Heneymon");
  }
}
```

public class BootSpringBootApplication  {
  public static void  main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}

깃헙에서는 코드블럭코드("```")시작점에 사용하는 언어를 선언하여 문법강조(Syntaxhighlighting)이 가능합니다.

```java
public class BootStrapBootApplication {
  public static void  main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```

public class BootSpringBootApplication  {
  public static void main(String[] args)  {
    System.out.println("Hello, Honeymon");
  }
}  


2.5 수평선 <hr/>
================

아래 줄은 모두 수평선을 만든것입니다. 마크다운 문서를 미리보기로 출력할 때 페이지 나누기 용도로 많이 사용합니다.

* * *
***
*****
- - -
---------------------------
* 적용예

2.6 링크
========
* 참조링크
[link keyword][id]

[id]: URL "Oprional Title here"

// code
Link: [Google][googlelink]

[googlelink]: http://google.com "Go google"

* 외부링크
사용문법: [Title](link)
적용예: [Google](http://google.com, "google link")

* 자동연결
일반적인 URL 혹은 이메일주소인 경우 적절한 형식으로 링크를 형성합니다.

* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>

2.7. 강조
=========

*single asterisks*
_single asterisks_
**double asterisks**
__double asterisks__
~~cancelline~~

> 문장 중간에 사용할 경우에는 **띄어쓰기** 를 사용하는 것이 좋습니다.

2.8. 이미지
==========
![Alt text](/path/to/img.jpg)
![Alt text](/path/to/img.jpg "Optional title")

사이즈 조절 기능은 없기 때문에 <img width="" height=""></img>를 이용합니다.

예)
<img src="/path/to/img.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
<img src="/path/to/img.jpg" width="40%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>

2.9. 줄바꿈
------------
3칸 이상 띄어쓰기( )를 하면 줄이 바뀝니다.

* 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸 이상을 띄어쓰기를 해야합니다.   
* 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸 이상을 띄어쓰기를 해야 합니다.___\\ 띄어쓰기를 이렇게 해줍니다.




