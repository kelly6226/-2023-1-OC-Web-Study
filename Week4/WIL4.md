# 2023-1-OC-Web-Study

# 4주차 Html과 Web

### 1. HTML : Hyper Text Markup Language

1. Html의 기본 골격

   1. Tag : 이름표를 문서에 달아주는 것

      ex) <html> <head> <title> <h1>

      → Tag를 열어주면 닫아야함 BUT 가끔 하나짜리도 있음

      ex. <input placeholder=”안녕”/>

      ex. <br/> 줄바꿈을 나타내는 tag

   2. attribute : Tag가 가지는 속성

      ex. <h1 style=”color: red”> 여러분 <h1/>

   c. 기본 구조는 4가지

   (1) <!Doctype html>

   → document인데 이것의 type이 HTML이라는 것을 브라우저에게 알려주는 것

   (2) head

   → head에 적은 것들은 <title> 빼고 눈에 보여지지 X

   → 컴퓨터에 주는 정보들이 적혀있는 곳이 head (문서는 이런 속성을 가지고 있어!)

   ex. <meta>

   (3) body

   → 실제로 웹사이트에 보이는 것들

   (4) html

   → <head>와 <body>를 감싸고 있음

   → html 문서라는 것을 <html> </html>로 감싸면서 나타냄

### 2. 다양한 Tag들 만나보기
   - <h1> </h1> , <h2> </h2> : 강조할때 또는 제목을 작성할때 사용
   - <p> </p> : 하나의 문단임을 나타내줌
   - <input> : 사용자로부터 입력을 받게 하는 태그

### 3. 크롬에서 개발자 도구 사용하기
→ f11를 누르면 나옴

   
## <웹 기초 스터디 4주차 과제\_빙고 만들기>

1. <ul> : unordered list, 순서가 없는 list

   → 순서가 없기 때문에 글자 앞에 불릿(동그라미)가 붙음

   ```html
   <ul>
     <li>가장 좋아하는 동물을 형광팬으로 그어봅시다.</li>

     <li>가장 싫어하는 동물을 볼드체와 밑줄로 강조해봅시다.</li>
   </ul>
   ```

2. <mark>강조하고자 하는 내용</mark>

   → 해당 부분에 노란색 형광펜 표시가 됨

3. <strong>볼드체로 표현할 부분</strong>
4. <u>밑줄칠 부분</u>
5. 표 만들기

   - <table> </table> : 해당 태그 안에 표를 만드는데 필요한 모든 태그들 들어감
   - border = “1” : 표의 테두리의 선 굵기 지정
   - <tr> </tr> : 표의 한 행을 의미. 해당 태그 안에 들어갈 열을 하나씩 작성
   - <td> </td> : 열의 각 내용을 작성
   - alingn = “left / center / right” : 각 열의 요소들이 왼쪽/가운데/오른쪽에 정렬될지를 결정
   - bgcolor = “색깔” : 표 행의 뒷 배경색을 의미

   ```html
   <table border="1">
     <tr alingn="left" bgcolor="white">
       <td>강아지</td>
       <td><mark>고양이</mark></td>
       <td>곰</td>
     </tr>
     <tr alingn="left" bgcolor="white">
       <td>닭</td>
       <td>말</td>
       <td>돼지</td>
     </tr>
     <tr alingn="left" bgcolor="white">
       <td>고라니</td>
       <td>호랑이</td>
       <td>
         <strong><u>개미 핥기</u></strong>
       </td>
     </tr>
   </table>
   ```

6. <input> : 사용자로부터 입력을 받는 요소

   1. <placeholder> : 해당 입력 받는 부분의 뒷배경에 작성되어 있는 글씨
   2. <label> : input 입력 창 앞에 있는 텍스트

      ```html
      <div>
        <label for="animal_id">이번 차례 체크할 동물 : </label
        ><input
          type="text"
          id="animal_id"
          placeholder="동물 이름을 입력하세요.."
        />
      </div>
      ```

→ **최종 결과**
![image](https://user-images.githubusercontent.com/110219986/230122050-d74bd79f-e7d4-46e9-88d0-0bc0d527b307.png)

