---
title:  render()
date:   2018-06-19
categories: ["latest","API"]
order: 1
---

## 차트객체 생성 및 랜더링
---

차트 객체를 생성 하는 방식은 

1. static 함수인 <code>sb.chart.render()</code> 를 사용하는 방식과

1. 인스턴스를 직접 생성하는  <code>new sb.chart()</code> 방식

2가지로 나누어지며 첫번째 방식 <code>sb.chart.render()</code> 함수는 객체 생성과 랜더링이 동시에 수행됩니다.


### sb.chart.render()

SBChart 객체를 생성하고 랜더링합니다.

static 함수이며 리턴값은 차트 Object 입니다.

* Parameters

  * 차트를 그려줄 엘리먼트 (bind element), Mandatory 

  * 차트 옵션 (데이터 포함), Mandatory

* Return

  * SBChart 객체

* Example

  ```javascript
var chart = sb.chart.render("#chartWrap",{
	data: {
		columns: [
			["2015",3.51,4.6,3.43,7.96,3.37,5.83,0.35,3.23,-0.09,4.47,2.21,1.13,0.77,0.35,0.92,2.65,1.64,8.08]
		]
	}
});
```


### [SBCHART].render()

이미 생성된 SBChart 객체에 차트를 (다시) 그려주기 위한 함수입니다.

* Parameters

  1. 차트를 그려줄 엘리먼트 (bind element), Optional

  1. 차트 옵션 (데이터 포함), Optional

* Example # 1

  ```javascript
var chart = new sb.chart("#chartWrap",{
	data: {
		columns: [
			["2015",3.51,4.6,3.43,7.96,3.37,5.83,0.35,3.23,-0.09,4.47,2.21,1.13,0.77,0.35,0.92,2.65,1.64,8.08]
		]
});
//랜더링-파라메터 없음
chart.render();
```

* Example #2

  ```javascript
var chart = new sb.chart("#chartWrap");
//랜더링-파라메터 1개
chart.render({
	data: {
		columns: [
			["2015",3.51,4.6,3.43,7.96,3.37,5.83,0.35,3.23,-0.09,4.47,2.21,1.13,0.77,0.35,0.92,2.65,1.64,8.08]
		]
});
```

* Example #3

  ```javascript
var chart = new sb.chart();
//랜더링-파라메터 2개
chart.render("#chartWrap", {
	data: {
		columns: [
			["2015",3.51,4.6,3.43,7.96,3.37,5.83,0.35,3.23,-0.09,4.47,2.21,1.13,0.77,0.35,0.92,2.65,1.64,8.08]
		]
});
```
