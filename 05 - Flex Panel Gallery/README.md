#Flex Panel Source 분석

## 목적

Flex 사용 법을 익힌다.

## 새로운 개념 및 이벤트

### flex
	새로운 레이아웃 모듈 중에 가장 포괄적인 격자 레이아웃과 함께 유동적인 레이아웃 모듈 또는 플렉스박스
	가장 기본적인 기능은 크기를 "유연"하게 조절하는 능력
	![alt tag](http://cfile3.uf.tistory.com/image/234B6A3F555354160CDAAF)
	* display에서 flex를 지정해줘야 flex를 사용 가능
	* flex의 부모 프로퍼티
		* flex-direction
            방향, 흐름, 시각적인 순서처리 
		* flex-wrap
            플렉스 항목들이 열을 바꾸는 방법을 제어하는 속성
		* flex-flow
            flex-direction과 flex-wrap 값을 명시하는 단축 속성
		* justify-content
		* align-items
		* align-content
	* flex의 자식 프로퍼티	
		* order
		* flex-grow
            양수 정수
            이 값은 남는 공간 중 얼마를 지정된 플렉스 항목에 분배해야 하는지 그 정도를 제어
		* flex-shrink
            양의 정수
            모자라는 공간을 회수할 때 해당 플렉스 항목이 플렉스 컨테이너상의 다른 항목들에 비해 얼마나 줄어들지를 결정
		* flex-basis
            너비 값을 수용하고 플렉스 항목의 초기 크기를 설정
		* flex
            위의 3가지를 한번에 설정할수 있음.
            flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
            플렉스 컨테이너 내부의 플렉스 항목들의 길이를 지정할 수 있고 각 항목 사이에 배분되는 여유 공간은 다음 세 가지 인자에 의해서 결정
            
		* align-self

출처 :https://css-tricks.com/snippets/css/a-guide-to-flexbox/
http://webdir.tistory.com/349
http://webclub.tistory.com/259