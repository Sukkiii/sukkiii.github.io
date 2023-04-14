---
layout: single
title:  "뷰 인스턴스"

categories: 
- Vue-story

tags: 
- vue
- codingstudy
- vue_instance 
---


# 뷰 인스턴스의 정의와 속성

인스턴스와 컴포넌트를 레고에 비유한다면 인스턴스는 레고를 조립하는 기본 판을, 커포넌트는 레고 블럭을 의미한다.

## 뷰 인스턴스 속성

```html
<html>
    <head>
        <title>Vue Sample</title>
    </head>
    <body>
        <div id="app">
            {{message}}
        </div>
        <script src="https://cdn.jsdelivr.net/npm/vue@2.5.2/dist/vue.js"></script>
        <script>
            new Vue({
                el: '#app', //el 속성
                data: {
                    message: 'Hello Vue.js!'
                }
            });
        </script>
    </body>
</html>
```

'Hello Vue.js!' 텍스트를 화면에 표시하기 위해서 new Vue()로 뷰 인스턴스를 생성하였고, 인스턴스 안에 el 속성으로 뷰 인스턴스가 그려질 지점을 지정하고, data속성에 message 값을 정의하여 화면에 그 값을 연결하였다.

### 뷰 인스턴스 생성자

new Vue()로 인스턴스를 생성할 때 Vue를 생성자라고 한다.

### 뷰 인스턴스 옵션 속성

뷰 인스턴스 옵션 속성은 인스턴스를 생성할 때 재정의할 data, el, template등의 속성을 의미한다.
- el: 뷰로 만든 화면이 그려지는 시작점을 의미. 뷰 인스턴스로 화면을 렌더링할 때 화면이 그려질 위치의 돔 요소를 지정하는 역할
- template: 화면에 표시할 HTML, CSS등의 마크업 요소를 정의하는 속성. 뷰의 데이터 및 기타 속성들도 화면에 함께 그릴 수 있음.
- methods: 화면 로직 제어와 관계된 메서드를 정의하는 속성. 마우스 클릭 이벤트 처리와 같이 화면의 전반적인 이벤트와 화면 동작과 관련된 로직을 추가할 수 있음.
- created: 뷰 인스턴스가 생성되자마자 실행할 로직을 정의할 수 있는 속성.

<span style="color:gray"> 해당 내용은 이지스퍼블리싱의 Do it! Vue.js 입문 교재의 내용을 인용하고 추가적으로 알고 있는 내용을 덧붙여 작성했습니다.</span>
    
