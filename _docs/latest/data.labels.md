---
title: data.labels
date: 2018-07-24
categories: ["latest","data"]
order: 9
---

## data.labels

`#2.0.0`

---

라벨 표시 여부를 지정합니다. 

원계열 차트(원, 도넛, 게이지)는 제외되며 `extend.pie.label`, `extend.donut.label`, `extend.gauge.label` 항목에서 각각 설정할 수 있습니다.

* Type : Boolean / Object

* Default : false

* Format

	* Boolean Type
```javascript
data: {
	labels: false
}
```

	* Object Type
```javascript
data: {
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

`#2.0.0`

라벨을 커스터마이징 합니다.

범례 별로 라벨을 다른 방식으로 커스터마이징 하고자 한다면 "Object Type"을 사용합니다.

* Type : Function \ Object

* Format

	* Function Type
```javascript
data: {
	labels: {
			format: function(value, id, index) {
				return value;
			}
	}
}
```

	* Object Type
```javascript
data: {
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

* Function 파라미터

	* value : 값

	* id : 범례 아이디

	* index : 그룹 Index (번호)


### data.labels.position

`#2.0.0`

라벨의 위치를 조정합니다.

* Type : Object

* Format
```javascript
data: {
	labels: {
		position: {
			x: 0,
			y: 0
		}
	}
}
```

### data.labels.position.x

`#2.0.0`

라벨의 위치를 X축 방향으로 지정된 값만큼 이동합니다.

(-) 값이면 좌측, (+) 값이면 우측으로 이동합니다.

* Type : Number

* Default: 0


### data.labels.position.y

`#2.0.0`

라벨의 위치를 Y축 방향으로 지정된 값만큼 이동합니다.

(-) 값이면 위로, (+) 값이면 아래로 이동합니다.

* Type : Number

* Default: 0
