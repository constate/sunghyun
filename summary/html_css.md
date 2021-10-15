# HTML

## HTML Introduction

https://www.w3schools.com/html/html_intro.asp

- HTML : Hyper Text Markup Language
- 웹 페이지의 내용을 표시하는 언어
  - 웹 페이지의 컨텐츠 표시
    - 텍스트 컨텐츠
    - 멀티미디어 컨텐츠 : 이미지(그림, 사진), 비디오, 오디오
  - 웹 페이지의 구조 표시

### HTML Element

https://www.w3schools.com/html/html_elements.asp

```
<tagname>Contents</tagname>
=> tagname : Contents 종류, 특성 표시 / 구조 표시

<tagname> : 시작 태그만 존재
=> Empty Element(빈 요소)
빈 요소는 시작태그로만 종료된다는 의미로 self-closing 기호를 사용할수 있음
<tagname />

- 기본 문법 : 사용하지 않음
- react.js 라이브러리에서는 반드시 사용
<tagname></tagname> => <tagname />

포함관계(Nested)
<tag1>
  <tag2>
    <tag3>Contents</tag3>
  </tag2>
</tag1>
<tag4></tag4>

tag1 ~ tag2의 관계
- tag1은 tag2의 Parent(부모요소)
- tag2는 tag1의 Children(자식요소)

tag1 ~ tag3의 관계
- tag1은 tag3의 Ancestor(조상요소)
- tag3은 tag1의 Descendants(자손요소)

tag1 ~ tag4의 관계
- Siblings(형제요소)

대소문자 구분하지 않음 => 소문자로 쓰는 것이 원칙
```

## HTML Attribute

https://www.w3schools.com/html/html_attributes.asp

- Attribute : 속성
- 추가정보를 제공

```
Ex)
<img src="이미지경로/파일이름">
<a href="이동경로주소">링크이름</a>

속성이름 = "정보"
```

## HTML Basic

https://www.w3schools.com/html/html_basic.asp

```
<!DOCTYPE html>
<html>
  <head>
    웹사이트(앱) 관련된 정보
  </head>
  <body>
    웹사이트의 콘텐츠
  </body>
</html>
```

- html 태그의 자식요소 : head, body
- head, body : 형제요소

## HTML TEXT Contents

### HTML Heading

https://www.w3schools.com/html/html_headings.asp

- h tag : heading
- h1 ~ h6

### HTML Paragraph

https://www.w3schools.com/html/html_paragraphs.asp

- p tag : paragraph - 단락표시
- hr tag : horizontal rules - 수평선 표시(단락 구분의미 포함) / 빈 요소

```
<p>단락</p>
<hr />
<p>단락</p>
```

- HTML paragraph display

  - 한 단락안에서 Enter 강제 줄바꿈, space 강제 공백은 적용이 안됨

  ```
  <br /> : Line Break / 강제 줄 바꿈, 빈 요소
  &nbsp; : non-break space - Entity code / 강제 공백 한칸
  (& : ampersand)

  ```

### HTML Links

https://www.w3schools.com/html/html_links.asp

- a tag : anchor
- attribute(속성) : href(hyper text reference) / 링크 연결 주소 정보

```
<a href="https://www.naver.com">네이버</a>
```

- 다른 페이지로 링크 연결
- 같은 페이지에서 상하 이동 -> 북마크 기능
  - href attr에 #만 사용하게 되면 페이지의 처음으로 이동

### HTML Lists

https://www.w3schools.com/html/html_lists.asp

- ul tag : unordered list / 순서 없는 목록
- ol tag : ordered list / 순서 있는 목록
- li tag : list item / 각 아이템 항목
- dl tag : description list / 설명 목록
- dt tag : description title(theme) / 설명 목록 제목
- dd tag : description data / 설명 내용

### HTML Table

https://www.w3schools.com/html/html_tables.asp

https://www.tablesgenerator.com/html_tables
(테이블 제네레이터)

표 구성 요소 : 열(세로줄), 행(가로줄), 셀(칸)

- table tag
- thead tag : 표 구성 영역 - 열제목 영역
- tbody tag : 표 구성 영역 - 데이터 영역
- tr tag : table row / 표의 행
- th tag : table header / 열 제목 셀
- td tag : table data / 데이터 셀

## HTML MULTIMEDIA Contents(Embed Contents)

### HTML Images

https://www.w3schools.com/html/html_images.asp

- img tag : image / 이미지 파일을 HTML 페이지에 삽입 / 빈 요소
- attribute
  - src : 이미지 파일의 경로/이름 정보
  - alt : alternative / 대체 텍스트

