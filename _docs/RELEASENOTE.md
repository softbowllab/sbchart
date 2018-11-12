---
title:  RELEASE Note
date:   2018-07-27
layout: default.md
permalink: /:collection/releasenote:output_ext
---

# Release Note
---
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
* `axis.x.type`이 category일 때, `x.tick.format` 파라미터에 category name 추가
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

