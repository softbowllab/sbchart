---
title:  data.groups
date:   2018-09-14
categories: ["latest","data"]
order: 7
---

## data.groups

`#2.0.3`

---

Stacked bar 차트에서 묶어서 보여줄 범례를 지정합니다.

그룹별로 범례 아이디들을 2차원 배열로 지정합니다.

범례 아이디가 일치 하지 않을 경우는 지정된 값은 무시되며 값이 지정하지 않았을 경우는 모든 범례를 하나로 묶어 보여줍니다.

* Type : string[][]

* Default : []

* Format

```javascript
data : {
    groups: [
        ["2015","2016"], ["2017"]
    ]
}
```

위 예제에서 “2015”, “2016”, “2017” 은 범례 아이디입니다.