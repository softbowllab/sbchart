---
title:  options
date:   2018-06-18
categories: ["latest","API"]
order: 0
---

## Options API

`#2.0.0`

---

### data()

데이터 옵션을 지정하거나 조회합니다.

* Example

  ```javascript
var chart = new sb.chart("#chartWrap");
chart.data({
    columns: [
    	["2015",3.51,4.6,3.43,7.96,3.37,5.83,0.35,3.23,-0.09,4.47,2.21,1.13,0.77,0.35,0.92,2.65,1.64,8.08],
        ["2016",0.71,2.14,3.18,-1.84,0.79,0.35,0.28,0.44,0.79,0.84,1.33,-0.7,-1.51,0.09,1.05,-1.66,-0.58,4.63],
        ["2017",1.48,3.64,2.35,1.29,1.42,1.34,1.51,-1.08,4.29,1.67,2.4,-0.36,-0.53,1.98,2.23,-0.9,-1.62,1.66]
    ]
}).render();
var columns = chart.data();
```


### grid()

`#2.0.0`

그리드 옵션을 지정하거나 조회합니다.

* Example

  ```javascript
var chart = new sb.chart("#chartWrap",conf);
chart.grid({
    x: { show: false }
}).render();
var opt = chart.grid().x.show;
```


### title()

`#2.0.0`

타이틀 옵션을 지정하거나 조회합니다.

* Example

  ```javascript
var chart = new sb.chart("#chartWrap",conf);
chart.title({
    text = "시도별 주택가격 변동률"
}).render();
var opt = chart.title().text;
```


### legend()

`#2.0.0`

범례 옵션을 지정하거나 조회합니다.

* Example

  ```javascript
var chart = new sb.chart("#chartWrap",conf);
chart.legend({
    show: false
}).render();
var opt = chart.legend().show;
```

### tooltip()

`#2.0.0`

툴팁 옵션을 지정하거나 조회합니다.


### axis()

`#2.0.0`

X, Y 축 옵션을 지정하거나 조회합니다.

* Example

  ```javascript
var chart = new sb.chart("#chartWrap",conf);
chart.axis({
    x : {
        label: "지역별"
    }
}).render();
var opt = chart.axis().x.label;
```


### extend()

`#2.0.0`

확장 옵션을 지정하거나 조회합니다.

* Example

  ```javascript
var chart = new sb.chart("#chartWrap",conf);
chart.extend({
    point : {
        show: false
    }
}).render();
var opt = chart.extend().point.show;
```