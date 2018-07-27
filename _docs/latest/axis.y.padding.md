---
title:  axis.y.padding
date:   2018-05-14
categories: ["latest","axis"]
order: 14
---

## axis.y.padding
---

Y축 1번째 값부터 마지막 n번째 값이 위치할 Tick의 상하 padding 값을 정의합니다.

단위는 1개 Tick의 높이입니다.
`#2.0.0`

* Type : number/object

* 상하 모두 동일한 값을 지정합니다.

* Format
```javascript
axis: {
    y : {
        padding: 2
    }
}
```

## axis.y.padding.top

Y축 1번째 Tick의 상단 padding 값을 정의합니다.
`#2.0.0`

* Type : number

* Format
```javascript
axis: {
    y : {
        padding:  {
            top: 2,
            bottom: 2
        }
    }
}
```

## axis.y.padding.bottom

Y축 마지막 Tick의 하단 padding 값을 정의합니다.
`#2.0.0`

* Type : number

