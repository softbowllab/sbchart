---
title: extend.gauge
date: 2018-10-18
categories: ["latest","extend"]
order: 6
---

## extend.gauge

`#2.0.4`

---

게이지 차트에 대한 확장 옵션을 지정합니다.

* Type : Object

* Format
```javascript
extend: {
	gauge: {
		label: {
			show: true,
			format: function(value, ratio) {
				return (value / 100).toFixed(3);
			}
		},
		innerRadius: 20,
		fullCircle: false,
		min: 0,
		max: 100,
		units: "%"
	}
}
```

### extend.gauge.innerRadius

`#2.0.4`

안쪽 반지름을 지정합니다.

지정하지 않았을 경우는 원의 크기에 따라 자동 계산됩니다.

* Type : Number



### extend.gauge.label.show

`#2.0.4`

게이지의 가운데에 표시되는 값에 대한 라벨의 표시 여부를 지정합니다.

* Type : Boolean

* Default : true


### extend.gauge.label.format

`#2.0.4`

게이지의 가운데에 표시되는 값에 대한 라벨을 커스터마이징 합니다.

* Type : Function

* Format
```javascript
extend: {
	gauge: {
		label: {
			format: function(value, ratio) {
				return (ratio / 100).toFixed(3);
			}
		}
	}
}
```

* Function 파라미터

	* value : 값

	* ratio : 계산된 비율 (0 ~ 1)

### extend.gauge.fullCircle

`#2.0.4`

full circle 여부를 지정합니다.

`extend.gauge.fullCircle = true`일 경우 원으로 표현됩니다.

* Type : Boolean

* Default : false


### extend.gauge.min

`#2.0.4`

최솟값을 지정합니다.

최솟값 라벨을 커스터마이징 하려면 Object 형태로 지정합니다.

* Type : Number / Object

* Default : 0

* Format (using Object)
```javascript
extend: {
	gauge: {
		min: {
			show: true,
			value: 0,
			format: function(value) {
				return value + " %";
			}
		}
	}
}
```

### extend.gauge.min.show

`#2.0.4`

최솟값 라벨을 show/hide 처리합니다.

* Type : Boolean

* Default : true


### extend.gauge.min.value

`#2.0.4`

`extend.gauge.min`를 Object 타입으로 지정하는 경우 최솟값을 지정합니다.

* Type : Number

* Default : 0


### extend.gauge.min.format

`#2.0.4`

최솟값 라벨을 커스터마이징 합니다.

* Type : Function


### extend.gauge.max

`#2.0.4`

최댓값을 지정합니다.

최댓값 라벨을 커스터마이징 하려면 Object 형태로 지정합니다.

* Type : Number / Object

* Default : 100

* Format (using Object)
```javascript
extend: {
	gauge: {
		max: {
			show: true,
			value: 100,
			format: function(value) {
				return value + " %";
			}
		}
	}
}
```

### extend.gauge.max.show

`#2.0.4`

최댓값 라벨을 show/hide 처리합니다.

* Type : Boolean

* Default : true


### extend.gauge.max.value

`#2.0.4`

`extend.gauge.max`를 Object 타입으로 지정하는 경우 최댓값을 지정합니다.

* Type : Number

* Default : 100


### extend.gauge.max.format

`#2.0.4`

최댓값 라벨을 커스터마이징 합니다.

* Type : Function

### extend.gauge.units

`#2.0.4`

단위 영역에 문자열을 지정합니다.

* Type : String
