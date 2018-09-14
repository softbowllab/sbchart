---
title:  axis.x.padding
date:   2018-05-14
categories: ["latest","axis"]
order: 5
---

## axis.x.padding

`#2.0.0`

---

X축의 첫번째 Tick 과 마지막 n번째 Tick의 좌우 padding 값을 정의합니다.

단위는 1개 Tick의 너비입니다.

* Type : number/object

* number형태의 값을 지정할 경우는 첫번째 Tick 과 마지막 Tick 모두 동일하게 반영됩니다.

* Format
```javascript
axis: {
    x : {
        padding: 2
    }
}
```

## axis.x.padding.left

`#2.0.0`

X축 첫번째 Tick의 좌측 padding 값을 정의합니다.

* Type : number

* Format
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

`#2.0.0`

X축 마지막 Tick의 우측 padding 값을 정의합니다.

* Type : number

* Format
```javascript
axis: {
    x : {
        padding:  {
            right: 2
        }
    }
}
```