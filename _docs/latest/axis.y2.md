---
title: axis.y2
date: 2019-09-17
categories: ["latest","axis"]
order: 200
---

## axis.y2

`#2.0.17`

---

Y2축 관련 값들을 설정합니다.

Y2축이 없는 원 계열 차트(원, 도넛, 게이지, 레이더) 차트는 해당되지 않습니다.

* Type : Object

* Format
```javascript
axis: {
	y2: {
		show: false,
		min: 0,
		max: 100,
		center: 50,
		zerobased: false,
        domain: {
            show: false
        }
	}
}
```

### axis.y2.show

`#2.0.17`

Y2축의 show/hide를 지정합니다.

* Type : Boolean

* Default : true

### axis.y2.min

`#2.0.17`

Y2축의 최솟값을 지정합니다.

이 값을 기준으로 Y2축의 bottom padding이 자동으로 추가되므로 필요 없을 경우 `axis.y2.padding = 0`으로 지정합니다.

* Type : Number

### axis.y2.max

`#2.0.17`

Y2축의 최댓값을 지정합니다.

이 값을 기준으로 Y2축의 top padding이 자동으로 추가되므로 필요 없을 경우 `axis.y2.padding = 0`으로 지정합니다.

* Type : Number

### axis.y2.center

`#2.0.17`

y2축 값의 중간값을 지정합니다.

* Type : Number


### axis.y2.zerobased

`#2.0.17`

값이 모두 양수이거나 모두 음수인 경우 Y2축의 최솟값 또는 최댓값이 0으로 설정됩니다.

모두 양수이면 최솟값(Y2축 최하단)이 0으로 모두 음수이면 최댓값(Y2축 최상단)이 0이 됩니다.

* Type : Boolean

* Default : true


### axis.y2.domain.show

`#2.0.21`

Y2축 Domain(Y2축 라인)의 노출 여부를 설정합니다.

* Type : Boolean

* Default : true
