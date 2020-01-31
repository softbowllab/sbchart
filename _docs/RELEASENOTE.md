---
title: RELEASE Note
date: 2018-07-27
layout: default.md
permalink: /:collection/releasenote:output_ext
---

# Release Note
---
## 2.0.21
`2020.01.31`

#### 기능 개선
* gauge chart, stack data 표현 가능하게 변경
* title, extend.donut.title 에서 \n으로 줄바꿈 가능하게 변경
* data에 null 허용 가능하게 변경
- bubble chart, data.columns일 때 배열로 입력하여 bubble 크기를 사용자가 지정 가능하게 변경
```
	ex) columns = [
			["data1", 20, [30, 50], 70, [40, 10], 20],
			["data2", [10, 20], 70, 40, 50, [60, 30]],
			["data3", 80, 60, [90, 20], 30, [40, 70]],
		]
```       

#### 옵션 추가
* extend.bar.padding 추가
* axis.x/y/y2.tick.culling.max 추가
* axis.x/y/y2.tick.line.show, axis.x/y/y2.tick.text.show, axis.x/y/y2.domain.show 추가

#### 버그 수정
* pie, donut, gauge chart fullcircle이 아닐 때, animation 오류 수정


## 2.0.20
`2020.01.03`

#### 기능 개선
* 차트 기본색상 변경

#### 기능 추가
* Scroll 기능 추가
* Zoom 기능 추가

#### 옵션 추가
* `axis.x.scroll.show`, `axis.x.scroll.xSize`, `axis.x.scroll.wheel` 추가
* `axis.x.zoom.type`, `axis.x.zoom.maxScale` 추가

## 2.0.19
`2019.11.20`

#### 기능 추가
* 이미지 다운로드 추가
* 범례 아이템 클릭 시 해당 차트 숨기기, 보이기 기능 추가
* `data.noData`에 이미지 경로 입력 시 이미지가 나오게 변경

#### 기능 개선
* IE9 지원

#### 옵션 추가
* `global.export.show` 추가
* `legend.item.onclick` 추가

#### 버그 수정
* Radar Chart가 `global.animation.show = true`일 때 IE에서 나오지 않는 현상 수정


## 2.0.18
`2019.10.04`

#### 옵션 추가
* `legend.item.paddingBottom` 추가
* `legend.item.tile.point` (rect/circle) 추가 
* `legend.item.tile.position` (left/right) 추가 

## 2.0.17
`2019.09.17`

#### 기능 추가
* Y2축 기능 추가

#### 옵션 추가
* `axis.axes`, `axis.y2` 옵션 추가


## 2.0.16
`2019.08.26`

#### 옵션 추가
* `data.noData` 추가 - 데이터가 없을 경우 문구 설정 기능 추가

#### 버그 수정
* stackarea percent chart에서 `global.pattern = true` 일 때 point 위치 오류 수정


## 2.0.15
`2019.07.10`

#### 기능 개선 

* radar chart에서 `axis.x.type`을 category로 고정
* radar chart에서 `global.pattern`의 형태를 area와 같은 형태로 변경
* scatter plot chart에서 `axis.x.type`을 indexed로 고정

#### 버그 수정

* radar chart `tooltip` 위치가 틀어지는 현상 수정
* step chart에서 `global.pattern="true"` 일 때 legend의 tile과 차트의 모양이 일치하지 않는 부분 수정
* step chart에서 `global.pattern="true"` 일 때 legend의 tile과 tooltip의 tile이 일치하지 않는 부분 수정
* scatter plot chart에서 `global.pattern="true"` 일 때 legend의 tile과 차트의 모양이 일치하지 않는 부분 수정
* scatter plot chart에서 `global.pattern="true"` 일 때 legend의 tile과 tooltip의 tile이 일치하지 않는 부분 수정
* bubble chart에서 `global.pattern="true"` 일 때 pattern이 정상적으로 나오지 않는 현상 수정


## 2.0.14
`2019.07.02`

#### 차트 추가

* Scatter Plot, Radar Chart 추가

#### 옵션 추가 

* `data.x`, `data.xs` 추가

#### 버그 수정

* `tooltip.grouped = false` 일 때 툴팁이 차트 영역 밖에 표시되는 현상 수정


## 2.0.13
`2019.05.14`

#### 기능 추가

* 차트 애니메이션 기능 추가

#### 옵션 추가

* `global.animation.show`, `global.animation.type`, `global.animation.types`, `global.animation.delay`, `global.animation.ease` 추가

#### 기능 개선

* step chart에서 `tooltip.grouped = false` 일 때 tooltip이 나타나는 영역 개선

#### 버그 수정

