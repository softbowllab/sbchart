---
title: data.json
date: 2018-05-14
categories: ["latest","data"]
order: 3
---

## data.json

`#2.0.0`

---

JSON 배열 형태로 차트 데이터를 지정하는 방식입니다.

배열 내 JSON 객체는 하나의 범례를 의미합니다.

**반드시** x축 열과 y축 값으로 쓰일 속성들을 [data.keys](/data/data.keys.html)로 지정해야 합니다.

data.keys.value 에 지정된 값들이 범례 아이디가 됩니다.

* Type : Object[]

* Format
```javascript
data: {
	json: [
		{"name": "seoul", "2015": 90, "2016": 120, "2017": 300},
		{"name": "busan", "2015": 40, "2016": 160, "2017": 240},
		{"name": "daegu", "2015": 50, "2016": 200, "2017": 290},
		{"name": "kwangju", "2015": 120, "2016": 160, "2017": 230},
		{"name": "sejong", "2015": 80, "2016": 130, "2017": 300},
		{"name": "incheon", "2015": 90, "2016": 220, "2017": 320}
	],
	keys: {
		x: "name",
		value: ["2015", "2016", "2017"]
	}
}
```
