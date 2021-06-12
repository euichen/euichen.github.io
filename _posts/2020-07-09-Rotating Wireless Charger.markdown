---
layout: post
title: 아두이노를 활용한 회전 무선 충전기 만들기 - 장려상
image: wmc.PNG
date: 2020-07-09 13:35:20 +0200
tags: [Arduino, C++, Capstone Design, 장려상]
categories: Arduino
---

개발 의도 : 하나의 무선 충전기로 다수의 무선 제품을 충전하여 충전 효율을 높이고 쉽고 간편하게 사용할 수 있도록 개발하자
<br><br><br><br>

+ ## 재료
___
![]({{site.baseurl}}/images/Charger/Material.PNG)

납땝 인두, 열수축 튜브, 나사 기타등등
<br><br><br><br>

___
# 제작 과정
___


+ ## 과제 계획 및 예상도 만들기
___

![]({{site.baseurl}}/images/Charger/plan.PNG)
<br><br><br><br>

+ ## 필수 해결 과제
___
    + 아두이노가 충전모듈의 신호를 읽을 수 있어야 이 프로젝트가 성공할 수 있다.

![]({{site.baseurl}}/images/Charger/wmc_c.PNG)
<br><br><br><br>

+ ## 3d 모델링
___

![]({{site.baseurl}}/images/Charger/3d.PNG)
<br><br><br><br>

+ ## 모듈 완성
___

![]({{site.baseurl}}/images/Charger/Module.PNG)
<br><br><br><br>

+ ## 결합
___

![]({{site.baseurl}}/images/Charger/Support.PNG)
![]({{site.baseurl}}/images/Charger/combine.PNG)
<br><br><br><br>

+ ## 완성품
___

![]({{site.baseurl}}/images/Charger/Support.PNG)

<br><br><br><br>

+ ## 소프트웨어 제작
___
    1. 동작 모드(버튼으로 전환 가능) 
        + 대기 모드
        + 1회전 모드
        + 무한 회전 모드
    2. 모드 변화 LED등
        + 종료 및 시작 시 모든 LED 등 두번 점멸 
        + 1회전 모드 시작 시 시계방향으로 LED등 점멸
        + 무한 모드 시작 시 시계방향으로 LED등 점멸
    3. 충전이 완료된 칸 충전완료 등 표시
        + 윗판은 돌아가고 LED가 있는 밑판은 돌아가지 않는다.
        완료표시 LED등이 같이 회전한다.
        + 완료 표시등이 충전 칸에 돌아온 경우 위에 기기가 없을 경우(사람이 가져간 경우) LED등을 끈다.
    4. 충전 신호
        + 충전신호와 종료 신호는 무선 충전 모듈에서 신호를 읽어 온다. 
<br><br><br><br>


+ ## 결과
![]({{site.baseurl}}/images/Charger/ing.png)
    + 불이 켜져 있는 두 이어폰은 충전이 완료된 상태
    + 불이 꺼져있는 이어폰은 충전을 기다리는 상태
    
    작동영상은 github를 참고해주세요


    
    



