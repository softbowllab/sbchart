---
title:  legend
date:   2018-05-14
categories: ["latest","legend"]
order: 1
---

## legend

`#2.0.0`

---

범례 위치, 형태 등을 지정합니다.

* Type : object

* Format
```javascript
legend: {
    show: true,
    position: "inset",
    inset: {
        anchor:"top-left",
        x: 10,
        y: 0
    },
    padding: 10
}
```

### legend.show

`#2.0.0`

범례의 show/hidden 여부를 지정합니다.

* Type : boolean

* Default : false

### legend.position

`#2.0.0`

범례의 위치를 지정합니다.

* Type : string

* Default : "botom"

* Values

	* bottom: `Default` 아래에 위치
	* right: 우측에 위치
	* inset: 차트내에 위치, 사항한 사항은 [legend.inset](./legend.inset.html) 참조

### legend.padding

`#2.0.0`

각 범례 아이템 박스의 padding 을 지정합니다.

* Type : number

* Default : 0

