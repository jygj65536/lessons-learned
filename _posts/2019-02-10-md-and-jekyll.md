---
layout: post
title: "Markdown, Github Page, Jekyll"
categories: misc
---

이미지를 첨부하는 방법을 찾았다. 앞으로 이미지를 사용하여 공부한 내용을 정리할 수 있을 것 같다.
<br></br>
<br></br>
<br></br>
<br></br>
![My helpful screenshot]({{ "/assets/screenshot.png" | absolute_url }})
<br></br>
<br></br>
<br></br>
<br></br>

어제 궁금해했던 내용도 찾았다. \`은 backtick이라고 부르는 모양인데, 위 이미지에서 보듯이 앞에 backslash(\\)를 붙여주면 해당 문자 그대로 출력이 가능하다.
<br></br>
<br></br>
<br></br>
<br></br>
recent
이미지 첨부를 하는 데에도 여러 번의 삽질이 있었다. Markdown과 Jekyll의 문법이 약간 달라서 헤멨다. 즉, 내가 포스트를 작성할 때 필요한 문법은 Markdown문법과 비슷하지만, 또 다른 부분이 있다. 위 이미지를 삽입하는 데에도 유의해야 할 점이 몇 가지 있었는데, 1)파일명에 space가 들어가면 안된다.(이건 Markdown에서도 공통) 2)Markdown에 이미지를 삽입하는 방식으로 경로를 지정해줘도 페이지에서는 나오지 않는다. `absolute_url`필터를 붙여줘야 한다.

Github page는 수정한 내용이 반영되는데 딜레이가 있어서 불편하다. 몇 초밖에 안걸리긴 하지만 지금처럼 시행착오를 거치는 와중에는 *결과를 기다리는 것*과 _반영이 됐는지 안됐는지를 알 수가 없다는 점_ 이 **상당**__히__ 거슬린다.

# This is an `<h1>` tag
## This is an `<h2>` tag

### This is an `<h3>` tag


#### This is an `<h4>` tag



##### This is an `<h5>` tag
###### This is an `<h6>` tag

Mardown syntax들을 시험하고 있는데, 제일 처음인 header 태그부터 거슬리는 것을 발견했다. 
1. Enter로 간격 조절이 안 된다. 각 태그마다 자신만의 간격을 가지고 있다. 이건 원래 그랬으니 그렇다 쳐도
2. 원래 h1부터 h6까지 크기 순으로 되어있어야 하지만 jekyll 문법에서는 h1이 따로 놀게 되어있다. h2부터 h6까지는 기존처럼 써도 되지만(약간의 차이는 있다) h1은 h3보다 조금 작아서 다른 header 태그들과 같이 쓰게 된다면 크기 순서에 혼란이 온다.

(+) 어제는 Markdown은 널리 쓰이는 형식이기 때문에 Github Markdown 문법이라는게 없다고 생각했지만, [막상 그렇지도 않았다]({{ "/assets/markdown-cheatsheet-online.pdf" | absolute_url }}). Github에서만 사용가능한 Markdown 문법이라는 것이 있긴 있는 것이다. 하지만, 그게 Jekyll에서 그대로 동작할 것인지는 또 다른 문제라는 것이 귀찮은 점이다.
