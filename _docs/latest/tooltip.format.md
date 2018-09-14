---
title:  tooltip.format
date:   2018-08-16
categories: ["latest","tooltip"]
order: 2
---

## tooltip.format

`#2.0.0`

---

툴팁의 제목, 범레명, 값을 변경 합니다.

* Type : object

* Format
```javascript
tooltip: {
    format: {
        title: function(x) {
            return x + "번쩨 제목입니다.";
        },
        name: function(name, ratio, id, index) {
            return name;
        },
        value: function(value, ratio, id, index) {
            return value;
        }
    }
}
```

### tooltip.format.title

`#2.0.0`

툴팁 제목을 지정합니다.

지정하지 않으면 X축 Tick 라벨이 제목이 됩니다.

* Type : function

* Parameter

  * x : X축 순서를 의미합니다. 0부터 시작합니다.

### tooltip.format.name

`#2.0.0`

툴팁의 범례 이름을 변경합니다.

* Type : function

* Parameter

  * name : 범례명입니다.

  * ratio : 비율값입니다. 원, 도넛 차트만 해당합니다.
  
  * id : 범례(그룹) 아이디입니다.

  * index : 범례 순번입니다. 0부터 시작합니다.

### tooltip.format.value

`#2.0.0`

툴팁의 범례 값을 변경합니다.

* Type : function

* Parameter

  * value : 범례 값입니다.

  * ratio : 비율값입니다. 원, 도넛 차트만 해당합니다.
  
  * id : 범례(그룹) 아이디입니다.

  * index : 범례 순번입니다. 0부터 시작합니다.