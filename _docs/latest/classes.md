---
title: classes
date:   2018-06-29
categories: ["latest","CLASS"]
order: 0
---

## CSS classes
---

CSS 클래스 입니다.

chart, title, axis, legned, grid, tooltip 등 차트내 각 영별로 classes 가 정의되어 있습니다.
`#2.0.0`


### chart

* .sbchart-chart : x,y축 라벨, 타이틀을 제외한 순수 영역. `#2.0.0`

* .sbchart-series :  Series(범례) 영역 `#2.0.0`


### title

* .sbchart-title : 타이틀 최상위. `#2.0.0`

* 예

   ```css
.sbchart-title { font-size:16px; font-weight:bold; }	/* 타이틀 폰트 사이즈 변경 */
```




### axis

* .sbchart-axis : x,y축 공통. `#2.0.0`

* .sbchart-axis-x  : x축 최상위. `#2.0.0`

* .sbchart-axis-x .tick text : x축 tick 텍스트. `#2.0.0`

* .sbchart-axis-x .tick line : x축 tick 라인. `#2.0.0`

* .sbchart-axis-x .domain : x축선. `#2.0.0`

* .sbchart-axis-x-label : x 축 라벨. `#2.0.0`

* .sbchart-axis-y : y축 최상위 클래스. `#2.0.0`

* .sbchart-axis-y .tick text : y축 tick 텍스트. `#2.0.0`

* .sbchart-axis-y .tick line : y축 tick 라인. `#2.0.0`

* .sbchart-axis-y .domain : y축 축선. `#2.0.0`

* .sbchart-axis-y-label : y 축 라벨. `#2.0.0`

* 예

   ```css
.sbchart-axis-x .tick text {font-size:13px;}	/* x축 tick 폰트 크기 변경 */
.sbchart-axis-x .tick line {display:none;}	/* x축 tick 라인(눈금) 없애기 */
.sbchart-axis-x .domain {display:none}	/* x축 선 없애기 */
.sbchart-axis-x .sbchart-axis-x-label {font-size:14px;}	/* x축 라벨 폰트 크기 변경 */
```


### legend 

* .sbchart-legend : 범례 최상위. `#2.0.0`

* .sbchart-legend .sbchart-legend-background : 범례 배경. `#2.0.0`

* .sbchart-legend .sbchart-legend-item : 범례 아이템. `#2.0.0`

* .sbchart-legend .sbchart-legend-item .sbchart-legend-item-text : 범례 텍스트. `#2.0.0`

* .sbchart-legend .sbchart-legend-item .sbchart-legend-item-tile : 범례 Tile. `#2.0.0`

* .sbchart-legend .sbchart-legend-item .sbchart-legend-item-event : TODO. `#2.0.0`

* 예

   ```css
.sbchart-legend .sbchart-legend-background {stroke-width: 0}	/* 범례 박스 라인 없애기 */
.sbchart-legend .sbchart-legend-item-text {font-size:14px;}	/* 범례 텍스트 폰트 크기 변경 */
```

### grid

* .sbchart-grid : 그리드 x,y축  공통. `#2.0.0`

* .sbchart-grid-x : 그리드 x축 최상위. `#2.0.0`

* .sbchart-grid-x .sbchart-grid-x-line : 그리드 x축 라인. `#2.0.0`

* .sbchart-grid-y : 그리드 y축 최상위. `#2.0.0`

* .sbchart-grid-y .sbchart-grid-y-line : 그리드 y축 라인. `#2.0.0`


### tooltip

* .sbchart-tooltip : TODO `#2.0.0`

* .sbchart-tooltip-title : TODO `#2.0.0`

* .sbchart-tooltip-cont : TODO `#2.0.0`


### 기타

* .sbchart-legend-arc : 원형 차트(Pie, Donut)의 영역(호)에 대한 값의 텍스트. `#2.0.0`
