---
title:  extend.gauge
date:   2018-10-18
categories: ["latest","extend"]
order: 6
---

## extend.gauge

`#2.0.4`

---

게이지 차트에 대한 확장 옵션를 지정합니다.

* Type : object

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

* Type : number



### extend.gauge.label.show

`#2.0.4`

원의 가운데에 표시되는 값에 대한 라벨의 표시 여부를 지정합니다.

* Type : boolean

* Default : true


### extend.gauge.label.format

`#2.0.4`

원의 가운데에 표시되는 값에 대한 라벨을 커스트마이징 합니다.

* Type : function
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

* Function 파라메터

  * value : 값

  * ratio : 계산된 비율 (0 ~ 1)


<!-- ### extend.gauge.startAngle

`#2.0.4`

원의 시작 각도를 지정한다.

원의 최상위 값을 기준으로 (값 = 0) 이며 좌측은 -, 우측은 + 값을 갖습니다.

* Type : number

* Default : -90


### extend.gauge.endAngle

`#2.0.4`

원의 종료 각도를 지정한다.

원의 최상위 값을 기준으로 (값 = 0) 이며 좌측은 -, 우측은 + 값을 갖습니다.

* Type : number

* Default : 90 -->


### extend.gauge.min

`#2.0.4`

최소값을 지정합니다.

최소값 라벨을 커스트마이징 하려면 object 형태로 지정합니다.

* Type : number / object

* Default : 0

* Format (using object)
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

최소값 라벨을 show/hidden 처리합니다.

* Type : boolean

* Default : true


### extend.gauge.min.value

`#2.0.4`

`extend.gauge.min`를 object 타입으로 지정하는 경우 최소값을 지정합니다.

* Type : number

* Default : 0


### extend.gauge.min.format

`#2.0.4`

최소값 라벨을 커스트마이징 합니다.

* Type : function


### extend.gauge.max

`#2.0.4`

최대값을 지정합니다.

최대값 라벨을 커스트마이징 하려면 object 형태로 지정합니다.

* Type : number / object

* Default : 0

* Format (using object)
```javascript
extend: {
    gauge: {
        max: {
            show: true,
            value: 0,
            format: function(value) {
                return value + " %";
            }
        }
    }
}
```

### extend.gauge.max.show

`#2.0.4`

최대값 라벨을 show/hidden 처리합니다.

* Type : boolean

* Default : true


### extend.gauge.max.value

`#2.0.4`

`extend.gauge.max`를 object 타입으로 지정하는 경우 최대값을 지정합니다.

* Type : number

* Default : 0


### extend.gauge.max.format

`#2.0.4`

최대값 라벨을 커스트마이징 합니다.

* Type : function

### extend.gauge.units

`#2.0.4`

단위 영역에 문자열을 지정합니다.

* Type : string
