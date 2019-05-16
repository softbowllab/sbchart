---
title: global.animation
date: 2019-05-14
categories: ["latest","global"]
order: 6
---

## global.animation

`#2.0.13`

---

차트에 애니메이션 기능을 설정합니다.


* Type : Object

* Format
```javascript
global: {
	animation: {
		show: true,
		type: "rise",
		types: {data1: "rise", data2: "fill"},
		delay: 800,
		ease: "bounce"
	}
}
```


### global.animation.show

`#2.0.13`

애니메이션 효과의 사용 여부를 설정합니다. 기본값은 false입니다.

* Type : Boolean

* Default : false



### global.animation.type

`#2.0.13`

적용할 애니메이션 타입을 설정합니다.
차트 종류에 따라 설정값이 달라집니다.

* Type : String

* Default : "rise" / "pop" / "fan" 

* Values (Bar 계열 차트 - bar, stackbar, stackbar 100%)
	* "rise": `Default` 
	* "fill" 
	* "mixed"
	* "fade"


* Values (Line 계열 차트 - line, spline, area, step, area-spline, area-step, stackarea, stackarea 100%)
	* "rise": `Default` 
	* "fill" 
	* "fade" 


* Values (bubble 차트)
	* "pop": `Default` 
	* "fade"


* Values (원 계열 차트 - pie, donut, gauge)
	* "fan": `Default` 
	* "circle"
	* "fade"


### global.animation.types

`#2.0.13`

콤비네이션 차트에서 적용할 애니메이션 타입들을 설정합니다.
적용 가능한 타입은 `global.animation.type`의 Values와 동일합니다.

* Type : Object


### global.animation.delay

`#2.0.13`

애니메이션 효과가 완료되기까지의 시간을 설정합니다.

* Type : Number (밀리초단위)

* Default : 500


### global.animation.ease

`#2.0.13`

애니메이션 가속도 효과를 설정합니다.

* Type : String

* Default : "linear"

* Values
	* "linear": `Default` 
	* "back"
	* "bounce"
	* "circle"
	* "cubic"
	* "elastic"
	* "exp"
	* "poly"
	* "quad"
	* "sin"


* 상세한 동작은 [D3.ease](https://github.com/d3/d3-ease){:target="_blank"}를 참조하세요.