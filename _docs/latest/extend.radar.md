---
title: extend.radar
date: 2019-06-07
categories: ["latest","extend"]
order: 8
---

## extend.radar

`#2.0.14`

---

레이더 차트에 대한 확장 옵션을 지정합니다.


* Type : Object

* Format
```javascript
extend: {
	radar: {
		area: false,
		axis: {
			show: false,
			label: false,
			maxValue: 500,
		},
		level: {
			depth: 5,
			label: false,
			format: function(value) {
				return value + '만';
			}
		}
	}
}
```


### extend.radar.area

`#2.0.14`

레이더 차트 내부 영역의 표시 여부를 설정합니다.

* Type : Boolean

* Default : true


### extend.radar.axis.show

`#2.0.14`

레이더 차트 축(axis)의 표시 여부를 설정합니다.

* Type : Boolean

* Default : true


### extend.radar.axis.label

`#2.0.14`

레이더 차트 축(axis)의 가장자리에 나타나는 카테고리 라벨의 표시 여부를 설정합니다.

* Type : Boolean

* Default : true


### extend.radar.axis.maxValue

`#2.0.14`

레이더 차트 축(axis)의 최댓값을 설정합니다.
설정하지 않을 경우 데이터의 최댓값으로 표현됩니다.

* Type : number


### extend.radar.level.depth

`#2.0.14`

레이더 차트에 표시할 레벨의 단계를 설정합니다.
기본값은 5이며, 0으로 설정할 경우 표시되지 않습니다.

* Type : number

* Default : 5


### extend.radar.level.label

`#2.0.14`

레이더 차트 레벨의 라벨 표시 여부를 설정합니다.

* Type : Boolean

* Default : true


### extend.radar.level.format

`#2.0.14`

레이더 차트 레벨의 라벨을 사용자 함수로 설정합니다.

* Type : Function
