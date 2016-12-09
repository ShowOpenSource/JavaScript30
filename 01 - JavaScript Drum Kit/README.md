#DRUM Source 분석

## 목적

키보드를 클릭하여 DRUM 소리를 내고 애니메이션을 준다.

## 새로운 개념 및 이벤트

* querySelector
	selector들이 지정한 그룹과 일치하는 document 내의 첫 번째 element를 반환합니다.
    querySelectorAll 도 있는데 이는 모든 문자열을 가져옴.
    
    출처 : https://developer.mozilla.org/ko/docs/Web/API/Document/querySelector
    
* es6 문자열 템플릿(Template String) 
	따옴표 문자 대신 백틱(backtick) 문자를 사용하여 표현
    탬플릿 대입문을 사용해서 다이나믹하게 데이터를 추가함(${})
    탬플릿 대입문에는 함수도 사용 가능하다.
    템플릿 인셉션 : 템플릿 문자열을 다른 템플릿 문자열 안에 포함시키는 것도 가능.
    줄바꿈과 들여쓰기 등 템플릿 문자열 속의 모든 화이트 스페이스들은 있는 그대로 포함됨.
	\`${[something]}\`
    
    출처 : http://hacks.mozilla.or.kr/2015/08/es6-in-depth-template-strings-2/
    
* classList
	해당 엘리먼트에서 classList 를 불러온다.
    아래 함수를 사용하여 추가, 제거 ,토글도 가능하다.
	add
    remove
    toggle
    item 
    
    출처 : https://developer.mozilla.org/ko/docs/Web/API/Element/classList
    
* transitionend event
	transition 이벤트가 끝나면 실행되는 이벤트이다!
    
* audio Element 
	문서에 소리 컨텐츠를 포함하기 위해 사용됩니다. 
    이것은 src 속성이나 <source> 요소를 통해 여러 오디오 소스를 포함할수 있음.
    currentTime
    
## 참고

http://keycode.info/ 홈페이지를 참고 하면 키보드의 key-code를 구할 수 있다.
