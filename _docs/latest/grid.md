---
title: grid
date: 2018-05-14
categories: ["latest","grid"]
order: 999
---

## grid

`#2.0.0`

---

그리드를 설정합니다.

X, Y축이 없는 원 계열 차트(원, 도넛, 게이지)는 해당되지 않습니다.

* Type : Object

* Format
```javascript
grid: {
	x: { 
		show: true
	},
	y: { 
		show: false,
		ticks: 5
	}
}
```


### grid.x.show

`#2.0.0`

X축 그리드를 show/hide 처리합니다.

* Type : Boolean

* Default : true

### grid.y.show

`#2.0.0`

Y축 그리드를 show/hide 처리합니다.

* Type : Boolean

* Default : true

### grid.y.ticks

`#2.0.0`

Y축 그리드 Tick 개수를 지정합니다.

* Type : Number
