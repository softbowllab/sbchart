---
title:  data.keys
date:   2018-05-14
categories: ["latest","data"]
order: 4
---

## data.keys
---

JSON 데이터를 사용할 경우 X축 기준이 될 속성과 값으로 쓰일 속성을 지정합니다.

X축 기준으로 지정된 속성 값이 범례 아이디가 됩니다.

<code>data.json</code>으로 원본 데이터를 지정할 경우 반드시 지정해야하는 옵션입니다.

단일 범례일 경우는 <code>data.keys.x</code> 옵션은 지정하지 않아도 되지만  **data.keys.x** 옵션은 항상 지정해야 합니다.
`#2.0.0`

* Type : object[][]

* Format
```javascript
data : {
    keys: {
        x: "name",
        value: ["seoul","busan","daegu","kwangju","sejong","incheon"]
    },
    json: [
        {name: '2015', seoul: 90, busan: 40, daegu: 50, kwangju: 120, sejong: 80, incheon: 90},
        {name: '2016', seoul: 120, busan: 160, daegu: 200, kwangju: 160, sejong: 130, incheon: 220},
        {name: '2017', seoul: 300, busan: 240, daegu: 290, kwangju: 230, sejong: 300, incheon: 320}
    ]
}
```

### data.keys.x

x축으로 쓰일 속성을 지정합니다.
`#2.0.0`

* Type : string

### data.keys.value

값으로 쓰일 속성들을 지정합니다.
`#2.0.0`

* Type : string[]

* 필수
