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
