#Video Source 분석

## 목적

Video 소스 코드를 분석하고 어떤 메서드가 있는지 알아봄

## 새로운 개념 및 이벤트

### Video
  비디오를 사용 할 수 잇는 태그이다.
  play
  paused
  currentTime
  volume
  playbackRate
  duration

참고 : http://www.w3schools.com/TAGs/ref_av_dom.asp

### ProgressBar
  flexBasis


### 신기한 문법 ?!
  ```
  function aaa(){
    console.log("!!!!")
    return false
  }

  function ccc(){
    console.log("!!!!2")
  }

  function bbb(){
    let foo = true;

    foo && aaa() && ccc();
  }


  bbb();

  ##
  결과
  !!!!만 나온다.

  이유는 체이닝의 원리와 비슷하게
  앞의 결과가 true이면 다음 함수를 실행시킴!

```