* bubble chart에서 `axis.rotated = true` 일 때 음수값의 label이 왼쪽으로 치우쳐있는 현상 수정
* stacked area percent chart에서 `axis.rotated = true` 일 때 크롬에서 가장 우측 label이 잘리는 현상 수정


## 2.0.12
`2019.05.02`

#### 옵션 추가

* `tooltip.sort` 추가 (asc, desc)

#### 버그 수정

* pie chart에서 `extend.pie.padding`을 2 이상 적용 시 라벨이 사라지는 현상 수정
* stacked area percent chart에서 `axis.x.type = timeseries`일 때 data.labels 및 tooltip이 표시되지 않는 현상 수정
* combination chart에서 툴팁 순서가 데이터 순으로 나오지 않는 현상 수정
* step chart에서 `tooltip.grouped = false` 일 때 point가 나타나는 현상 수정


## 2.0.11
`2019.04.15`

#### 차트 추가

* stacked area, stacked area (percent), stacked area-spline, stacked area-spline (percent) 차트 추가

#### 기능 개선

* stacked percent chart에서 `axis.y.tick`에 % 표시 추가


## 2.0.10
`2019.03.12`

#### 차트 추가

* step, area-step, area-spline 차트 추가

#### 기능 변경

* line, spline, area, bubble 차트에서 `axis.rotated = true` 적용되게 변경


## 2.0.9
`2019.01.30`

#### 기능 추가

* 웹 접근성 기능 추가

#### 옵션 추가

* `global.accessibility.use`, `global.accessibility.title`, `global.accessibility.description` 추가 
* `global.pattern` 추가



## 2.0.8
`2018.12.14`


#### 기능 변경

* `legend.position = bottom` 일 때, 마지막 범례 우측으로 legend.padding이 적용되지 않게 변경

#### 버그 수정

* `legend.background = true` 일 때, background 위치 조정



## 2.0.7
`2018.12.13`

#### 기능 개선

* `legend.background` 옵션 추가

#### 버그 수정

* 원 차트의 크기에 따른 label, legend 위치 변경


## 2.0.6
`2018.11.06`

#### 신규 차트

* 버블(bubble) 차트

#### 버그 수정

* 게이지(gauge) 차트의 min, max 값에 따른 값 계산오류 `extend.gauge.min`, `extend.gauge.max`

* 게이지(gauge), 도넛(donut) 차트에서 차트 크기에 따른 내부 원 반지름 비율 계산오류


## 2.0.5 
`2018.10.30`

#### 버그 수정

* 원, 도넛 차트에서 영역 시작점(각도) 변경


## 2.0.4 
`2018.10.26`

#### 신규 차트

* 게이지(gauge) 차트

#### 기능 개선

* 도넛차트 내부 원 내부에 문자열 표현 기능 추가 `extend.donut.title`

#### 버그 수정

* `axis.x.type = "category"` & `axis.x.tick.centered = true` 일 때 첫번째 tick이 사라지는 현상
* `axis.x.type = "category"` & `axis.x.tick.outer = false` 일 때 우측 tick이 사라지지 않는 현상

## 2.0.3 
`2018.09.14`

#### 버그 수정

* `axis.x.type`이 `timeseries`일 때, tooltip이 표시되지 않는 현상
* `axis.x.type = "timeseries"`에서 데이터가 시간 순이 아닐 때, 시간 순으로 자동 정렬

#### 기능 개선

* 범례 항목 마우스 event (legend.item.onmouseover, legend.item.onmouseout) 추가
* zerobased 옵션 변경
	* `extend.bar.zerobased`, `extend.area.zerobased` 옵션 제거
	* `axis.y.zerobased` 옵션 추가
	* bar와 area에서만 적용되던 zerobased 옵션이 공통으로 변경됨에 따라, line, spline 에서도 영향을 받게 변경
* `axis.x.type`이 category일 때, `axis.x.tick.format` 파라미터에 category name 추가
* `data.groups` 옵션 추가 : stacked bar 차트 계열에서 범례별 묶음(그룹화) 처리 지원

## 2.0.2 
`2018.08.22`

#### 버그 수정

* pie, donut 차트에서 label.show가 false일 때 tooltip이 표시되지 않는 현상

#### 기능 개선

* stacked bar 계열 차트의 data.labels 표시 추가
* d3 Version 업데이트 (v5.5.0)
* svg 구조 및 class명 변경
* sbchart.css minify

## 2.0.1 
`2018.08.09`

#### 버그 수정

* sbgrid와 함께 사용할 경우 toFixed 동작하지 않는 현상
* window resize 시 pie, donut 차트 사라지는 현상
* data name에 띄어쓰기가 들어갈 경우 data labels가 나타나지 않는 현상
* IE에서 stackbar 차트가 나타나지 않는 현상

## 2.0.0 
`2018.08.01`

* **Renewal Launching**
