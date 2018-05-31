---
title:  axes.y.tick
date:   2018-05-14
categories: ["latest","axes"]
order: 13
---

## axes.y.tick
---

y축 tick 의 갯수와 라벨 등을 지정한다.
`#2.0.0`

* Type : object

* Format
```javascript
axes: {
	y : {
		tick: {
			format: function(d) { return d + "%"; },
			count: 5,
			values: [2,4,10]
		}
	}
}
```

### axes.y.tick.format

y축 tick에 display 될 문자/숫자를 정의할 사용자 함수

파라메터로 y축 값을 넘겨받고 tick에 display 될  문자/숫자를 리턴하는 함수를 지정한다.
`#2.0.0`

* Type : any


### axes.y.tick.count

y축 display 될 tick 갯수를 지정한다.
`#2.0.0`

* Type: number


### axes.y.tick.values

y축에서 해당값을 가진 tick 만 나타난다.
`#2.0.0`

* Type: any[]
