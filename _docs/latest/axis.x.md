---
title: axis.x
date: 2018-05-14
categories: ["latest","axis"]
order: 5
---

## axis.x

`#2.0.0`

---

X축 관련 값들을 설정합니다.

X축이 없는 원 계열 차트(원, 도넛, 게이지) 차트는 해당되지 않습니다.

* Type : Object

* Format
```javascript
axis: {
	x: {
		show: false,
		type: "indexed",
		max: 10,
		min: 1,
		height: 20,
		localtime: true
	}
}
```

### axis.x.show

`#2.0.0`

X축 show/hide를 지정합니다.

* Type : Boolean

* Default : true


### axis.x.type

`#2.0.0`

X축의 형태를 지정합니다.

* Type : String

* Default : "indexed"

* Values
	* "indexed": `Default` x축을 데이터 순으로 일정하게 배열합니다.
	* "category": X축 라벨 수동 지정합니다. `axis.x.categories = []` 값도 함께 지정해야 합니다.
	* "timeseries": X축을 시간 순으로 배열합니다. `axis.x.categories = []` 값도 함께 지정해야 합니다.

### axis.x.min

`#2.0.0`

X축 값 범위의 최솟값을 지정합니다.

* Type : Number


### axis.x.max

`#2.0.0`

X축 값 범위의 최댓값을 지정합니다.

* Type : Number

### axis.x.height

`#2.0.0`

X축 영역의 높이를 지정합니다.

* Type : Number

### axis.x.localtime

`#2.0.0`

X축 시간대를 처리하는 방법으로 true인 경우 x값을 localtime으로 처리, false이면 내부적으로 UTC로 변환합니다.

* Type : Boolean

* Default : true
