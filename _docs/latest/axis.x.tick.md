---
title:  axis.x.tick
date:   2018-05-14
categories: ["latest","axis"]
order: 3
---

## axis.x.tick
---

x축 tick 의 갯수와 라벨 등을 지정한다.
`#2.0.0`

* Type : object

* Format
```javascript
axis: {
	x : {
		tick: {
			format: function(d) { return d + "%"; },
			count: 5,
			fit: false,
			values: [2,4,10]
		}
	}
}
```

### axis.x.tick.format

x축 tick에 display 될 문자/숫자를 정의할 사용자 함수

파라메터로 x축 값을 넘겨받고 tick에 display 될  문자/숫자를 리턴하는 함수를 지정한다.

axis.x.type="timeseries" 인 경우 "%Y/%m/%d" 와 같이 포멧 문자열을 지정할 수 있다.
`#2.0.0`

* Type : any

* 일반적

  ```javascript
axis: {
	x : {
		tick: {
			format: function(d) { return (d*100) + "%"; }
		}
	}
}
```

* axis.x.type="timeseries" 인 경우 아래와 같이 사용 가능

  ```javascript
axis: {
	x : {
		tick: {
			format: "%Y-%m"
		}
	}
}
```

### axis.x.tick.count

x축 display 될 tick 갯수를 지정한다.

2이하의 값은 유효하지 않으므로 3이상의 값을 입력한다.
`#2.0.0`

* Type: number

### axis.x.tick.fit

x축 tick이 알맞게 배치된다.

예를 들어  값이 false는 x 축의 값에 따라 배치되지만, "true" 로 지정한 경우는 보도 nice하게 배치된다.
`#2.0.0`

* Type: boolean

* Default: true


### axis.x.tick.values

x축에서 해당값을 가진 tick 만 나타난다.
`#2.0.0`

* Type: any[]
