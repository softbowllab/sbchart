---
title:  axes.x
date:   2018-05-14
categories: ["latest","axes"]
order: 2
---

## axes.x
---

x축관련 값들을 설정합니다.

x축이 없는 원(pie), 도녓(donut) 계열 차트는 지원하지 않습니다.
`#2.0.0`

* Type : object

* Format
```javascript
axes: {
	x : {
		show:false,
		type: "indexed",
		tick: {
			format: function(d) { return d + "%"; },
			count: 5,
			fit: false,
			values: [2,4,10]
		}
	}
}
```

### axes.x.show

x축의 show/hidden 을 지정합니다.
`#2.0.0`

* Type : boolean

* Default : true


### axes.x.type

x축의 형태를 지정한다.

* Type : string

* Default : "indexed"

* Values
  * "timeseries": x축을 시간순으로 배열
  * "indexed": x축을 데이터순으로 일정하게 배열
  * "category": 카테고리(x축 라벨 수동 지정, axes.x.categories = []
