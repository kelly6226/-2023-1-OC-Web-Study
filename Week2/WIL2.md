# 2023-1-OC-Web-Study

2주차 : Git / Github

1. Git

→ 컴퓨터 파일의 변경사항을 저장하고, 변경사항을 추적할 수 있음.

→ 사람들 사이의 작업을 조율할 수 있음

→ 코드에 수많은 분기들(많은 버전들)을 만들 수 O

(1) branch : 분기들(나무처럼 갈라지는 모습)

→ 분기를 나눌수도, 합칠수도 O

→ 변화 추적 (버전 관리 가능)

→ 특정 시점으로 되돌리기

2. Git 기본 동작 방식

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
