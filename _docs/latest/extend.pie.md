---
title: extend.pie
date: 2018-07-24
categories: ["latest","extend"]
order: 4
---

## extend.pie

`#2.0.0`

---

원 차트에 대한 확장 옵션을 지정합니다.

* Type : Object

* Format
```javascript
extend: {
	pie: {
		label: {
			show: true,
			format: function(value, ratio, id) {
				return (ratio * 100).toFixed(3) + "%";
			}
		},
		padding: 0,
		fullCircle: true
	}
}
```


### extend.pie.label.show

`#2.0.0`

라벨 표시 여부를 지정합니다.

* Type : Boolean

* Default : true


### extend.pie.label.format

`#2.0.0`

라벨을 커스터마이징 합니다.

* Type : Function

* Format
```javascript
extend: {
	pie: {
		label: {
			format: function(value, ratio, id) {
				return (ratio * 100).toFixed(3) + "%";
			}
		}
	}
}
```

* Function 파라미터

	* value : 값

	* ratio : 계산된 비율 (0 ~ 1)

	* id : 범례 ID


### extend.pie.padding

`#2.0.0`

각 영역(원호) 사이의 여백을 지정합니다.

* Type : Number

* Default : 0


### extend.pie.fullCircle

`#2.0.4`

원 차트의 full circle 여부를 지정합니다.

`extend.pie.fullCircle = false`일 경우 반원으로 표현됩니다.

* Type : Boolean

* Default : true
