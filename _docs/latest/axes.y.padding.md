---
title:  axes.y.padding
date:   2018-05-14
categories: ["latest","axes"]
order: 13
---

## axes.y.padding
---

y축 1번째 값부터 마지막 n번째 값이 위치할 tick의 상하 padding 값을 정의한다.

단위는 1개 tick의 높이이다.
`#2.0.0`

* Type : number/object

* 상하 모두 동일한 값을 지정


```javascript
axes: {
	y : {
		padding: 2
	}
}
```

## axes.y.padding.top

y축 1번째 tick의 상단 padding 값을 정의한다.
`#2.0.0`

* Type : number

* Example

  ```javascript
axes: {
	y : {
		padding:  {
			top: 2,
			bottom: 2
		}
	}
}
```

## axes.y.padding.bottom

y축 마지막 tick의 하단 padding 값을 정의한다.
`#2.0.0`

* Type : number

