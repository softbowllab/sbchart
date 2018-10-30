---
title:  extend.pie
date:   2018-07-24
categories: ["latest","extend"]
order: 4
---

## extend.pie

`#2.0.0`

---

원차트에 대한 확장 옵션를 지정합니다.

* Type : object

* Format
```javascript
extend: {
    pie: {
        label: {
            show: true,
            format: function(value, ratio, id) {
                return (ratio * 100).toFixed(3) + "%";
            }
        },
        padding: 0
    }
}
```


### extend.pie.label.show

`#2.0.0`

라벨 표시 여부를 지정합니다.

* Type : boolean

* Default : true


### extend.pie.label.format

`#2.0.0`

라벨을 커스트마이징 합니다.

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

`#2.0.0`

각 영역(원호) 사이의 공간을 지정합니다.

* Type : number

* Default : 0


<!-- ### extend.pie.startAngle

`#2.0.4`

원의 시작 각도를 지정한다.

원의 최상위 값을 기준으로 (값 = 0) 이며 좌측은 -, 우측은 + 값을 갖습니다.

* Type : number

* Default : -180


### extend.pie.endAngle

`#2.0.4`

원의 종료 각도를 지정한다.

원의 최상위 값을 기준으로 (값 = 0) 이며 좌측은 -, 우측은 + 값을 갖습니다.

* Type : number

* Default : 180 -->

