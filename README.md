# NaverBoostCamp
NaverBoostCamp Web full-stack developer process

#Web Browser Rendering
How Browser work : Behind the scenes of modern web browsers

<소스 보기> : html의 소스코드를 볼 수 있음.

브라우저의 동작 과정을 알아야 하는 이유 : 브라우저의 동작을 알면, 내가 짠 코드가 어떻게 돌아갈지 알 수 있음.

#Browser Component

UI : OS level의 소프트웨어
Browser Engine : Browser Software Control -> Data Persistant
Rendering Engine : Networking, JavaScript Interpretor, UI backend

#HTML Parser

parsing  HTML : 문자 각각의 의미를 해석하는 것 -> tree 구조

#CSS Box Model

Component
padding
border
margin
등으로 이루어짐.

#Page Source
HTML 문서는 html 태그로 시작해서 html 태그로 끝남.
head는 어떤 html의 추가적인 내용을 담고 있음.
html은 계층적인 구조다.

#html 문서의 구조
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title></title>
</head>
<body>

</body>
</html>

<div> : 요소를 추가할 수 있음.
<style> : css 추가.
<script> : JavaScript code 추기. 보통 html 끝에 추가하는 것이 일반적임.

#Web Server
Web Server : Software, client가 요청하는 html문서나 각종 리소스를 전달하는 것.
Resource : 컴퓨터에 저장되어 있는 정적인 데이터이거나, 프로그램을 통해서 만들어진 동적인 데이터일 수 있음.
Web croller : 다른 웹 사이트 정보를 읽어갈 때, 사용하는 프로그램.

Apache, Nginx, Microsoft, Google WebServer 등이 가장 많이 사용 됨.

#WAS (Web Application Server)
client는 서비스를 제공하는 서버에게 정보를 요청하여 응답 받은 결과를 사용.

DBMS(Database Management System) : 다수의 사용자들이 데이터베이스 내의 데이터를 접근할 수 있도록 해주는 소프트웨어.

MiddleWare : Client와 DBMS 사이의 서버.
(WAS도 MiddleWare의 한 종류.)

#HTML tags
tag의 종류
- 링크
- 이미지
- 목록
- 제목

#HTML latout tags
- header
- section
- nav
- footer
- aside

#CSS 상속 우선순위 결정
- width, height, margin, padding, border 등과 같은 박스 모델- 상속 X
- 상위 엘리먼트가 하위 엘리먼트에 상속됨.
- inline > internal == external CSS
- id > class > element

#CSS selector
span{} - element
#spantag{} - id
#.spanclass - class

+ css에 Web font를 사용할 수도 있음

#Element가 배치되는 방식 (layout; lendering)
- span 같은 tag는 좌->우로 흐름
- display (block, inline, inline-block)
- position (static, absolute, relative, fixed)
- float (left, right)

inline : 옆으로 흐르는 Element
static : 순서대로 배치
absolute : 특정한 위치에 배치 가능 (static이 아닌 position이 기준점)
- top, left 값을 무조건 입력하는 것이 좋음.

- margin으로 배치를 다르게 할 수 있음.

- 기본 배체에서 벗어나서 떠있는 방법 (float:left)
