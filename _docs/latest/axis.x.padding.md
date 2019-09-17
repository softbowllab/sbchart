---
title: axis.x.padding
date: 2018-05-14
categories: ["latest","axis"]
order: 9
---

## axis.x.padding

`#2.0.0`

---

X축의 첫 번째 Tick과 마지막 n번째 Tick의 좌우 padding 값을 정의합니다.

단위는 1개 Tick의 너비입니다.

단, `axis.x.type = "timeseries"`인 경우 시간 단위로 입력해야 합니다.

* Type : Number / Object

* Number형태의 값을 지정할 경우는 첫 번째 Tick과 마지막 Tick 모두 동일하게 반영됩니다.

* Format
```javascript
axis: {
	x: {
		padding: 2
		// or
		padding: 1000*60*60*24*1
	}
}
```
* 주의 
	* `axis.x.type = "indexed" or "timeseries"`인 경우 좌우 기본 padding이 적용되어 있어 0을 입력하면 좌우 여백이 사라집니다.


## axis.x.padding.left

`#2.0.0`

X축 첫 번째 Tick의 좌측 padding 값을 정의합니다.

* Type : Number

* Format
```javascript
axis: {
	x: {
		padding: {
			left: 2
			// or
			left: 1000*60*60*24*1
		}
	}
}
```

## axis.x.padding.right

`#2.0.0`

X축 마지막 Tick의 우측 padding 값을 정의합니다.

* Type : Number

* Format
```javascript
axis: {
	x: {
		padding: {
			right: 2
			// or
			right: 1000*60*60*24*2
		}
	}
}
```
