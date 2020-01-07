---
title: axis.x.scroll
date: 2019-01-07
categories: ["latest","axis"]
order: 10
---

## axis.x.scroll

`#2.0.20`

---

X축 스크롤 관련 값들을 설정합니다.

X축이 없는 원 계열(원, 도넛, 게이지) 차트와 Radar 차트는 해당되지 않습니다.

* Type : Object

* Format
```javascript
axis: {
	x: {
        scroll: {
            show: true,
            xSize: 2000,
            wheel: true,
        }
	}
}
```

### axis.x.scroll.show

`#2.0.20`

X축 스크롤 표시 여부를 설정합니다.

* Type : Boolean

* Default : false


### axis.x.scroll.xSize

`#2.0.20`

x축의 사이즈를 설정합니다. (스크롤로 표시하고 싶은 실제 차트의 크기)

* Type : Number


### axis.x.scroll.wheel

`#2.0.20`

마우스 휠 스크롤 이동 여부를 설정합니다.

* Type : Boolean

* Default : true
