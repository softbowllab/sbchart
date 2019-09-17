---
title: index
date: 2018-05-14
categories: ["latest"]
order: 0
---

## SBChart v2.0 Document
---

### global

크기, Padding, 색 패턴, 웹 접근성 항목을 정의할 수 있는 옵션입니다.

{% assign cate = "global" %}
{% assign pages = site.docs | where: "categories", page.categories[0] | where: "categories", cate | sort: "order"%}
{% for item in pages %}
* [{{ item.title }}]({{ site.baseurl }}{{site.path}}{{ item.url }})
{% endfor %}


### data

대상 데이터 및 차트 종류 등 데이터 관련 옵션입니다.

{% assign cate = "data" %}
{% assign pages = site.docs | where: "categories", page.categories[0] | where: "categories", cate | sort: "order"%}
{% for item in pages %}
* [{{ item.title }}]({{ site.baseurl }}{{site.path}}{{ item.url }})
{% endfor %}


### axis

X, Y, Y2 축 관련 옵션입니다.

{% assign cate = "axis" %}
{% assign pages = site.docs | where: "categories", page.categories[0] | where: "categories", cate | sort: "order"%}
{% for item in pages %}
* [{{ item.title }}]({{ site.baseurl }}{{site.path}}{{ item.url }})
{% endfor %}


### grid

Grid 설정 옵션입니다.

{% assign cate = "grid" %}
{% assign pages = site.docs | where: "categories", page.categories[0] | where: "categories", cate | sort: "order"%}
{% for item in pages %}
* [{{ item.title }}]({{ site.baseurl }}{{site.path}}{{ item.url }})
{% endfor %}


### title

타이틀의 위치, 모양에 대한 옵션입니다.

{% assign cate = "title" %}
{% assign pages = site.docs | where: "categories", page.categories[0] | where: "categories", cate | sort: "order"%}
{% for item in pages %}
* [{{ item.title }}]({{ site.baseurl }}{{site.path}}{{ item.url }})
{% endfor %}


### legend

범례의 위치, 모양에 대한 옵션입니다.

{% assign cate = "legend" %}
{% assign pages = site.docs | where: "categories", page.categories[0] | where: "categories", cate | sort: "order"%}
{% for item in pages %}
* [{{ item.title }}]({{ site.baseurl }}{{site.path}}{{ item.url }})
{% endfor %}


### tooltip

툴팁 표시 여부 및 그룹핑 등에 대한 옵션입니다.

{% assign cate = "tooltip" %}
{% assign pages = site.docs | where: "categories", page.categories[0] | where: "categories", cate | sort: "order"%}
{% for item in pages %}
* [{{ item.title }}]({{ site.baseurl }}{{site.path}}{{ item.url }})
{% endfor %}


### extend

차트별 확장 옵션입니다.

{% assign cate = "extend" %}
{% assign pages = site.docs | where: "categories", page.categories[0] | where: "categories", cate | sort: "order"%}
{% for item in pages %}
* [{{ item.title }}]({{ site.baseurl }}{{site.path}}{{ item.url }})
{% endfor %}


### API

제공되는 함수들입니다.

{% assign cate = "API" %}
{% assign pages = site.docs | where: "categories", page.categories[0] | where: "categories", cate | sort: "order"%}
{% for item in pages %}
* [{{ item.title }}]({{ site.baseurl }}{{site.path}}{{ item.url }})
{% endfor %}


### CLASS

CSS 클래스 정의입니다.

{% assign cate = "CLASS" %}
{% assign pages = site.docs | where: "categories", page.categories[0] | where: "categories", cate | sort: "order"%}
{% for item in pages %}
* [{{ item.title }}]({{ site.baseurl }}{{site.path}}{{ item.url }})
{% endfor %}
