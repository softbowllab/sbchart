---
title:  data.labels
date:   2018-07-24
categories: ["latest","data"]
order: 8
---

## data.labels

_`#2.0.0`_

---

라벨 표시 여부를 지정합니다. 

원계열 차트(원, 도넛) 는 제외되며 `extend.pie.label`, `extend.donut.label` 항목에서 각각 설정할 수 있습니다.

* Type : boolean \ object

* Default : false

* Format

  * boolean Type
```javascript
data : {
    labels: false
}
```

  * object Type
```javascript
data : {
    labels: {
        format: function(value, id, index) {
            return value;
        },
        position: {
            x: 0,
            y: 0
        }
    }
}
```

### data.labels.format

_`#2.0.0`_

라벨을 커스트마이징 합니다.

범례별로 라벨을 다른방식으로 커스트마이징 하고자 한다면 "object Type"을 사용합니다.

* Type : function \ object

* Format

  * function Type
```javascript
data : {
    labels: {
        format: function(value, id, index) {
            return value;
        }
    }
}
```

  * object Type
```javascript
data : {
    labels: {
        format: { 
            data1: function(value, id, index) {
                return value;
            }, 
            data2: function(value, id, index) {
                return value;
            }
        }
    }
}
```

* Function 파라메터

  * value : 값

  * id : 범례 ID (키)

  * index : 그룹 Ibdex (번호)


### data.labels.position

_`#2.0.0`_

라벨의 위치를 조정합니다.

* Type : object

* Format

  ```javascript
data : {
    labels: {
        position: {
            x: 0,
            y: 0
        }
    }
}
```

### data.labels.position.x

_`#2.0.0`_

라벨의 위치를 X축 방향으로 지정된 값 만큼 이동합니다.

(-) 값이면 좌측, (+) 값으면 우측으로 이동합니다.

* Type : number

* Default: 0


### data.labels.position.y

_`#2.0.0`_

라벨의 위치를 Y축 방향으로 지정된 값 만큼 이동합니다.

(-) 값이면 위로, (+) 값으면 아래로 이동합니다.

* Type : number

* Default: 0
