### 버블링과 캡쳐링 차이점 
 버블링(fasle)는 자식노드 로부터 이벤트가 발생하여 부모로 이벤트가 전파됩니다.
 캡쳐링(true)는 버블링과 반대로 부모노드에서 자식노드로 이벤트가 전파됩니다.

버블링 결과 
ex) https://codepen.io/choiyunmi/pen/NvmwMR
결과
c b a
 b a
  a

캡쳐링 결과 
ex) https://codepen.io/choiyunmi/pen/NvmwMR
결과
a b c
 b c
  a

이벤트의 전이되는것을 차단 하려 면   stopPropagation()  메서드를 사용하면 이벤트 전파는 차단된다.

참고 url http://romeoh.blog.me/140178486203


####  Element.offsetHeight 
- 실제 내용의 높이 + padding-top + padding-bottom + border-top  + border + bottom

####  Element.clientHeight
- 실제 내용의 높이 + padding-top + padding - bottom

#### Element.scrollHeight 

#### outerHeight()
- padding , border 값포함
- $(element).outerHeight(true); margin 을 포함한 높이값
- $(element).outerHeight(); margin 을 제외한 높이값

#### innerHeight()
padding값 까지만 포함한 내부 높이

#### height()
padding값도 제외한 순수 내용의 높이만 리턴

### fixed 확대 안튀는것
height + 95px sticky 클래스 추가 
sticky-wrap  높이값을 갖고와서 안의 컨텐츠 영역이 fixed의 뜨는 속성 값을 자연스럽게 막아준다.
ex) top부분의 자연스럽게 나타나고  footer부분에서사라지는 효과animate 콜백함수를 이용하여 사용해보기!!
this._welSticky.outerHeight(true) 

참고 url 
- http://eppffy.tistory.com/26
- https://github.com/telltrue33/telltrue33.github.io/blob/master/convention/02_Etc.md
- https://developer.mozilla.org/ko/docs/Web/API/Element/scrollHeight



#sort 
184 line ~ 187 line down 오름차순 일경우의 case
- https://github.com/Hongzoo/study/blob/gh-pages/JavaScript/se_ui/exam06/sort.html

- https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array/sort





