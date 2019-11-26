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
            width: 10,
            point: "circle",
            position: "right"
		}
		onmouseover: function(id) {
			return false;
		},
		onmouseout: function(id) {
			return false;
        },
        onclick: function() {
            return false;
        },
        paddingBottom: 5
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


### legend.item.tile.point

`#2.0.18`

각 범례의 Tile 박스의 모양을 지정합니다.

* Type: String
 
* Default: "rect"

* Values

	* rect: `Default` 사각형

    * circle: 원


### legend.item.tile.position

`#2.0.18`

각 범례의 Tile 박스의 위치를 지정합니다.

* Type : String
 
* Default : "left"

* Values

    * left: `Default` 텍스트의 좌측에 위치

    * right: 텍스트의 우측에 위치


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


### legend.item.onclick

`#2.0.19`

범례 각 항목 클릭 이벤트 핸들러를 지정합니다.

범례 항목 마우스 클릭 시 해당되는 범례의 차트가 제외되는 기본 기능을 사용하지 않는 경우만 사용합니다.

* Type : Function


### legend.item.paddingBottom

`#2.0.10`

범례 각 항목의 하단 padding을 지정합니다.

`legend.position = "inset"`, `legend.position="right"` 일 때 적용되며, 마지막 범례 항목에는 적용되지 않습니다.

* Type : Number
