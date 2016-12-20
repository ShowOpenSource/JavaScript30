#Dev Tools Source 분석

## 목적

console의 다양한 이벤트를 학습한다.

## 새로운 개념 및 이벤트

### console

* log
  기본 로그

* warn
  경고 알림

* error
  에러 알림

* info
  정보 알림

* debug
  디버그시 로그
  파란색 표시

* assert
  테스트 메서드
  테스트 통과시 표시하지 않고 실패시에만 표시

* clear
  콘솔을 삭제시키고 삭제시켯다고 메시지를 남김

* dir
  콘솔을 디렉토리 구조로추 출려
  함수형태로(?)

* dirxml
  콘솔을 xml형태로 출력

* counting
  해당 내용을 몇번째 찍는지 표시 해줌.

* group
  콘솔들을 묶어줌
  group[Collapsed]
  그룹이 열려있는 상태로 시작[닫혀있는 상태로]
  groupEnd
  끝
* time
  콘솔이 처음찍힌 시간에서 마지막(timeEnd메서드가 발생한 시점)으로 찍힌 시간을 측정
  timeEnd

* table
  object 나 array를 보기 좋게 테이블로 출력

* trace
  메서드 콜된 순서를 출력
  (Prints a stack trace from the point where the method was called.)




출처 : https://developers.google.com/web/tools/chrome-devtools/console/console-reference#consoleerrorobject--object-