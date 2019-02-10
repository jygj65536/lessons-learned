---
layout: post
title: "C++ Development environment with Visual Studio Code"
categories: misc
---

VS Code가 가볍고 좋다는 얘기를 들어서 C++ 컴파일, 디버깅 환경을 구성하고 Github와 연동하는 것을 공부하였다. 일단 해본 지금의 소감으로는 썩 편하지 않다. 아주 원시적인 방법으로 환경을 구축해서 그런 것이라는 생각이 들고, 익숙해지면서 좀 더 편한 환경을 찾을 수 있도록 노력해야겠다.

https://youtu.be/UHS-aenkPPg

내가 현재 필요한 부분인 28분까지만 보고 해당 내용을 따라하면서 에디터에서 작성한 코드를 빌드(컴파일)하는 것과 실행해 보았고, 작동하는 것을 확인하였다. 또, VS Code 안에 있는 Github 연동 기능을 사용해서 Github에 직접 코드를 업로드해보기도 했는데, 내가 제대로 못 다뤄서 그런 것이겠지만 커맨드라인보다 그렇게 편한 것 같지도 않다 :(

코드를 작성한 다음, 빌드하기 위해 tasks.json 파일을 만들어서 어떤 파일을 어떤 컴파일러로 빌드할 것인지를 지정한다.

```json
{
    // See https://go.microsoft.com/fwlink/?LinkId=733558
    // for the documentation about the tasks.json format
    "version": "2.0.0",
    "tasks": [
        {
            "label": "build",
            "type": "shell",
            "command": "g++ -g 2455_허자용.cpp -o 2455_허자용", 
            "group": {
                "kind": "build",
                "isDefault": true
            },
            "problemMatcher":"$gcc"
        }
    ]
}
```
