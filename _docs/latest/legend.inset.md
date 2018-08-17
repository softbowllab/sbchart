---
title:  legend.inset
date:   2018-05-14
categories: ["latest","legend"]
order: 2
---

## legend.inset

_`#2.0.0`_

---

legend.position="inset" 인 경우 범례의 위치, 형태 등을 지정합니다.

* Type : object

* Format
```javascript
legend: {
    inset: {
        anchor:"top-left",
        x: 10,
        y: 0,
        step: 2
    }
}
```

### legend.inset.anchor

_`#2.0.0`_

legend.position="inset" 인 경우 차트 내에서 범례의 위치를 ​​결정합니다.

* Type : string

* Default : "top-left"

* Values

	* top-left: `default`, 상단 좌측
	* top-right: 상단 우측
	* bottom-left: 하단 좌측
	* bottom-right: 하단 우측

### legend.inset.x

_`#2.0.0`_

legend.position="inset" 인 경우 해당값 만큼 범례의 위치를 X축 방향으로 조정합니다.

* Type : string

* Default : 0

### legend.inset.y

_`#2.0.0`_

legend.position="inset" 인 경우 해당값 만큼 범례의 위치를 Y축 방향으로 조정합니다.

* Type : number

* Default : 0

### legend.inset.step

_`#2.0.0`_

legend.position="inset" 인 경우 범례의 행의 갯수를 정의합니다 

* Type : number

* Default : 1

