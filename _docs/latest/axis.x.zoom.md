---
title: axis.x.zoom
date: 2019-01-07
categories: ["latest","axis"]
order: 11
---

## axis.x.zoom

`#2.0.20`

---

X축 줌 관련 값들을 설정합니다.

X축이 없는 원 계열(원, 도넛, 게이지) 차트와 Radar 차트는 해당되지 않습니다.

* Type : Object

* Format
```javascript
axis: {
	x: {
        zoom: {
            type: "drag",
            maxScale: 15,
        }
	}
}
```

### axis.x.zoom.type

`#2.0.20`

zoom type을 설정합니다. (현재 drag 한가지만 설정 가능합니다.)

* Type : Boolean

* Default : "drag"


### axis.x.scroll.maxScale

`#2.0.20`

zoom 배율을 설정합니다. (default : 20)

* Type : Number

* Default : 20
