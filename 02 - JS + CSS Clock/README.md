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

* animation
  CSS3 애니메이션은 엘리먼트에 적용되는 CSS 스타일을 다른 CSS 스타일로 부드럽게 전환시킴.
  애니메이션은 애니메이션을 나타내는 CSS 스타일과 애니메이션의 중간 상태를 나타내는 키프레임들로 이루어짐.

  animation-delay
    엘리먼트가 로드되고 나서 언제 애니메이션이 시작될지 지정.
  animation-direction
    애니메이션이 종료되고 다시 처음부터 시작할지 역방향으로 진행할지 지정.
  animation-duration
    한 싸이클의 애니메이션이 얼마에 걸쳐 일어날지 지정.
  animation-iteration-count
    애니메이션이 몇 번 반복될지 지정.
    infinite로 지정하여 무한히 반복 가능
  animation-name
    이 애니메이션의 중간 상태를 지정.
    중간 상태는  @keyframes 규칙을 이용하여 기술.
  animation-play-state
    애니메이션을 멈추거나 다시 시작할 수 있음.
  animation-timing-function
    중간 상태들의 전환을 어떤 시간간격으로 진행할지 지정.
  animation-fill-mode
    애니메이션이 시작되기 전이나 끝나고 난 후 어떤 값이 적용될지 지정.

  * @keyframe
    at-rule(@) 개발자가 애니메이션 중간중간의 특정 지점들을 거칠 수 있는 키프레임들을 설정함으로써 CSS 애니메이션 과정의 중간 절차를 제어할 수 있게함.
    <identifier>
      keyframe 이름
    from
      시작(0%)
    to
      끝(100%)
    <percentage>
      지점(%)

  출처 : https://developer.mozilla.org/ko/docs/Web/CSS/CSS_Animations/Using_CSS_animations
