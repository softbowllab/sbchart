---
title:  extend.bar
date:   2018-05-14
categories: ["latest","extend"]
order: 2
---

## extend.bar
---

막대차트의 확장 옵션를 지정합니다. `#2.0.0`

* Type : object

* Format
```javascript
extend: {
    bar: {
        width: {
            ratio: 0.6,
            max: 20
        },
        zerobased: false
    }
}
```

### extend.bar.width

각 막대의 너비를 지정합니다. `#2.0.0`

* Type : any (number/object)


### extend.bar.width.ratio

각 막대의 너비 비율을 지정합니다. 0 ~ 1 사이의 값을 지정합니다. `#2.0.0`

* Type : number

* Default: 0.6

### extend.bar.width.max

각 막대의 너비 최대값을 지정합니다. 너비 지정된 비율값에 따라 max 값을 넘을 경우는 max 값으로 고정됩니다. `#2.0.0`

* Type : number


### extend.area.zerobased

값이 모두 양수이거나 모두 음수인 경우 Y축의 최소값 또는 최대 값이 0으로 설정됩니다.

모두 양수이면 최소값(Y축 최하단)이 0으로 모두 음수이면 최대값(Y축 최상단)이 0이 됩니다. `#2.0.0`

* Type : boolean

* Default : false
