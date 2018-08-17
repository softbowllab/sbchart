---
title:  grid
date:   2018-05-14
categories: ["latest","grid"]
order: 999
---

## grid

_`#2.0.0`_

---

차트의 그리드를 설정 합니다.

X,Y축이 없는 원 계열 차트(원, 도넛) 차트는 해당되지 않습니다.

* Type : object

* Format
```javascript
grid: {
    x: { 
        show:true
    },
    y: { 
        show:false,
        ticks: 5
    }
}
```


### grid.x.show

_`#2.0.0`_

X축 그리드를 show/hidden 처리합니다.

* Type : boolean

* Default : true

### grid.y.show

_`#2.0.0`_

Y축 그리드를 show/hidden 처리합니다.

* Type : boolean

* Default : true

### grid.y.ticks

_`#2.0.0`_

T축 그리드 Tick 갯수를 지정합니다.

* Type : number
