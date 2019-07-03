---
title: data.x
date: 2019-06-07
categories: ["latest","data"]
order: 10
---

## data.x

`#2.0.14`

---

[data.columns](./data.columns.html)의 첫 번째 행에 X축 카테고리명을 설정할 경우 사용합니다.

data.x의 Value는 [data.columns](./data.columns.html)의 첫 번째 행, 첫 번째 열의 항목과 일치해야 합니다.

<u>axis 옵션을 사용하지 않는 Radar Chart에 필요한 항목입니다.</u>
  
* Type : String

* Format
```javascript
data: {
	x: "x",
	columns: [
		["x", "Category 1", "Category 2", "Category 3", "Category 4", "Category 5", "Category 6"],
		['2015', 90, 40, 50, 120, 80, 90],
		['2016', 120, 160, 200, 160, 130, 220],
		['2017', 300, 240, 290, 230, 300, 320]
	]
}
```

### 주의
* 이 항목을 사용할 경우 [data.columns](./data.columns.html)로 데이터를 설정해야 합니다.
