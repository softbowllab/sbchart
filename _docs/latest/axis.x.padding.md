---
title:  axis.x.padding
date:   2018-05-14
categories: ["latest","axis"]
order: 5
---

## axis.x.padding
---

x축 1번째 값부터 마지막 n번째 값이 위치할 tick의 좌우 padding 값을 정의합니다.

단위는 1개 tick의 너비입니다.
`#2.0.0`

* Type : number/object

* 좌우 모두 동일한 값을 지정


```javascript
axis: {
	x : {
		padding: 2
	}
}
```

## axis.x.padding.left

x축 1번째 tick의 좌측 padding 값을 정의합니다.
`#2.0.0`

* Type : number

* Example

  ```javascript
axis: {
	x : {
		padding:  {
			left: 2,
			right: 2
		}
	}
}
```

## axis.x.padding.right

x축 마지막 tick의 우측 padding 값을 정의합니다.
`#2.0.0`

* Type : number

