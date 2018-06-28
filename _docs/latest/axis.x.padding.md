---
title:  axis.x.padding
date:   2018-05-14
categories: ["latest","axis"]
order: 5
---

## axis.x.padding
---

x축의 첫번째 tick 과 마지막 n번째 tick의 좌우 padding 값을 정의합니다.

단위는 1개 tick의 너비입니다.
`#2.0.0`

* Type : number/object

* number형태의 값을 지정할 경우는 첫번째 tick 과 마지막 tick 모두 동일하게 반영됩니다.


```javascript
axis: {
    x : {
        padding: 2
    }
}
```

## axis.x.padding.left

x축 첫번째 tick의 좌측 padding 값을 정의합니다.
`#2.0.0`

* Type : number

* Example

  ```javascript
axis: {
    x : {
        padding:  {
            left: 2
        }
    }
}
```

## axis.x.padding.right

x축 마지막 tick의 우측 padding 값을 정의합니다.
`#2.0.0`

* Type : number

* Example

  ```javascript
axis: {
    x : {
        padding:  {
            right: 2
        }
    }
}
```