---
title:  axis.y.label
date:   2018-05-14
categories: ["latest","axis"]
order: 13
---

## axis.y.label

`#2.0.0`

---

Y축 라벨과 위치를 지정합니다.

문자열 또는 Object 타입으로 지정할 수 있습니다. 문자열(string)로 지정한 경우는 해당문자열이 라벨이 됩니다.

Object 타입으로 지정하면 라벨 및 위치를 조정할 수 있습니다.

* Type : string/object

* Example

  ```javascript
axis: {
    y : {
        label: "지역별"
    }
}
```
또는

  ```javascript
axis: {
    y : {
        label:  {
            text: "변동률(%)",
            position: "inner-top"
        }
    }
}
```

## axis.y.label.text

_`#2.0.0`_

Y축 라벨을 지정합니다.

* Type : string

* Format
```javascript
axis: {
    y : {
        label:  {
            text: "변동률(%)"
        }
    }
}
```

## axis.y.label.position

_`#2.0.0`_

Y축 라벨의 위치를 지정합니다.

* Type : string

* Values (일반)
  * "inner-top": 축 안쪽 상단
  * "inner-middle": 축 안쪽 중간
  * "inner-bottom": 축 안쪽 하단
  * "outer-top": 축 바깥쪽 상단
  * "outer-middle": 축 바깥쪽 중간
  * "outer-bottom": 축 바깥쪽 하단

* Values (Rotated)
  * "inner-right":  축 안쪽 오른쪽
  * "inner-center": 축 안쪽 가운데
  * "inner-left":  축 안쪽 왼쪽
  * "outer-right":  축 바깥쪽 오른쪽
  * "outer-center":  축 바깥쪽 가운데
  * "outer-left":축 바깥쪽 왼쪽

* Default : "inner-top"

* Format
```javascript
axis: {
    y : {
        label:  {
            text: "변동률(%)",
            position: "inner-top"
        }
    }
}
```
