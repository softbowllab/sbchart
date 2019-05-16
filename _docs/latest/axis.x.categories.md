---
title: axis.x.categories
date: 2018-05-14
categories: ["latest","axis"]
order: 3
---

## axis.x.categories

`#2.0.0`

---

X축 카테고리명을 지정합니다.

`axis.x.type = "category"` 혹은 `axis.x.type = "timeseries"` 로 지정되어 있어야 합니다.

`axis.x.type = "timeseries"` 일 때는 날짜 형식(yyyy-MM-dd)으로 입력해야 합니다.

* Type : String[]

* Format
```javascript
axis: {
	x: {
		type: "category",
		categories: ["전국", "서울", "부산", "대구", "인천", "광주", "대전", "울산", "세종", "경기", "강원", "충북", "충남", "전북", "전남", "경북", "경남", "제주"]
		// or 
		type: "timeseries",
		categories: ["2019-01-01", "2019-02-01", "2019-03-01", "2019-04-01", "2019-05-01"]
	}
}
```
