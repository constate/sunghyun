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

## HTML MULTIMEDIA Contents

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

# CSS
