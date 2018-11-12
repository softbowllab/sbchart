---
title:  extend.bubble
date:   2018-11-02
categories: ["latest","extend"]
order: 1
---

## extend.bubble

`#2.0.6`

---

버블 차트에 대한 확장 옵션를 지정합니다.


* Type : object

* Format
```javascript
extend: {
    bubble: {
        maxR: 40
    }
}
```


### extend.bubble.maxR

`#2.0.6`

버블의 최대 반지름값을 지정합니다.

* Type : number

* Default : 40

### 주의 

* 버블 차트는 각각의 버블의 크기에 따라서 차트 영역을 벗어날 수 있으므로 다음과 같은 방식으로 버블이 잘리지 않도록 하셔야 합니다.

  * X축을 카테고리로 지정 해주는 것이 좋습니다. `axis.x.type='category'`

  * 버블의 최대 반지름값을 낮게 지정합니다. `extend.bubble.maxR = 10`

  * X,Y축에 Padding을 설정합니다.

    * X축
```javascript
    axis: {
        x: {
            type: "indexed",
            padding: 1
        }
    }
```
```javascript
    axis: {
        x: {
            type: "timeseries",
            padding: 1000*60*60*24
        }
    }
```

    * Y축
```javascript
    axis: {
        y: {
            padding: 3
        }
    }
```

  * Y축은 `axis.y.max` 값을 늘려 조정할 수 있습니다.

* 버블 차트는 툴팁이 그룹화되어 표시되지 않습니다. 

  * 항상 `tooltip.grouped = false` 로 동작합니다.
