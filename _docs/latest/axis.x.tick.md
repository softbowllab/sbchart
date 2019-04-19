---
title: axis.x.tick
date: 2018-05-14
categories: ["latest","axis"]
order: 3
---

## axis.x.tick

`#2.0.0`

---

X축 Tick의 개수와 라벨 등을 지정합니다.

* Type : Object

* Format
```javascript
axis: {
	x: {
		tick: {
			count: 5,
			fit: false,
			values: [2, 4, 10],
			outer: true,
			rotate: 0,
			multiline: true,
			centered: false
		}
	}
}
```

### axis.x.tick.count

`#2.0.0`

X축에 표시할 Tick 개수를 지정합니다.

2 이하의 값은 유효하지 않으므로 3 이상의 값을 입력합니다.

* Type: Number


### axis.x.tick.fit

`#2.0.0`

X축 Tick이 알맞게 배치됩니다.

예를 들어 값이 false는 X축의 값에 따라 배치되지만, "true" 로 지정한 경우는 nice하게 배치됩니다.

* Type: Boolean

* Default: true


### axis.x.tick.values

`#2.0.0`

X축에서 해당 값을 가진 Tick만 표시됩니다.

* Type: Any[]


### axis.x.tick.outer

`#2.0.0`

X축 좌우측 끝 부분에 Tick을 표시합니다.

`axis.x.type = "categories"` 인 경우는 X축 마지막 Tick과 동일한 위치에 중복되어 표시됩니다.

* Type: Boolean

* Default: true


### axis.x.tick.rotate

`#2.0.0`

X축 Tick을 주어진 각도로 회전합니다.

* Type: Number

* Default: 0


### axis.x.tick.multiline

`#2.0.0`

X축 Tick의 멀티라인 여부를 허용합니다.

`axis.rotated == false` 일 때(세로 그래프)만 허용합니다.

* Type: Boolean

* Default: true


### axis.x.tick.centered

`#2.0.0`

X축 Tick이 영역의 가운데 위치하도록 합니다.

`axis.x.type == "category"` 인 경우만 유효합니다.

X축의 Tick은 n번째와 n+1번째 영역 구분선에 위치하지만(그리드 선과 동일한 위치) X축 형태가 "카테고리"인 경우는 Tick 위치를 가운데로 변경 가능합니다.

* Type: Boolean

* Default: false


### axis.x.tick.format

`#2.0.0`

X축 Tick에 표시할 문자/숫자를 정의할 사용자 함수를 지정합니다.

파라미터로 X축 값을 넘겨받고 Tick에 표시할 문자/숫자를 리턴하는 함수를 지정합니다.

`axis.x.type = "timeseries"` 인 경우 "%Y/%m/%d" 와 같이 포맷 문자열을 지정할 수 있습니다.

* Type : Any

* Parameter

	* index : Tick 순번입니다. 0부터 시작합니다.

	* value : Tick 값입니다.

		* `axis.x.type = "indexed"` 인 경우는 Tick 순번

		* `axis.x.type = "category"` 인 경우는 카테고리명 

		* `axis.x.type = "timeseries"` 인 경우는 Date 값


* 일반적

	```javascript
axis: {
	x: {
		tick: {
			format: function(index, value) { 
				return index + "번"; 
			}
		}
	}
}
```

* `axis.x.type = "category"` 인 경우 아래와 같이 두 번째 파라미터를 사용할 수 있습니다.

	```javascript
axis: {
	x: {
		tick: {
			format: function(index, value) {
				var m = value.substring(5,7);
				return (index == 0 || m =="01" )? value: m;
			}
		}
	}
}
```

* `axis.x.type = "timeseries"` 인 경우 아래와 같이 사용 가능합니다. 

	* 포맷 Syntax는 [D3.format](https://github.com/d3/d3-3.x-api-reference/blob/master/Time-Formatting.md)을 참조하세요 

	```javascript
axis: {
	x: {
		tick: {
			format: "%Y-%m-%d %H:%M:%S"
		}
	}
}
```
