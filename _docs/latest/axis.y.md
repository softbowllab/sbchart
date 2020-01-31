---
title: axis.y
date: 2018-05-14
categories: ["latest","axis"]
order: 101
---

## axis.y

`#2.0.0`

---

Y축 관련 값들을 설정합니다.

Y축이 없는 원 계열 차트(원, 도넛, 게이지) 차트는 해당되지 않습니다.

* Type : Object

* Format
```javascript
axis: {
	y: {
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

### axis.y.show

`#2.0.0`

Y축의 show/hide를 지정합니다.

* Type : Boolean

* Default : true

### axis.y.min

`#2.0.0`

Y축의 최솟값을 지정합니다.

이 값을 기준으로 Y축의 bottom padding이 자동으로 추가되므로 필요 없을 경우 `axis.y.padding = 0`으로 지정합니다.

* Type : Number

### axis.y.max

`#2.0.0`

Y축의 최댓값을 지정합니다.

이 값을 기준으로 Y축의 top padding이 자동으로 추가되므로 필요 없을 경우 `axis.y.padding = 0`으로 지정합니다.

* Type : Number

### axis.y.center

`#2.0.0`

y축 값의 중간값을 지정합니다.

* Type : Number


### axis.y.zerobased

`#2.0.3`

값이 모두 양수이거나 모두 음수인 경우 Y축의 최솟값 또는 최댓값이 0으로 설정됩니다.

모두 양수이면 최솟값(Y축 최하단)이 0으로 모두 음수이면 최댓값(Y축 최상단)이 0이 됩니다.

* Type : Boolean

* Default : true


### axis.y.domain.show

`#2.0.21`

Y축 Domain(Y축 라인)의 노출 여부를 설정합니다.

* Type : Boolean

* Default : true
