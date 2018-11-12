---
title:  tooltip
date:   2018-07-24
categories: ["latest","tooltip"]
order: 1
---

## tooltip

`#2.0.0`

---

툴팁에 대한 옵션을 지정합니다.

툴팁은 차트의 값 영역에 마우스 오버하면 나타납니다.

* Type : object

* Format
```javascript
tooltip: {
    show: true,
    grouped: true,
}
```

### tooltip.show

`#2.0.0`

툴팁 표시 여부를 지정합니다.

* Type : boolean

* Default : true


### tooltip.grouped

`#2.0.0`

툴팁이 그룹화되어 같이 표시될지 여부를 지정합니다.

* Type : boolean

* Default : true

* 주의

  * 버블 차트 `data.type = 'bubble'`는 값과 상관없이 항상 `tooltip.grouped = false` 로 동작합니다.
