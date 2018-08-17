---
title:  axis.x.tick
date:   2018-05-14
categories: ["latest","axis"]
order: 3
---

## axis.x.tick

_`#2.0.0`_

---

X축 Tick 의 갯수와 라벨 등을 지정합니다.

* Type : object

* Format
```javascript
axis: {
    x : {
        tick: {
            count: 5,
            fit: false,
            values: [2,4,10],
            outer:true,
            rotate: 0,
            multiline: true,
            centered: false
        }
    }
}
```

### axis.x.tick.count

_`#2.0.0`_

X축에 표시 될 Tick 갯수를 지정합니다.

2이하의 값은 유효하지 않으므로 3이상의 값을 입력합니다.

* Type: number

### axis.x.tick.fit

_`#2.0.0`_

X축 Tick이 알맞게 배치됩니다.

예를 들어  값이 false는 X축의 값에 따라 배치되지만, "true" 로 지정한 경우는 nice하게 배치됩니다.

* Type: boolean

* Default: true


### axis.x.tick.values

_`#2.0.0`_

X축에서 해당값을 가진 Tick 만 표시됩니다.

* Type: any[]


### axis.x.tick.outer

_`#2.0.0`_

X축 좌우측 끝 부분에 Tick을 표시합니다.

`axis.x.type="categories"` 인 경우는 X축 마지막 Tick과 동일한 위치에 중복되어 표시됩니다.

* Type: boolean

* Default: true

### axis.x.tick.rotate

_`#2.0.0`_

X축 Tick을 주어진 각도로 회전합니다.

* Type: number

* Default: 0

### axis.x.tick.multiline

_`#2.0.0`_

X축 Tick의 멀티라인 여부를 허용합니다.

axis.rotated == false 일 때(세로 그래프)만 허용합니다.

* Type: boolean

* Default: true

### axis.x.tick.centered

_`#2.0.0`_

X축 Tick이 영역의 가운데 위치하도록 합니다.

axis.x.type == "category" 인 경우만 유효합니다.

X축의 Tick은 n번째 와 n+1번째 영역 구분선에 위치하지만(그리드 선과 동일한 위치) X축 형태가 "카테고리"인 경우는 Tick 위치를 가운데로 변경 가능합니다.

* Type: boolean

* Default: false

### axis.x.tick.format

_`#2.0.0`_

X축 Tick에 표시 될 문자/숫자를 정의할 사용자 함수를 지정합니다.

파라메터로 X축 값을 넘겨받고 Tick에 표시 될  문자/숫자를 리턴하는 함수를 지정합니다.

axis.x.type="timeseries" 인 경우 "%Y/%m/%d" 와 같이 포멧 문자열을 지정할 수 있습니다.

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
