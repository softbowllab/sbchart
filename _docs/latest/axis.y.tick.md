---
title:  axis.y.tick
date:   2018-05-14
categories: ["latest","axis"]
order: 13
---

## axis.y.tick
---

Y축 Tick 의 갯수와 라벨 등을 지정합니다.
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

Y축 Tick에 표시 될 문자/숫자를 정의할 사용자 함수입니다.

파라메터로 Y축 값을 넘겨받고 Yick에 표시 될 문자/숫자를 리턴하는 함수를 지정합니다.
`#2.0.0`

* Type : any


### axis.y.tick.count

Y축에 표시 될 tick 갯수를 지정합니다.
`#2.0.0`

* Type: number


### axis.y.tick.values

Y축에서 해당값을 가진 Tick 만 나타납니다.
`#2.0.0`

* Type: any[]

### axis.y.tick.outer

Y축 바깥쪽 Tick 표시 여부를 지정합니다.
`#2.0.0`

* Type: boolean

* Default: true


### axis.y.tick.outer

Y축 바깥쪽 Tick 표시 여부를 지정합니다.
`#2.0.0`

* Type: boolean

* Default: true

### axis.y.tick.rotate

Y축 Tick을 주어진 각도로 회전합니다.
`#2.0.0`

* Type: number

* Default: 0
