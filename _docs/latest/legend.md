---
title: legend
date: 2018-05-14
categories: ["latest","legend"]
order: 1
---

## legend

`#2.0.0`

---

범례의 위치, 형태 등을 지정합니다.

* Type : Object

* Format
```javascript
legend: {
	show: true,
	background: false,
	position: "inset",
	inset: {
		anchor: "top-left",
		x: 10,
		y: 0
	},
	padding: 10
}
```

### legend.show

`#2.0.0`

범례의 show/hide 여부를 지정합니다.

* Type : Boolean

* Default : true

### legend.position

`#2.0.0`

범례의 위치를 지정합니다.

* Type : String

* Default : "bottom"

* Values

	* bottom: `Default` 아래에 위치
	* right: 우측에 위치
	* inset: 차트 내에 위치, 자세한 사항은 [legend.inset](./legend.inset.html) 참조

### legend.background

`#2.0.7`

`legend.position = "bottom" or "right"`인 경우 범례의 백그라운드 영역을 표시합니다.

`legend.position = "inset"`인 경우에는 항상 백그라운드 영역을 표시됩니다.

* Type : Boolean

* Default : false


### legend.padding

`#2.0.0`

각 범례 아이템 박스의 padding을 지정합니다.

`legend.position = bottom`일 때, 마지막 범례의 우측으로는 `legend.padding`이 적용되지 않습니다. `#2.0.8`

* Type : Number

* Default : 0
