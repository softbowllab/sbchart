---
title:  extend.pie
date:   2018-07-24
categories: ["latest","extend"]
order: 4
---

## extend.pie
---

원차트에 대한 확장 옵션를 지정합니다. `#2.0.0`

* Type : object


### extend.pie.label.show

라벨 표시 여부를 지정합니다.
`#2.0.0`

* Type : boolean

* Default : true

* Format
```javascript
extend: {
    pie: {
        label: {
            show: true
        }
    }
}
```


### extend.pie.label.format

라벨을 커스트마이징 합니다.
`#2.0.0`

* Type : function
```javascript
extend: {
    pie: {
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


### extend.pie.padding

각 영역(원호) 사이의 공간을 지정합니다.
`#2.0.0`

* Type : number

* Default : 0

* Format
```javascript
extend: {
    pie: {
        padding: 0
    }
}
```
