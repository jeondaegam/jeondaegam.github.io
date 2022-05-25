---
emoji: 🎁   
title: What is Webpack?   
date: '2022-05-25 21:15'  
author: 여름  
tags: webpack, nodejs, npm  
categories: ECT
---

###Webpack  
`Webpack is a module bundler for JavaScript applications.`  
Webpack은 Javascript를 위한 bundler이다.  
서로 관련있는 파일들을 하나로 bundling(=packaging)해준다.  

###Bundler의 역할
모듈화된 js 파일들을 묶어준다.   
따라서 번들링이란 모듈화된 js 파일을 묶어준다는 의미이다.   


### 왜 나온거지?(todo)
Software가 커질수록 세분화된 모듈은 많아지고, 
모듈 단위의 파일들을 호출할 때 변수들의 스코프 문제,
호출할 때의 네트워크 코스트도 신경써야 한다.

### Bundling을 하면 왜 좋을까?
- 동일한 타입(html, css, js등)의 파일을 묶어 요청/응답할 수 있으므로 network cost가 감소한다.   
  예를들어 A 파일에서 B 파일을 호출해야 할 경우 두 파일을 하나로 묶어 네트워크 요청을 최소화 할 수 있다.
- webpack의 주요 구성요소중 하나인 Loader가 일부 브라우저에서 지원이 되지 않는 
ES6 형식의 js 파일을 ES5로 변환하여 사용할 수 있게 만들어준다.

  
### Webpack의 구성요소

### 1. Entry(todo)

### 2. Output
webpack의 번들링에 대한 결과를 어느 경로에 생성해낼 것인지와 이름을 정의하는 요소이다.
- webpack.config.js  
  `path`: 번들을 생성할 경로  
    `name`: 파일명
```javascript
module.exports = {
	entry: './App.js',
	output: {
		path: './dist',
		filename: 'bundle.js'
              }
}
```

### 3. Loaders
`webpack only understands JavaScript and JSON files.`  
webpack은 오직 js와 json 파일만 이해한다.  
loader는 다른 유형의 파일을 webpack이 이해할 수 있는 모듈로 변환한다.  
loader를 사용하면 webpack이 다른 유형의 파일을 application에서 사용하고 종속성 그래프에 추가할 수 있는 유효한 모듈로 변환할 수 있다. 

### 4. Plugins
번들링된 결과물에 대해 적용할 수 있는 속성이다.  
번들링된 .js 파일을 난독화 하거나 번들링된 .css, .js 파일들을 html 파일에 주입하는 등의 역할을 한다.  
번들된 파일을 압축, 복사, 추출, 별칭 등의 부가 작업 가능
번들링된 파일별 커스텀을 위해 사용한다.  

### 설치(todo)
npm을 이용해 설치한다.

### webpack.config.js(todo)
root directory에 생성한다.

### webpack.config.js 설정하기(todo)


### Webpack 5의 이전버전과의 차별점?? 


**Reference**  
[webpack.js.org](https://webpack.js.org/)  
[What is Webpack?](https://hipdizzy.tistory.com/91)
  
  