```
<img src="이미지 파일 경로/이름" alt="이미지 설명글">
(alt 자세한 설명이 필요 웹표준)
```

### HTML File Paths

https://www.w3schools.com/html/html_filepaths.asp

- 파일 경로 =(비슷) URL(Uniform Resource Locator)

```
URL
www.w3schools.com/html/html_filepaths.asp
www.w3schools.com/html/

File 경로
www.w3schools.com/html/html_filepaths.asp
```

- 인터넷 주소

  - IP : Internet Protocol / 인터넷에서 사용하는 실제 주소 ex)192.168.0.1
  - Domain Name : IP 주소를 대체하는 영어로 된 주소체계(www.naver.com)

- URL(Uniform Resource Locator)

```
URL
https://codesandbox.io/s/html-css-x1mfl?file=/summary/html_css.md

Domain Name
https://codesandbox.io/
```

- 인터넷에서 사용하는 서버에 저장된 자원의 위치
- 자세한 인터넷 주소

- 절대주소(URL)
  - File이나 Resource를 찾거나 이동하기 위한 기준 지점이 서버의 주소(IP, 도메인 주소)
  - 항상 같은 위치를 찾거나 이동할 수 있음

```
<a href="https://github.com/constate/sunghyun/blob/main/README.md"></a>

<img src="https://codesandbox.io/s/html-css-x1mfl?file=/summary/images/img.png" />
```

- 상대주소(URL)
  - File이나 Resource를 찾거나 이동하기 위한 기준 지점이 이동하거나 찾으려고 하는 파일의 위치
  - 상황에 따라 경로/주소 표시 형태가 변경될 수 있음

```
(현재문서 폴더 기준으로 이동)
<a href="README.md"></a>

<a href="../../README.md"></a>
(../ : 상위폴더)

<img src="summary/images/img.png" />

<img src="images/img.png" />
```

### HTML Video

https://www.w3schools.com/html/html5_video.asp

- video tag : 저장된 영상 파일을 해당 웹 페이지에 삽입

```
<video>
  <source src="영상 경로/이름" type="video/mp4" />
</video>
```

- attribute
  - html5에서 추가된 속성
  - name = "value" 형식에서 name만 쓰는 형식으로 변경
  - controls : 동영상 컨트롤 버튼 표시
  - loop : 반복 재생
  - autoplay : 자동 재생
  - muted : 음소거

## HTML Semantic Elements

https://www.w3schools.com/html/html5_semantic_elements.asp

- 영역을 구분하는 태그(요소)를 의미있게 구분하고 영역을 설정하도록 하는 태그

> header : 웹 페이지 상단 영역 - 로고, 로그인, 메뉴 등
>
> nav : navigation - 웹 사이트 메뉴
>
> section : 콘텐츠를 담는 영역
>
> article : 짧은 글 / 한 내용으로 완성되는 글
>
> aside : 부수적인 내용, 광고 등
>
> footer : 하단 영역 - 서브 로고, 주소, 연락처, 소유권 등

## HTML Block & inline

https://www.w3schools.com/html/html_blocks.asp

- HTML Element는 기본적으로 각각의 영역을 가짐

- HTML Elements의 특성(디자인 개념)

  - Block 요소

    - 항상 새 줄에서 표시됨(줄 바뀌어서 표시)
    - Block 요소로 만들어지는 영역의 가로길이가 전체 너비에 채워짐
    - div tag : division - container 요소

  - Inline 요소

    - 한 줄에 나란히 표시됨(줄 바뀌지 않음)
    - Inline 요소로 만들어지는 영역의 가로길이가 콘텐츠 길이만큼 너비를 차지함
    - span tag : container 요소

## HTML ID, Class

https://www.w3schools.com/html/html_id.asp
https://www.w3schools.com/html/html_classes.asp

- HTML Element에 이름을 지정해주는 attribute

> ID
>
> - 하나의 HTML 문서내에서 고유해야 함(하나만 존재) - 논리적 특징
> - 하나의 HTML Element에 여러개 ID 이름을 지정할 수 없음
> - 일반적으로 데이터를 고유하게 표시할 때 사용

```
<h1 id="heading">제목</h1>
<h1 id="heading">제목</h1> (x)

<p id="paragraph">단락</p>
<p id="sentence chapter">단락</p> (x)
```

