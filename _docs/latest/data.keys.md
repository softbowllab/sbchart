---
title:  data.keys
date:   2018-05-14
categories: ["latest","data"]
order: 4
---

## data.keys

`#2.0.0`

---

JSON 데이터를 사용할 경우 X축 기준이 될 속성과 값으로 쓰일 속성을 지정합니다.

value속성 에 지정된 값들이 범례 아이디가 됩니다.

JSON 형태 데이터(<code>data.json</code>)를 사용한 경우 반드시 지정해야하는 옵션입니다.

* Type : object[][]

* Format
```javascript
data : {
    keys: {
        x: "name",
        value: ["2015","2016","2017"]
    },
    json: [
        {"name": "seoul", "2015": 90, "2016": 120, "2017": 300},
        {"name": "busan", "2015": 40, "2016": 160, "2017": 240},
        {"name": "daegu", "2015": 50, "2016": 200, "2017": 290},
        {"name": "kwangju", "2015": 120, "2016": 160, "2017": 230},
        {"name": "sejong", "2015": 80, "2016": 130, "2017": 300},
        {"name": "incheon", "2015": 90, "2016": 220, "2017": 320}
    ]
}
```

### data.keys.x

`#2.0.0`

x축으로 쓰일 속성을 지정합니다.

* Type : string

### data.keys.value

`#2.0.0`

값으로 쓰일 속성들을 지정합니다.

* Type : string[]

* 필수
