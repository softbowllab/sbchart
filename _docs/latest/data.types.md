---
title:  data.types
date:   2018-05-14
categories: ["latest","data"]
order: 6
---

## data.types

`#2.0.0`

---

범례 별로 차트의 종류를 지정하여 콤바네이션 차트를 구성합니다.

지정되지 않은 범례는 기본으로 라인차트로 처리 됩니다.

* Type : object

  * 데이터 구조는 `범례아이디:차트종류` 형태 입니다.

* Format
```javascript
data: {
	types: {"2015":"line", "2016":"bar", "2016":"spline"}
}
```

* 사용 가능 차트는 다음과 같습니다.

  * 라인(line)
  * 곡선라인(spline)
  * 공간(area)
  * 막대(bar)
  * 버블(bubble)

