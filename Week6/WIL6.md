### 개구리 게임 1-13 & 18-20 stage 답
<br>

- 개구리 게임 링크 주소 : https://flexboxfroggy.com/#ko <br>
  <br>
**각 문제의 답 앞에는 display: flex; 속성이 有** <br>
🐸 **stage 1**의 답 : justify-content: flex-end; <br>
🐸 **stage 2**의 답 : justify-content: center; <br>
🐸 **stage 3**의 답 : justify-content: space-around; <br>
🐸 **stage 4**의 답 : justify-content: space-between; <br>
🐸 **stage 5**의 답 : align-items: flex-end; <br>
🐸 **stage 6**의 답 : justify-content: center;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;align-items: center;<br>
🐸 **stage 7**의 답 : justify-content: space-around; &nbsp; &nbsp; align-items: flex-end;<br>
🐸 **stage 8**의 답 : flex-direction: row-reverse; <br>
🐸 **stage 9**의 답 : flex-direction: column; <br>
🐸 **stage 10**의 답 : flex-direction: row-reverse; &nbsp; &nbsp; justify-content: left;<br>
🐸 **stage 11**의 답 : flex-direction: column; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; justify-content: flex-end; <br>
🐸 **stage 12**의 답 : flex-direction: column-reverse; &nbsp; &nbsp; justify-content: space-between;<br>
🐸 **stage 13**의 답 : flex-direction: row-reverse; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  justify-content: center; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; align-items: flex-end;<br>
🐸 **stage 18**의 답 : flex-wrap: wrap;<br>
🐸 **stage 19**의 답 : flex-direction: column; &nbsp; &nbsp; flex-wrap: wrap;<br>
🐸 **stage 20**의 답 : flex-flow: column wrap; <br>

<br>

### 개구리 게임 완료 인증샷
![image](https://user-images.githubusercontent.com/110219986/235890230-192e1553-ac4c-4047-96ee-bdcce26bea03.png)




### 6주차 수업 정리 : Box model & Flex

#### 1. Box model

1. 블록 레벨 요소 : 한 줄을 차지하는 박스
    
    → ex) div, p, h1
    
2. 인라인 레벨 요소 : 자신만을 감싸는 박스
    
    → ex) span, strong
    

#### 2. Padding

   → content와 border 사이의 간격

#### 3. Margin

   → 여백 (요소들 간의 공간)

#### 4. FLEX Box Layout

→ flexible box layout : 아이템이 배열될 방향인 주축을 정할 수 有

```css
.flex-box {
	display: flex;
	flex-direction: row;
	jusfity-content: //같은 라인에서 어디에 아이템들이 정렬될지를 정해주는 요소
}
```

→ flex-end : justify-content의 가능한 값의 예시

→ space-around : “ (균등한 공간을 가지고 배치가 되도록 함)

+) 더 알아보기!  1) grid layout  2) can i use 홈페이지 사용 ← 어느 버전부터 어떠한 요소 지원하는지 알 수 있음
