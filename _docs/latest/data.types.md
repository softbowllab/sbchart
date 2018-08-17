---
title:  data.types
date:   2018-05-14
categories: ["latest","data"]
order: 6
---

## data.types

_`#2.0.0`_

---

범례 별로 차트의 종류를 지정하여 콤바네이션 차트를 구성합니다.

**라인차트(line)**,**곡선라인차트(spline)**,**공간차트(area)**, **막대차트(bar)** 만 가능합니다.

지정되지 않은 범례는 기본으로 라인차트로 처리 됩니다.

* Type : string[]

* Format
```javascript
data: {types: ["line", "bar"]}
```
