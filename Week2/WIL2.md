# 2023-1-OC-Web-Study

### 필수 과제

**1. git의 명령어 add, commit, push는 각각 어떤 역할을 하는지 정리하고, git pull과 fetch의 차이점을 정리하시오.**

    (1) add : working directory에서 staging area로 내가 원하는 파일/다이렉토리를 보내는 명령어
    (2) commit : staging area에서 local repository로 내가 원하는 파일/다이렉토리를 보내는 명령어
    (3) push : local respository에서 remote respository로 내가 원하는 파일/다이렉토리를 보내는 명령어

    (4) git pull : git remote 명령을 통해 서로 연결된 원격 저장소의 최신 내용을 local respository로 가져오며 병합
        → git push와 반대 성격
        → 자동으로 병합을 해줌

    (5) git fetch : local respository와 remote respository의 변경 사항이 다를때 이를 비교 대조하고, git merge 명령어와 함께 최신 데이터를 반영하거나 충돌 문제 등을 해결
        → 자동으로 병합을 해주지 X

**2. 지난 주와 이번주 학습 내용을 정리하고 WIL을 작성하여 제출한다.**

## 1주차 : Web

**1. 주소 : resource(허니콤보)가 저장된 주소**

    - URI : resource를 식별하는 통일된 방식
      - 허니콤보를 얻을 수 있는 방식
    - URN : Uniform Resource Name 이름으로 찾기!
                 ex. 도서 출판 번호
    - URL : Uniform Resource Location 교촌치킨 신촌점
      - URL은 프로토콜 + DNS 주소 로 이루어져 있음.

**2. 서버 & 리소스**

    → 서버 : 컴퓨터 (ex. 홍익대학교 컴퓨터)

    → 리소스 : 정보들 (ex. 홍익대학교가 제공하는 정보들)

**3. DNS 주소가 탄생하게 된 배경 - 문제점들**

    (a) 사람은 길고 복잡한 IP 주소들을 외우거나 관리하기 너무 힘들었음.

          (원래는 복잡한 IP 주소를 통해 리소스에 접근해야했음)

    (b) IP 주소는 사정에 따라 변동 가능함

**4. DNS : Domain Name System**
→ 이름으로 서버를 접근할 수 있게 해주는 것 (원래의 IP 주소, 즉 숫자들이 아니라)

**5. Resource : HTML, CSS, JS file들**

    → 해당 사이트를 방문하면 3가지 정보들을 우리에게 제공
    → 받은 정보들을 가지고 그려주는 친구들 (ex. 크롬, 인터넷 익스플로어)
    → HTML, CSS, JS를 재료 삼아서 브라우저가 그림을 그려줌 (랜더링)
     (a) HTML : 자료 (뼈대)
     (b) CSS : UI (살과 옷)
     (c) Javascript : 제어 체제
        ex. 움직이는 그림들, 변화하는 배너들

    결론 : 브라우저에 URL를 입력 → DNS 서버가 내가 원하는 서버로 이동시켜줌 → 3가지 정보를 제공 → 브라우저가 예쁜 그림을 그려서 우리에게 보여줌

## 2주차 : Git / Github

# 1. Git

    → 컴퓨터 파일의 변경사항을 저장하고, 변경사항을 추적할 수 있음.

    → 사람들 사이의 작업을 조율할 수 있음

    → 코드에 수많은 분기들(많은 버전들)을 만들 수 O

(1) branch : 분기들(나무처럼 갈라지는 모습)

    → 분기를 나눌수도, 합칠수도 O

    → 변화 추적 (버전 관리 가능)

    → 특정 시점으로 되돌리기

# 2. Git 기본 동작 방식

(1) 파일의 4가지 상태

    (a) 추적 X

    → 여기부터는 추적을 O는 구간들

    (b) 변경 X

    (c) 변경 O

    (d) staged

Working Directory → Staging Area → Local repository
→ add로 staging area로 보냄

명령어 : **git add**

→ staging area가 있는 이유 : 논리적으로 단계를 보여주기 위해서

    ex. 최종 결과물인 A를 만들기 위해 나는 B, C, D라는 단계들을 거쳤어

→ staging area에서 commit을 통해 local repository(git에서 관리하는 저장 공간) 로 보냄

명령어 : **git commit**

3. **Git으로 협업하기**

Remote repository = GitHub

    → Working Directory, Staging Area, Local Repository는 다 내 컴퓨터에 있는것

    → 다른 사람과의 협업을 하기위해서 remote respository를 사용해 거기에 저장시키겠다!!!

    → 사용되는 명령어 : **git push**
