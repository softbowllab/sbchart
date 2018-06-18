---
title:  axis.y.tick
date:   2018-05-14
categories: ["latest","axis"]
order: 13
---

## axis.y.tick
---

y축 tick 의 갯수와 라벨 등을 지정합니다.
`#2.0.0`

* Type : object

* Format
```javascript
axis: {
	y : {
		tick: {
			format: function(d) { return d + "%"; },
			count: 5,
			values: [2,4,10],
			outer: true,
			rotate: 0
		}
	}
}
```

### axis.y.tick.format

y축 tick에 display 될 문자/숫자를 정의할 사용자 함수입니다.

파라메터로 y축 값을 넘겨받고 tick에 display 될  문자/숫자를 리턴하는 함수를 지정합니다.
`#2.0.0`

* Type : any


### axis.y.tick.count

y축 display 될 tick 갯수를 지정합니다.
`#2.0.0`

* Type: number


### axis.y.tick.values

y축에서 해당값을 가진 tick 만 나타납니다.
`#2.0.0`

* Type: any[]

### axis.y.tick.outer

y축 바깥쪽 tick display 여부를 지정합니다.
`#2.0.0`

* Type: boolean

* Default: true


### axis.y.tick.outer

y축 바깥쪽 tick display 여부를 지정합니다.
`#2.0.0`

* Type: boolean

* Default: true

### axis.y.tick.rotate

y축 tick을 주어진 각도로 회전합니다.
`#2.0.0`

* Type: number

* Default: 0
