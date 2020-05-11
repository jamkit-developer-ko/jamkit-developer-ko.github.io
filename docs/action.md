---
layout: page
title: 액션
nav_order: 7
---

# {{page.title}}

## 액션의 대상 지정

액션을 실행할 때, 해당 액션을 수행할 대상을 지정할 수 있다. 그 대상은 크게 오브젝트(object), 뷰(view), 그리고 컨트롤러(controller)이다. 액션을 지정할 때에는 ```target``` 속성을 이용한다. 예를 들어 특정 오브젝트에 ```reload``` 액션을 수행하도록 지정하려면 다음과 같이 기술하면 된다.

```
action=reload, target=object, object={오브젝트의 ID}
```

## 액션의 전달 경로

액션 명령은 액션이 처리될 때까지 전달(propagation)된다. 액션을 처리하는 최종 담당자는 컨트롤러(controller)이다. 컨트롤러에 의해서도 처리될 수 없는 액션은 최종적으로 무시된다.

뷰(view) -> 컨트롤러(controller)
오브젝트(object) -> 컨트롤러(controller)

