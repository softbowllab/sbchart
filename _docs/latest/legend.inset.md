---
title: legend.inset
date: 2018-05-14
categories: ["latest","legend"]
order: 2
---

## legend.inset

`#2.0.0`

---

`legend.position = "inset"` 인 경우 범례의 위치, 형태 등을 지정합니다.

* Type : Object

* Format
```javascript
legend: {
	inset: {
		anchor: "top-left",
		x: 10,
		y: 0,
		step: 2
	}
}
```

### legend.inset.anchor

`#2.0.0`

`legend.position = "inset"` 인 경우 차트 내에서 범례의 위치를 ​​결정합니다.

* Type : String

* Default : "top-left"

* Values

	* top-left: `Default`, 상단 좌측
	* top-right: 상단 우측
	* bottom-left: 하단 좌측
	* bottom-right: 하단 우측

### legend.inset.x

`#2.0.0`

`legend.position = "inset"` 인 경우 해당 값만큼 범례의 위치를 X축 방향으로 조정합니다.

* Type : Number

* Default : 10

### legend.inset.y

`#2.0.0`

`legend.position = "inset"` 인 경우 해당 값만큼 범례의 위치를 Y축 방향으로 조정합니다.

* Type : Number

* Default : 0

### legend.inset.step

`#2.0.0`

`legend.position = "inset"` 인 경우 범례의 행의 개수를 정의합니다 

* Type : Number
