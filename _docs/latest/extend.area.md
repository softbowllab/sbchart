---
title: extend.area
date: 2018-06-15
categories: ["latest","extend"]
order: 3
---

## ~~extend.area~~ 

`#2.0.0` _`deprecated #2.0.3`_

---

~~영역차트에 대한 확장 옵션을 지정합니다.~~

* Type : Object

* Format
```javascript
extend: {
	area: {
		zerobased: false
	}
}
```

### ~~extend.area.zerobased~~

`#2.0.0` _`deprecated #2.0.3`_ _integrate with `axis.y.zerobased`_

~~값이 모두 양수이거나 모두 음수인 경우 Y축의 최솟값 또는 최댓값이 0으로 설정됩니다.~~

~~모두 양수이면 최솟값(Y축 최하단)이 0으로 모두 음수이면 최댓값(Y축 최상단)이 0이 됩니다.~~

* Type : Boolean

* Default : false
