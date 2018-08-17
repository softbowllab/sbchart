---
title:  extend.area
date:   2018-06-15
categories: ["latest","extend"]
order: 3
---

## ~~extend.area~~ 

_`#2.0.0`_ _`deprecated`_

---

영역차트에 대한 확장 옵션를 지정합니다. 

* Type : object

* Format
```javascript
extend: {
    area: {
        zerobased: false
    }
}
```

### ~~extend.area.zerobased~~

_`#2.0.0`_ _`deprecated`_

값이 모두 양수이거나 모두 음수인 경우 Y축의 최소값 또는 최대 값이 0으로 설정됩니다.

모두 양수이면 최소값(Y축 최하단)이 0으로 모두 음수이면 최대값(Y축 최상단)이 0이 됩니다. 

* Type : boolean

* Default : false
