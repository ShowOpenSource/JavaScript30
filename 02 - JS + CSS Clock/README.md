#Clock Source 분석

## 목적

아날로그 시계처럼 동작하도록 구현한다.

## 새로운 개념 및 이벤트

* transition
  CSS 속성을 변경할 때 애니메이션 속도를 조절하는 방법

  transition-property
    CSS 속성의 이름 혹은 이름
  transition-duration
    트랜지션이 일어나는 지속 시간을 명시
  transition-timing-function
    속성의 중간값을 계산하는 방법을 정의하는 함수를 명시

  transitionend
    트랜지션을 완료하면 발생하는 단일 이벤트

  출처 : https://developer.mozilla.org/ko/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions

* transform
  transform은 요소 박스를 변형하는 속성.
  2차원, 3차원 변형이 가능하고, 변형 형태별로 함수 타입의 속성값을 지정.

  * 2d transform
    translate()
      수평 이동
    scale()
      크기 조절
    rotate()
      회전
    skewX()
      X축 기울기
    skewY()
      Y축 기울기
    matrix()
      이동 및 회전 크기 변화와 기울임등을 복합적으로 적용할 수 있는 기능
      maxtrix(num, num, num, num, num, num);
      순서는 scaleX, skewX, skewY, scaleY, translateX, translateY 이다
    transform-origin
      transform의 변형 기준점을 지정하는 속성
    perspective
      3D 공간에서 요소와 관측 점과의 거리, 즉원근감을 자정하는 속성
    perspective-origin
      3D 공간상에서 원근감의 방향을 지정하는 속성

  출처 : http://blog.singihae.com/css3-transform-or-transition-or-animaiton/


* style 객체를 통해서 style 변경하기
  DOM을 통해, 요소의 스타일을 결정하는 style 객체에 접근가능.
  이 style 객체는 CSSStyleDeclaration 으로 정의됨.
  [DOM].style.[속성이름] 으로 스타일을 직접 변경가능하다.

  출처 : http://www.clearboth.org/48_dynamic_style_-_manipulating_css_with_javascript/
