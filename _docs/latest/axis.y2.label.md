---
title: axis.y2.label
date: 2019-09-17
categories: ["latest","axis"]
order: 202
---

## axis.y2.label

`#2.0.17`

---

Y2축 라벨과 위치를 지정합니다.

문자열 또는 Object 타입으로 지정할 수 있습니다. 문자열(String)로 지정한 경우는 해당 문자열이 라벨이 됩니다.

Object 타입으로 지정하면 라벨 및 위치를 조정할 수 있습니다.

* Type : String / Object

* Example
```javascript
axis: {
	y2: {
		label: "변동률(%)"
	}
}
```
또는
```javascript
axis: {
	y2: {
		label: {
			text: "변동률(%)",
			position: "inner-top"
		}
	}
}
```

## axis.y2.label.text

`#2.0.17`

Y2축 라벨을 지정합니다.

* Type : String

* Format
```javascript
axis: {
	y2: {
		label: {
			text: "변동률(%)"
		}
	}
}
```

## axis.y2.label.position

`#2.0.17`

Y2 라벨의 위치를 지정합니다.

* Type : String

* Default : "inner-top" / "inner-right"

* Values (일반)
	* "inner-top": `Default` 축 안쪽 상단
	* "inner-middle": 축 안쪽 중간
	* "inner-bottom": 축 안쪽 하단
	* "outer-top": 축 바깥쪽 상단
	* "outer-middle": 축 바깥쪽 중간
	* "outer-bottom": 축 바깥쪽 하단

* Values (Rotated, `axis.rotated = true` 인 경우)
	* "inner-right": `Default` 축 안쪽 오른쪽
	* "inner-center": 축 안쪽 가운데
	* "inner-left": 축 안쪽 왼쪽
	* "outer-right": 축 바깥쪽 오른쪽
	* "outer-center": 축 바깥쪽 가운데
	* "outer-left": 축 바깥쪽 왼쪽


* Format
```javascript
axis: {
	y2: {
		label: {
			text: "변동률(%)",
			position: "inner-top"
		}
	}
}
```
