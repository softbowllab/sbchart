---
title:  axis.y
date:   2018-05-14
categories: ["latest","axis"]
order: 11
---

## axis.y

_`#2.0.0`_

---

Y축 관련 값들을 설정합니다.

Y축이 없는 원 계열 차트(원, 도넛) 차트는 해당되지 않습니다.

* Type : object

* Format
```javascript
axis: {
    y : {
        show:false,
        min: 0,
        max: 100,
        center: 50
    }
}
```

### axis.y.show

_`#2.0.0`_

Y축의 show/hidden 을 지정합니다.

* Type : boolean

* Default : true

### axis.y.min

_`#2.0.0`_

Y축의 최소값을 지정한다.

이 값을 기준으로 Y축의 bottom padding이 자동으로 추가되므로 필요 없을 경우 `axis.y.padding = 0` 으로 지정합니다.

* Type : number

### axis.y.max

_`#2.0.0`_

Y축의 최대값을 지정한다.

이 값을 기준으로 Y축의 top padding이 자동으로 추가되므로 필요 없을 경우 `axis.y.padding = 0` 으로 지정합니다.

* Type : number

### axis.y.center

_`#2.0.0`_

y축 값의 중간값을 지정합니다.

* Type : number

