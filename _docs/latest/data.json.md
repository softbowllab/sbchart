---
title:  data.json
date:   2018-05-14
categories: ["latest","data"]
order: 3
---

## data.json
---

JSON 배열 형태로 차트 데이터를 지정하는 방식입니다.

배열내 JSON 객체는 하나의 범례를 의미합니다.

**반드시** x축 열과 y축 값으로 쓰일 속성들을 [data.keys](/data/data.keys.html)로 지정 하셔야 합니다.

data.keys.x 에 지정된 JSON 속성이 범례 아이디가 됩니다.
`#2.0.0`

* Type : object[]

* Format
```javascript
data : {
    json: [
        {name: '2015', seoul: 90, busan: 40, daegu: 50, kwangju: 120, sejong: 80, incheon: 90},
        {name: '2016', seoul: 120, busan: 160, daegu: 200, kwangju: 160, sejong: 130, incheon: 220},
        {name: '2017', seoul: 300, busan: 240, daegu: 290, kwangju: 230, sejong: 300, incheon: 320}
    ],
    keys: {
        x: "name",
        value: ["seoul","busan","daegu","kwangju","sejong","incheon"]
    }
}
```