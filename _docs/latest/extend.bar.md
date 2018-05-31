---
title:  extend.bar
date:   2018-05-14
categories: ["latest","extend"]
order: 1
---

## extend.bar
---

막대차트의 확장 옵션를 지정합니다. `#2.0.0`

* Type : object

* Format
```javascript
extend: {
	bar: {
		width: {
			ratio: 0.6,
			max: 20
		}
	}
}
```

### extend.bar.width

각 막대의 너비를 지정합니다. `#2.0.0`

* Type : any (number/object)


### extend.bar.width.ratio

각 막대의 너비 비율을 지정합니다. 0 ~ 1 사이의 값을 지정합니다. `#2.0.0`

* Type : number

* Default: 0.6

### extend.bar.width.max

각 막대의 너비 최대값을 지정합니다. 너비 지정된 비율값에 따라 max 값을 넘을 경우는 max 값으로 고정됩니다. `#2.0.0`

* Type : number

