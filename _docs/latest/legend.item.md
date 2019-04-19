---
title: legend.item
date: 2018-05-14
categories: ["latest","legend"]
order: 2
---

## legend.item

`#2.0.0`

---

각 범례의 세부 사항을 정의합니다.

* Type : Object

* Format
```javascript
legend: {
	item: {
		tile: {
			height: 10,
			width: 10
		}
		mouseover: function(id) {
			return false;
		},
		mouseout: function(id) {
			return false;
		}
	}
}
```

### legend.item.tile.height

`#2.0.0`

각 범례의 Tile 박스의 높이를 지정합니다.

* Type : Number

* Default : 10


### legend.item.tile.width

`#2.0.0`

각 범례의 Tile 박스의 너비를 지정합니다.

* Type : Number

* Default : 10

### legend.item.onmouseover

`#2.0.3`

범례 각 항목 마우스 오버 이벤트 핸들러를 지정합니다.

현재는 범례 항목 마우스 오버 시 해당되는 차트 내 데이터 표현 부분을 highlight 하는 기본 기능을 사용하지 않는 경우만 사용합니다.

* Type : Function


### legend.item.onmouseout

`#2.0.3`

범례 각 항목 마우스 아웃 이벤트 핸들러를 지정합니다.

현재는 범례 항목 마우스 아웃 시 해당되는 차트 내 데이터 표현 부분을 highlight 하는 기본 기능을 사용하지 않는 경우만 사용합니다.

* Type : Function
