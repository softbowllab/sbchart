---
title:  extend.donut
date:   2018-07-24
categories: ["latest","extend"]
order: 5
---

## extend.donut

`#2.0.0`

---

도넛 차트에 대한 확장 옵션를 지정합니다.

* Type : object

* Format
```javascript
extend: {
    donut: {
		padding: 0,
        label: {
            show: true,
            format: function(value, ratio, id) {
                return (ratio * 100).toFixed(3) + "%";
            }
        },
        innerRadius: 0,
        padding: 0
    }
}
```

### extend.donut.innerRadius

`#2.0.0`

안쪽 반지름을 지정합니다.

지정하지 않았을 경우는 원의크기에 따라 자동 계산됩니다.

* Type : number


### extend.donut.padding

`#2.0.0`

각 영역(원호) 사이의 공간을 지정합니다.

* Type : number

* Default : 0


### extend.donut.label.show

`#2.0.0`

라벨 표시 여부를 지정합니다.

* Type : boolean

* Default : true


### extend.donut.label.format

`#2.0.0`

라벨을 커스트마이징 합니다.

* Type : function
```javascript
extend: {
    donut: {
        label: {
            format: function(value, ratio, id) {
                return (ratio * 100).toFixed(3) + "%";
            }
        }
    }
}
```

* Function 파라메터

  * value : 값

  * ratio : 계산된 비율 (0 ~ 1)

  * id : 범례 ID



