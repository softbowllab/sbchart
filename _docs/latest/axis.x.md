---
title:  axis.x
date:   2018-05-14
categories: ["latest","axis"]
order: 2
---

## axis.x
---

X축관련 값들을 설정합니다.

X축이 없는 원 계열 차트(원, 도넛) 차트는 해당되지 않습니다.
`#2.0.0`

* Type : object

* Format
```javascript
axis: {
    x : {
        show:false,
        type: "indexed",
        max: 10,
        min: 1,
        height: 20,
        localtime:true
    }
}
```

### axis.x.show

X축 show/hidden 을 지정합니다.
`#2.0.0`

* Type : boolean

* Default : true


### axis.x.type

X축의 형태를 지정합니다.

* Type : string

* Default : "indexed"

* Values
  * "timeseries": X축을 시간순으로 배열합니다.
  * "indexed": `default` x축을 데이터순으로 일정하게 배열합니다.
  * "category": X축 라벨 수동 지정합니다. `axis.x.categories = []` 값도 함께 지졍하셔야 합니다.

### axis.x.min

X축 값 범위의 최소값을 지정합니다.

axis.x.type = "timeseries" 인 경우는 동작하지 않는다.

* Type : number


### axis.x.max

X축 값 범위의 최대값을 지정합니다.

axis.x.type = "timeseries" 인 경우는 동작하지 않는다.

* Type : number

### axis.x.height

X축 영역의 높이를 강제 지정합니다.

* Type : number

### axis.x.localtime

X축 시간대를 처리하는 방법으로 true 인 경우 x 값을 localtime으로 처리, false이면 내부적으로 UTC로 변환합니다.

* Type : boolean

* Default : true

