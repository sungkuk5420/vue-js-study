# vue-js-study
인프런 Vue js 완벽 가이드 - 실습과 리팩토링으로 배우는 실전 개요.

### 시작날짜 2021년 02월 26일

### 강의에서 다루는 내용
1.Vue.js를 이용한 웹 서비스 구현 절차
2.실무 프로젝트 진행 방식(컴포넌트, 라우터, API, 스토어)
3.컴포넌트 디자인 패턴과 자바스크립트 비동기 처리
4.Mixins과 HOC를 이용한 컴포넌트 재활용 방법
5.외부 라이브러리 모듈화 및 실무 프로젝트 구성 방법
6.사용자 경험을 높이는 라우터 설계 방법과 고급 라우터 패턴.
Vuex를 사용한 API 호출과 Vuex를 사용안한 API 호출 비교

### 강의에 사용되는 플러그인
색 테마 : Night Owl
파일 아이콘 테마 : Material Icon Theme
뷰 확장 플러그인 : Vetur
뷰 코드 스니펫 : Vue VSCode Snippets
문법 검사 : ESLint, TSLint
실습 환경 보조 : Live Server
기타
Prettier, Path Intellisense, Project Manager, HTML CSS Support, Auto Close Tag, GitLens, Atom Keymap, Jetbrains IDE Keymap 등


### 코드 컨벤션 및 스타일 가이드
https://kr.vuejs.org/v2/style-guide/index.html

### 만들어볼 사이트는 Hacker News 의 클론 코딩.
```
공식 사이트
https://news.ycombinator.com/


api
https://github.com/tastejs/hacker-news-pwas/blob/master/docs/api.md
```

### vue create vue-cli3
npm install -g @vue/cli

명령어 
-2.x : vue init '프로젝트 템플릿 이름' '파일위치'
-3.x : vue create '프로젝트 이름'

Default ([Vue 2]babel, eslint)를 고를것.

## eslint
```
package.json에 설정 내용이 들어가있다.


```

### 라우터 기본
```
뷰 라우터 설치
npm install --save vue-router@3.0.2
그후 main.js에


import Vue from 'vue'
import App from './App.vue'
import vueRouter from 'vue-router'

Vue.config.productionTip = false
Vue.use(vueRouter)

const router = new vueRouter({
  routes:[

  ]
})

new Vue({
  render: h => h(App),
  router
}).$mount('#app')


이렇게 작성한다.
redirect속성과 router-link
```

## 확장프로그램 목록
```
 vetur를 확장프로그램으로 설치하면 뷰파일 인식이 된다.
 vue peek 컴포넌트 링크이동

```