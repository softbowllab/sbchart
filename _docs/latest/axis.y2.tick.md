---
title: axis.y2.tick
date: 2019-09-17
categories: ["latest","axis"]
order: 201
---

## axis.y2.tick

`#2.0.17`

---

Y2축 Tick의 개수와 라벨 등을 지정합니다.

* Type : Object

* Format
```javascript
axis: {
	y2: {
		tick: {
			format: function(d) { return d + "%"; },
			count: 5,
			values: [2, 4, 10],
			outer: true,
			rotate: 0,
            culling: {
                max: 5
            },
            line: {
                show: false
            },
            text: {
                show: false
            }
		}
	}
}
```

### axis.y2.tick.format

`#2.0.17`

Y2축 Tick에 표시할 문자/숫자를 정의할 사용자 함수입니다.

파라미터로 Y2축 값을 넘겨받고 Yick에 표시할 문자/숫자를 리턴하는 함수를 지정합니다.

* Type : Any


### axis.y2.tick.count

`#2.0.17`

Y2축에 표시할 Tick의 개수를 지정합니다.

* Type: Number


### axis.y2.tick.values

`#2.0.17`

Y2축에서 해당 값을 가진 Tick만 나타납니다.

* Type: Any[]

### axis.y2.tick.outer

`#2.0.17`

Y2축 바깥쪽 Tick 표시 여부를 지정합니다.

* Type: Boolean

* Default: true


### axis.y2.tick.rotate

`#2.0.17`

Y2축 Tick을 주어진 각도로 회전합니다.

`axis.rotated == true` 일 때(가로 차트)만 허용합니다.

* Type: Number

* Default: 0


### axis.y2.tick.culling.max

`#2.0.21`

Y2축 Tick의 Text의 max값을 지정할 수 있습니다. (max값이기 때문에 지정한 수보다 적게 나올 수 있습니다.)

* Type: Number


### axis.y2.tick.line.show

`#2.0.21`

Y2축 Tick의 Line의 노출 여부를 설정합니다.

* Type: Boolean

* Default : true


### axis.y2.tick.text.show

`#2.0.21`

Y2축 Tick의 Text의 노출 여부를 설정합니다.

* Type: Boolean

* Default : true