> Class
>
> - 하나의 HTML 문서내에서 여러 Element에 사용할 수 있음
> - 하나의 HTML Element에 여러 Class 이름을 사용할 수 있음
> - 스타일을 공통 적용하거나 효과를 여러 곳에 동일하게 적용할 때 사용

```
<h1 class="heading">제목</h1>
<h1 class="heading">제목</h1> (o)

<p class="paragraph">단락</p>
<p class="sentence chapter">단락</p> (o)
```

# CSS

## CSS Introduction

https://www.w3schools.com/css/css_intro.asp

- css : Cascading Style Sheets
- HTML Element를 스타일링 해주는 언어

> cascading : 연속적인
>
> 동일한 HTML Element에 대해서 여러가지 스타일링 적용
>
> - 가장 마지막에 적용된 스타일이 HTML Element에 적용되어 화면에 표시

## CSS Syntax(문법, 구문)

https://www.w3schools.com/css/css_syntax.asp

- selector(선택자)
- declaration(선언)

```
선택자 {선언 - property(속성) : value(값);}
```

## CSS Selector(선택자)

https://www.w3schools.com/css/css_selectors.asp

- 스타일링할 대상(HTML Element)을 선택

> Simple Selector - name(tag), id, class 3가지를 사용해서 선택자를 표현
>
> Combinator Selector(복합 선택자)
>
> Pseudo-class(가상 클래스)
>
> Pseudo-element(가상 요소)

### Element(Tag) Selector

- 요소의 이름을 선택자로 사용
- 해당 요소를 모두 선택해서 스타일링 적용

```
p {}
div {}
```

### ID Selector

```
#heading {}
```

### Class Selector

```
.sentence {}
```

> 선택자 연결 표현
>
> - 여러 요소중 특정 요소를 선택하기 위해 사용

```
<p id="para" class="sentence">단락</p>

p#para {}
p.sentence {}
#para.sentence {}

```

## CSS 작성 방식

- External : 외부 파일
- Internal : html 파일 내부에 작성 - head 부분 style태그 사용
- Inline : html element에 직접 작성

## Color 이론

> 색 혼합 방식
>
> - 가산 혼합 : 빛 혼합
>
>   - 혼합하는 색이 많을 수록 밝아짐, 모든 색을 혼합 => 흰색
>   - 스크린 : 빛의 정보를 이용
>   - 컬러모드 : RGB (Red, Green, Blue)
>
> - 감산 혼합 : 잉크 혼합
>   - 혼합하는 색이 많을 수록 어두워짐, 모든 색을 혼합 => 검은색
>   - 프린트 : 잉크 색을 이용
>   - 컬러모드 : CMYK (Cyan, Magenta, Yellow, blacK(Key))

> RGB 모드
>
> 컴퓨터 사용 진법 : 2진법(0,1)
>
> 데이터 저장 최소 단위 : bit
>
> - 저장 공간 1칸 : 0,1중 하나를 저장
>
>   정보 표현 최소 단위 : byte(1byte = 8bit)
>
> RGB 컬러모드
>
> - Red, Green, Blue 각각 1byte 색 정보 표현
> - 총 3byte => 24bit 트루 컬러
>
> - CSS에서의 색 표현 방식
>   - 10진수 표시(0~9) : rgb(150, 200, 56) => 10진수 변형 : 0 ~ 255
>   - 16진수 표시(0~9, A~F) : #1AFFd3 => 16진수 변형 : 2진수 24bit -> 16진수 6자리

> 컴퓨터 용량 단위
>
> - 1000byte = 1KB
> - 1000KB = 1MB
> - 1000MB = 1GB
> - 1000GB = 1TB

> 투명모드
>
> - transparent, opacity, alpha
>
> CSS 표현
>
> - opacity : HTML Element 투명도 조절
> - rgba() : 색의 투명도 조절

## CSS 상속

- 조상 또는 부모요소에 적용된 css style이 자식 또는 자손요소에 상속되어 적용되는 현상
- 모든 CSS property의 style이 상속되는 것은 아님
- 모든 HTML Element가 상속되어 적용되는 것은 아님

```
-html
<div class="parent">
  <p class="child">단락</p>
</div>

-css
.parent{color:red;}

=> font 색상은 child 요소에도 적용
```

## CSS Property Category

- HTML Contents Styling

  - Text Contents Styling
  - Multimedia Contents Styling

- HTML 구조 Styling

## Text Contents Styling

### CSS Text

https://www.w3schools.com/css/css_text.asp

> color
>
> - 글꼴 색

> text-align
>
> - left, center, right, justify(양쪽맞춤)
