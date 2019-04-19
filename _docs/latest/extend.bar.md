---
title: extend.bar
date: 2018-05-14
categories: ["latest","extend"]
order: 2
---

## extend.bar 

 `#2.0.0`

---

막대 차트의 확장 옵션을 지정합니다.

* Type : Object

* Format
```javascript
extend: {
	bar: {
		width: {
			ratio: 0.6,
			max: 20
		},
		zerobased: false
	}
}
```

### extend.bar.width

`#2.0.0`

각 막대의 너비를 지정합니다. 

* Type : Number / Object


### extend.bar.width.ratio

`#2.0.0`

각 막대의 너비 비율을 지정합니다. 0 ~ 1 사이의 값을 지정합니다.

* Type : Number

* Default: 0.6

### extend.bar.width.max

`#2.0.0`

각 막대의 너비 최댓값을 지정합니다. 너비 지정된 비율 값에 따라 max 값을 넘을 경우는 max 값으로 고정됩니다.

* Type : Number


### ~~extend.area.zerobased~~

`#2.0.0` _`deprecated #2.0.3`_ _integrate with `axis.y.zerobased`_

~~값이 모두 양수이거나 모두 음수인 경우 Y축의 최솟값 또는 최대 값이 0으로 설정됩니다.~~

~~모두 양수이면 최솟값(Y축 최하단)이 0으로 모두 음수이면 최댓값(Y축 최상단)이 0이 됩니다.~~

* Type : Boolean

* Default : false
