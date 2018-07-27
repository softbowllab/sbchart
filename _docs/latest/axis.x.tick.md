---
title:  axis.x.tick
date:   2018-05-14
categories: ["latest","axis"]
order: 3
---

## axis.x.tick
---

X축 Tick 의 갯수와 라벨 등을 지정합니다.
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
            values: [2,4,10],
            outer:true,
            rotate: 0,
            multiline: true
        }
    }
}
```

### axis.x.tick.format

X축 Tick에 표시 될 문자/숫자를 정의할 사용자 함수를 지정합니다.

파라메터로 X축 값을 넘겨받고 Tick에 표시 될  문자/숫자를 리턴하는 함수를 지정합니다.

axis.x.type="timeseries" 인 경우 "%Y/%m/%d" 와 같이 포멧 문자열을 지정할 수 있습니다.
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

* axis.x.type="timeseries" 인 경우 아래와 같이 사용 가능합니다.

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

X축에 표시 될 Tick 갯수를 지정합니다.

2이하의 값은 유효하지 않으므로 3이상의 값을 입력합니다.
`#2.0.0`

* Type: number

### axis.x.tick.fit

X축 Tick이 알맞게 배치됩니다.

예를 들어  값이 false는 X축의 값에 따라 배치되지만, "true" 로 지정한 경우는 nice하게 배치됩니다.
`#2.0.0`

* Type: boolean

* Default: true


### axis.x.tick.values

X축에서 해당값을 가진 Tick 만 표시됩니다.
`#2.0.0`

* Type: any[]


### axis.x.tick.outer

X축 바깥쪽 Tick의 표시 여부를 지정합니다.
`#2.0.0`

* Type: boolean

* Default: true

### axis.x.tick.rotate

X축 Tick을 주어진 각도로 회전합니다.
`#2.0.0`

* Type: number

* Default: 0

### axis.x.tick.multiline

X축 Tick의 멀티라인 여부를 허용합니다.

axis.rotated == false 일 때(세로 그래프)만 허용합니다.
`#2.0.0`

* Type: boolean

* Default: true
