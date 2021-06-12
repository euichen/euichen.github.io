---
layout: post
title: 니들이 AR지도를 R A? (AR 네비게이션 앱 - 졸업작품)
image: navi.png
date: 2021-06-07 17:35:20 +0200
tags: [Unity, Android, AR, Capstone Design, 졸업작품]
categories: Android
---


개발 의도 : AR navigation을 앱으로 만들어 학교에서 유용하게 사용해보자
<br><br><br><br>


+ ## 기획 의도 
    + GPS 기반의 기존의 2D navigation의 불편함을 해소하기 위해
    + 학교 시설에 대한 홍보 및 정보를 제공하여 시설의 사용도를 높이기 위해
    + 길찾기의 어려움을 해소하기 위해
<br><br><br><br>

+ ## 개발 환경 
    + Unity
    + Mapbox
    + Android
<br><br><br><br>

+ ## 구축 
    + Mapbox의 Map SDK for Unity를 사용하여 안드로이드 기기에서 캠퍼스 지도를 3D 오브젝트 형태로 나타냄
    + 3D형태로 나타내어진 지도 위에 건물들의 정보를 AR로 표현하여 쉽게 건물을 찾을 수 있도록 나타냄
    + Mapbox 지도 위에 현재 자신의 위치와 목적지의 위치를 나타내고 목적지까지의 경로를 AR로 표현할 수 있도록 구현

![]({{site.baseurl}}/images/NV/struct.png)
<br><br><br><br>

+ ## 구조도
![]({{site.baseurl}}/images/NV/struct1.png)
<br><br><br><br>

+ ## 핵심 스크립트
```
void Query()
{
	var count = _waypoints.Length;
	var wp = new Vector2d[count];
	for (int i = 0; i < count; i++)
	{
		wp[i] = _waypoints[i].GetGeoPosition(_map.CenterMercator, _map.WorldRelativeScale);
	}
	var _directionResource = new DirectionResource(wp, RoutingProfile.Driving);
	_directionResource.Steps = true;
	_directions.Query(_directionResource, HandleDirectionsResponse);
}
```
     입력된 목적지 정보와, 현재 사용자의 위치를 이용하여 Mapbox에서 제공한 지도에 맞게 길 찾기 생성

<br><br><br><br>

+ ## 실행
![]({{site.baseurl}}/images/NV/ing1.png)
![]({{site.baseurl}}/images/NV/ing2.png)
<br><br><br><br>

+ ## 느낀점
    + 길찾기 알고리즘을 이용하여 사용자 위치와 목적지 위치를 GPS를 이용하기 위해서 미리만들어진 컴포넌트를 분석하고 이를 스크립트 단위에서 수정하기 위해서 정말 많은 시간과 노력이 들어갔다.
    + unity mapbox에 대한 정보가 너무 부족해서 스스로 공부하고 여러 방법을 시도하면서 정이 정말 많이 들어갔다.  
<br><br><br><br>





