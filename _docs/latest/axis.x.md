---
title:  axis.x
date:   2018-05-14
categories: ["latest","axis"]
order: 2
---

## axis.x
---

x축관련 값들을 설정합니다.

x축이 없는 원(pie), 도녓(donut) 계열 차트는 지원하지 않습니다.
`#2.0.0`

* Type : object

* Format
```javascript
axis: {
	x : {
		show:false,
		type: "indexed",
		max: 10,
		min: 1,
		height: 20
	}
}
```

### axis.x.show

x축의 show/hidden 을 지정합니다.
`#2.0.0`

* Type : boolean

* Default : true


### axis.x.type

x축의 형태를 지정한다.

* Type : string

* Default : "indexed"

* Values
  * "timeseries": x축을 시간순으로 배열
  * "indexed": x축을 데이터순으로 일정하게 배열
  * "category": 카테고리(x축 라벨 수동 지정, axis.x.categories = []

### axis.x.min

x축 값 범위의 최소값을 지정한다.

axis.x.type = "timeseries" 인 경우는 동작하지 않는다.

* Type : number


### axis.x.max

x축 값 범위의 최대값을 지정한다.

axis.x.type = "timeseries" 인 경우는 동작하지 않는다.

* Type : number

### axis.x.height

x축 영역의 높이를 강제 지정한다.

* Type : number

