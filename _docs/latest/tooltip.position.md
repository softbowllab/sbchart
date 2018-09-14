---
title:  tooltip.position
date:   2018-08-17
categories: ["latest","tooltip"]
order: 3
---

## tooltip.position

`#2.0.0`

---

툴팁의 표시 위치를 변경합니다.

툴팁이 그려질 top, left 값을 지정해 주셔야 합니다.

이때 top, left 값은 해당 페이지의 top, left 가 아닌 차트 영역내의 상대값입니다.

* Type : function

* Format
```javascript
tooltip: {
    position: function(data, element, width, height) {
        return {top: 300, left: 0};
    }
}
```

* Parameter

  * data : 표시되는 해당 툴팁의 각 범례별 데이터입니다. 

    * Type : object[]

    * object 구조는 아래와 같습니다.

    ```javascript
	{
		x: 5,
		value: 16,
		id: "data1",
		index: 0,
		ratio: 0.16,
		name: "범례1"
	}
    ```

    * x : X축 순서를 의미합니다. 0부터 시작합니다.

    * name : 범례명입니다.

    * value : 범례 값입니다.

    * ratio : 비율값입니다. 원, 도넛 차트만 해당합니다.

    * id : 범례(그룹) 아이디입니다.

    * index : 범례 순번입니다. 0부터 시작합니다.

  * element : 툴팁 대상이 되는 차트 Element 입니다.
  
  * width : 툴팁 영역 너비입니다.

  * height : 툴팁 영역 높이입니다.
