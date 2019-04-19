---
title: axis.y.tick
date: 2018-05-14
categories: ["latest","axis"]
order: 13
---

## axis.y.tick

`#2.0.0`

---

Y축 Tick의 개수와 라벨 등을 지정합니다.

* Type : Object

* Format
```javascript
axis: {
	y: {
		tick: {
			format: function(d) { return d + "%"; },
			count: 5,
			values: [2, 4, 10],
			outer: true,
			rotate: 0
		}
	}
}
```

### axis.y.tick.format

`#2.0.0`

Y축 Tick에 표시할 문자/숫자를 정의할 사용자 함수입니다.

파라미터로 Y축 값을 넘겨받고 Yick에 표시할 문자/숫자를 리턴하는 함수를 지정합니다.

* Type : Any


### axis.y.tick.count

`#2.0.0`

Y축에 표시할 tick 개수를 지정합니다.

* Type: Number


### axis.y.tick.values

`#2.0.0`

Y축에서 해당 값을 가진 Tick만 나타납니다.

* Type: Any[]

### axis.y.tick.outer

`#2.0.0`

Y축 바깥쪽 Tick 표시 여부를 지정합니다.

* Type: Boolean

* Default: true


### axis.y.tick.rotate

`#2.0.0`

Y축 Tick을 주어진 각도로 회전합니다.

`axis.rotated == true` 일 때(가로 차트)만 허용합니다.

* Type: Number

* Default: 0
