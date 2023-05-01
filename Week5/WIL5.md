# HTML5 정리

## 1. 2 HTML5 Introduction & Syntax (HTML5 기본 문법)

1. HTML (HyperText Markup Language) : 웹페이지를 기술하기 위한 마크업 언어

   1. 웹페이지의 내용(content)와 구조(structure)를 담당하는 언어로써 HTML 태그를 통해서 정보를 구조화
   2. 반드시 <!DOCYPE html>로 시작해서 문서 형식을 지정
   3. 웹브라우저에 출력되는 모든 요소는 <body> </body> 사이에 위치

   ```html
   <!DOCTYPE html>
   <html>
     <head>
       <meta charset="utf-8" />
       <title>Hello World</title>
     </head>
     <body>
       <h1>Hello World</h1>
       <p>안녕하세요! HTML5</p>
     </body>
   </html>
   ```

1. HTML의 기본 문법

   1. 요소 (Element)

      → HTML 요소는 시작 태그(start tag)와 종료 태그(end tag) 그리고 태그 사이에 위치한 content로 구성

      <img src="https://file.notion.so/f/s/9480a121-db3a-4808-9ea8-a969bd4785c0/Untitled.png?id=41490a76-6ec6-4056-a47e-b2e04e901de1&table=block&spaceId=e8de49d9-29cd-4578-abb7-f03bed67e2c5&expirationTimestamp=1683028177391&signature=8JJScwJadcL-aNsoEEDro-7sS6V-d1xMcEXIXYi7FQI&downloadName=Untitled.png">

      → 요소는 중첩 가능 (다른 요소를 포함 가능) : 부자관계로 정보를 구조화하는 것

      → 빈 요소 (Self-Closing element) : attribute 만을 가질 수 有 (content가 X)

      ex) br, hr, img, input, link, meta 태그

1. 속성 (attribute)

   → 요소의 성질, 특징을 정의하는 명세

   → 시작 태그에 위치해야하며, 이름과 값의 쌍을 이룸

   ![img](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/23d7684c-aef5-4098-bfa6-b76b6e6349e2/Untitled.png)

---

## 1.3 Semantic Web (시맨틱 요소와 검색 엔진)

1. Semantic Tag & Non-semantic Tag

   1. Semantic Tag : 브라우저, 검색엔진, 개발자 모두에게 content의 의미를 명확히 설명하는 역할

      → ex) form, table, img, article(본문의 주내용이 들어가는 공간을 의미) , section (본문의 여러 내용을 포함하는 공간을 의미), header(헤더를 의미)

   2. Non-Semantic Tag : content에 대한 어떠한 설명도 하지 X

      → ex) div, span 등

      ![img](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c04b03bb-ddf9-4501-af47-e5d8c09e37aa/Untitled.png)

      원하는 위치에 따른 Semantic Tag 사용하기

   ***

   ## 1.4 HTML Tag - Basic (웹페이지를 구성하는 기본 태그)

   1. 문서 형식 정의를 하는 Tag

      → 출력한 웹 페이지의 형식을 브라우저에 전달

      → 문서의 최상위에 有

      ```html
      <!DOCTYPE html>
      ```

   2. html tag

      → 모든 HTML 요소의 부모 요소 & 웹페이지에 단 하나만 존재

      → 모든 요소들은 html 요소의 자식 요소이며, html 요소 내부에 기술되어야함

      → 단, <!Doctype html>은 예외

      ```html
      <!DOCTYPE HTML>
      <html>
        <head>
          <meta charset="utf-8">
      		<html lang="ko">
          <title>문서 제목</title>
        </head>
        <body>
          화면에 표시할 모든 콘텐츠는 이곳에 기술한다.
        </body>
      </html>
      ```

   3. head tag <head> </head>

      → 화면에 표시되지 않는 요소들 정의하는 부분

      → HTML 문서의 title,style, link, script에 대한 데이터로 화면에 표시되지 X

      1. title tag

         → 문서의 제목을 정의 / 정의된 제목은 브라우저의 탭에 표시됨

         ```html
         <title>문서 제목</title>
         ```

      2. style tag

         → css와 관련된 내용들을 새로운 파일에 작성하지 X고, html 문서 내부에 작성 시

         → <head> </head> 안에 작성됨

         ```html
         <style>
           body {
             background-color: yellow;
             color: blue;
           }
         </style>
         ```

      3. link tag

         → 외부 리소스와의 연계 정보를 정의 (주로 html과 외부 CSS 파일을 연계 시)

         → <head> </head> 안에 작성됨

         ```html
         <link rel="stylesheet" href="style.css" />
         ```

      4. script tag

         → 외부 client-side Javascript를 정의시

         ```html
         <script>
           document.addEventListener("click", function () {
             alert("Clicked!");
           });
         </script>
         ```

         ```html
         <script src="main.js"></script>
         ```

   4. body tag

      → HTML 문서의 내용을 나타냄

      → <body> </body>

   ***

## 1.5 HTML Tag - Text

1. 제목 (headings) 태그

   → 제목을 나타낼 때 사용하는 태그 (h1~h6 까지 존재)

2. 글자 형태 태그

   1. b : bold 체를 지정

      ```html
      <b>This text is bold.</b>
      ```

   2. i : 이텔릭체를 지정

      ```html
      <i>This text is italic.</i>
      ```

   3. small : 작은 글씨를 제공

      ```html
      <h2>HTML <small>Small</small> Formatting</h2>
      ```

   4. mark : highlighted text를 제공

      ```html
      <h2>HTML <mark>Marked</mark> Formatting</h2>
      ```

   5. del : 삭제되었다는 표시인 중간에 줄 그어진 text를 제공

      ```html
      <p>My favorite color is <del>blue</del> red.</p>
      ```

3. 본문 태그
   1. p : 단락 (paragraphs)를 지정
   2. br : 강제 개행을 지정
   3. pre : 작성한 그대로 브라우저에 표시됨
   4. hr : 수평한 줄을 삽입
   ***
