---
layout: post
title: "결코 다시 포항"
categories: misc
---

이미지를 첨부하는 방법을 찾았다. 앞으로 이미지를 사용하여 공부한 내용을 정리할 수 있을 것 같다.

![My helpful screenshot]({{ "/assets/screenshot.png" | absolute_url }})

쉽지 않았다. Markdown과 Jekyll의 문법이 또 달라서 헤멨다. 즉, 내가 포스트를 작성할 때 필요한 문법은 Markdown문법과 비슷하지만, 분명 다른 부분이 있다. 위 이미지를 삽입하는 데에도 유의해야 할 점이 몇 가지 있었는데, 1)파일명에 space가 들어가면 안된다.(이건 Markdown에서도 공통) 2)Markdown에 이미지를 삽입하는 방식으로 경로를 지정해줘도 페이지에서는 나오지 않는다. `absolute_url`필터를 붙여줘야 한다.

Github page는 수정한 내용이 반영되는데 딜레이가 있어서 불편하다. 몇 초밖에 안걸리긴 하지만 지금처럼 시행착오를 거치는 와중에는 결과를 기다리는 것과 반영이 됐는지 안됐는지를 알 수가 없다는 점이 상당히 거슬린다.

# This is an `<h1>` tag
## This is an `<h2>` tag

### This is an `<h3>` tag


#### This is an `<h4>` tag



##### This is an `<h5>` tag
###### This is an `<h6>` tag

header tag를 시험하던 중에 이상한 것을 발견했다. Enter로 간격 조절이 안 되는 것은 상당히 거슬리지만 그렇다 쳐도, Markdown에서는 h1부터 h6까지 크기 순으로 되어있는 반면에 jekyll을 사용한 블로그에서는 왠지 모르게 h2가 h1보다 더 크게 나타나게 되어있어서 이상하게 출력이 된다. 이게 맞는지 확인하려고 여러 번 새로고침을 하고 기다려도 봤으나(이게 거슬린다) 
