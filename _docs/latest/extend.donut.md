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
        label: {
            show: true,
            format: function(value, ratio, id) {
                return (ratio * 100).toFixed(3) + "%";
            }
        },
        innerRadius: 20,
        padding: 0,
        title: "점유율"
    }
}
```

### extend.donut.innerRadius

`#2.0.0`

안쪽 반지름을 지정합니다.

지정하지 않았을 경우는 원의 크기에 따라 자동 계산됩니다.

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


### extend.donut.title

`#2.0.4`

타이틀을 지정합니다.

`title` 옵션과는 구별되어 도넛의 가운데 영역에 표현됩니다.

* Type : string


<!-- ### extend.donut.startAngle

`#2.0.4`

원의 시작 각도를 지정한다.

원의 최상위 값을 기준으로 (값 = 0) 이며 좌측은 -, 우측은 + 값을 갖습니다.

* Type : number

* Default : -180


### extend.donut.endAngle

`#2.0.4`

원의 종료 각도를 지정한다.

원의 최상위 값을 기준으로 (값 = 0) 이며 좌측은 -, 우측은 + 값을 갖습니다.

* Type : number

* Default : 180
 -->
