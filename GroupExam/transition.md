transform (변형)

transform  은 엘리먼트의 크기,위치, 모양을 변경하는 속성입니다.

엘리 먼트 크기 , 비틀기 , 회전등 포토샵에서 가능했던 작업들을 코드화한 기능 ex)2차원 3차원 이있다

transform은 아래와 같은 형식

속성 정리 

https://codepen.io/vineethtr/pen/XKKEgM

https://www.technig.com/css3-2d-transform-tutorial/

https://webplatform.github.io/docs/css/functions/scale3d/

2차원 변형 함수

- tranlate(tx,ty)  지정한 크기만큼 x축과 y축으로 이동합니다.
- translateX(tx) 지정한 크기만큼 x축으로 이동합니다.
- translatezY(ty) 지정한 크기만큼 y축으로 이동합니다.
- scale(sx,sy) 지정한 크기만큼 x축과 y축으로 확대/축소합니다.
- scaleX(sx) 지정한 크기만큼 x축으로 확대/축소합니다.
- scaleY(sy) 지정한 크기만큼 y축으로 확대/축소합니다.
- rotate(각도) 지정한 각도만큼 회전합니다.
- skew(ax,ay) 지정한 각도만큼 x축과 y축으로 왜곡합니다.
- rotate(각도) 지정한 각도만큼 회전합니다.
- skew(ax,ay) 지정한 각도만큼 x축과 y축으로 왜곡합니다.
- skewX(ax) 지정한 각도만큼 x축으로 왜곡합니다.
- skeyY(ay) 지정한 각도만큼 y축으로 왜곡합니다.

3차원 변형함수

2차원 병형함수에 z축을 추가하면 3차원 변형 함수가 됩니다.

3차원 변형함수도 최시브라우저에서는 모두 지원되지만 이전 브라우저를 위해 -webkit-과 -moz-등의 브라우저 접두사를 붙여야 합니다. 인터넷 익스플로러의 경우, 10이상에서 3차원 변형 함수를 지원하므로 -ms-접두사를 따로 사용하지 않습니다.

- matrix3d(n[,n]) : 4*4 행렬을 이용해 이동과 확대/축소, 회전등의 변환을 지정합니다.
- translate3d(tx,ty,tz) :  지정한 크기만큼 x축과 y축,z축으로 이동합니다.
- translateZ(tz) : 지정한 크기만큼 z축으로 이동합니다.
- scale3d(sx,sy,sz) : 지정한 크기만큼 x축과 y축,z축으로 확대/축소 합니다.
- scaleZ(sz) : 지정한 크기만큼 z축으로 이동합니다.
- rotate3d(rx,ry,rz, 각도) : 지정한 각도만큼 회전합니다.
- rotateX(각도) :지정한 각도만큼 x축으로 회전합니다.
- rotateY(각도) : 지정한 각도만큼 y축으로 회전합니다.
- rotateZ(각도) : 지정한 각도만큼 z축으로 회전합니다.
- perspective(길이) : 입체적으로 보일수 있는 깊이 값을 지정합니다.

2차원 변형함수는 최신 브라우저에서는 모두 지원 되지만 인터넷 익스플로러 9를 비롯한 이전 브라우저를 위해 -webkit과 -moz-,-ms-,-o-등의 브라우저 접두사를 붙여야 합니다.

[ transform 지원 범위 ]

  익스플로러 11 부터 지원

  http://caniuse.com/#search=transform

  ex)

  모바일 에서 자주 이용하는 마크업 css

  .test{top:0;width:33.33%;background-position-y:20px;-webkit-transform:translateY(20%);transform:translateY(20%)}  고정

  .test{position:absolute;top:20%} 가변

  wekit

  안전하게 사용

  http://aboooks.tistory.com/271 접두어

transition (전환)

전환은 효과가 변경되었을 때 부드럽게 처리해주는 CSS의 기능입니다. 이와 관련된 것으로는 아래와 같은 속성들이 있습니다. 

transition 표준문법 

transtion: transition-property | transition-duration | transition-timing-function | transition-delay

- transition-property :  css 속성을 지정함
- transition-duration : 트렌지션 실행 시간, 이속성은 항상 지정해 주어야합니다. 그렇지 않을 경우 기본값 0s 이 적용되는 아무런 효과가 나타나지 않습니다. 
- transition-timing-function :  트렌지션이 실행되는 동안 속도 설정
- transition-timing-function : ease | linear | ease-in | ease-out | cubic-bezier()

- linear : 시작부터 끝까지 똑같은 속도로 트랜지션을 진행합니다.
- ease : 처음에는 천천히 시작하고 점점 빨라지다가 마지막에는 천천히 끝냅니다. 기본값입니다.
- ease-in : 시작을 느리게 합니다.
- ease-out : 느리게 끝냅니다.
- ease-in-out : 느리게 시작하고 느리게 끝냅니다.
- cubic-bezier(n,n,n,n)  : 베지에 함수를 직접 정의해 사용합니다. n에서 사용할 수 있는 값은 0~1 입니다.
- transition-delay :  언제 트렌지션을 시작할지 지정

직접 설정 하는곳  http://www.roblaplaca.com/examples/bezierBuilder/#

             http://cubic-bezier.com/#.55,.06,.09,1.11



[transition 브라우저 지원 범위]

 ie 10.0+ ,chrome 26.0+, firefox 16.0+,safari 6.1+,opera 12.1+

접두어 버전 

chrome 4.0+ : -webkit-

firefox 4.0+ : -moz

safari 3.1+ : -webkit - 

opera 10.5+ : -0-

https://www.w3schools.com/cssref/tryit.asp?filename=trycss3_transition-timing-function2

https://www.w3schools.com/cssref/playit.asp?filename=playcss_animation-timing-function&preval=linear

익스플로러 11 부터 지원

http://caniuse.com/#feat=css-transitions

벤더 프리 픽스(접두어 버전 ) 

https://autoprefixer.github.io/

http://cpbest.kr/study/study.html






