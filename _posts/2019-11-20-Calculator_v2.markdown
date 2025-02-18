---
layout: post
title: 진변변환 + 사칙연산 계산기
image: cal_v2.png
date: 2019-11-20 15:35:20 +0200
tags: [JAVA, exe]
categories: exe
---


개발 의도 : 계산기를 만든 후 너무 단순하다 싶어 새로운 기능을 추가시켰다.
<br><br><br><br>



+ ## 기획 의도 
___
    + 과학기술의 발전에 한계에 따라 2진법체제에서 3진법체제로 갈 가능성이 열린 지금 이시기에 더욱더 진법에 대해 이해할 필요성을 느끼고 기획하게 되었다.
    + 책에서 진법에 대해 공부하다 보면 단순한 예제를 제외하곤 결과값을 확인할 수 없는 불편함을 느꼈고 해설의 부재 또한 너무 많았다.
    진법을 공부하고자 하는 사람들에게 위와 같은 불편함을 해결하고 좀 더 간편하고 효율적으로 사용되고자 만들게되었다.
<br><br><br><br>

+ ## 프로그램 개요 
___
    + 진법 계산과 결과에 대한 해설을 포함하는 진법게산프로그램이다.
<br><br><br><br>

+ ## 사용자 인터페이스 구상
___
    + 원도우 표준 계산기 모양 + 진법변환을 위한 키 + 해설지 
<br><br><br><br>
   
+ ## 소프트웨어 핵심기능
___
    + 진법변환을 자유롭게 계산할 수 있다.
    + 진법계산을 사용할 경우 옆 해설지에 해설이 나타난다.
    + *, /, +, - 다수 포함된 식을 우선순위에 따라 계산한다.
    + () 사용한 우선순위 조정을 통해 완벽한 게산을 유도한다. 
    + 예) ( 3 + 4 ) * 5 = 35
<br><br><br><br>

+ ## 함수 구조 및 알고리즘
___
![]({{site.baseurl}}/images/Calculator/struct_v2.PNG)

<br><br><br><br>

+ ## 사용자 인터페이스 및 작동화면
___
![]({{site.baseurl}}/images/Calculator/ing_v2.PNG)
<br><br><br><br>

+ ## 개발 후기
___
    + 괄호 부분 (()),()() 중복괄호와 병력괄호 두개를 동시에 해결할 수 있는 알고리즘을 생각하는데 시간이 많이 소모되었다.












