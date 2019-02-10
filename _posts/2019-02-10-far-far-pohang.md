---
layout: post
title: "다시 시작"
categories: misc
---

이미지를 첨부하는 방법을 찾았다. 앞으로 이미지를 사용하여 공부한 내용을 정리할 수 있을 것 같다.

![My helpful screenshot]({{ "/assets/screenshot.png" | absolute_url }})

쉽지 않았다. 유의해야 할 점이 몇 가지 있는데, 1)파일명에 space가 들어가면 안된다. 2)Markdown에 이미지를 삽입하는 방식으로 경로를 지정해줘도 페이지에서는 나오지 않는다. `absolute_url`필터를 붙여줘야 한다.

`
# This is <h1> tag
## This is <h2> tag
###### This is <h6> tag
`
# This is an `<h1>` tag
## This is an `<h2>` tag
###### This is an `<h6>` tag
