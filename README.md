# Kakao-Clone_v2

Module #3 CSS3

1. 기본구조
   selector(id, class, tag name){
   property-name : vlaue;
   property-name : vlaue;
   property-name : vlaue;
   property-name : vlaue;
   }
2. 방식 : 인라인, link
3. padding: 20px 10px; / 상하 좌우 , 4개 기재(상우하좌) 순서
4. block : element가 크기와 상관없이 그 옆에 다른 element가 위치하는 것을 허용하지 않는 것
   -display: inline-block; 사용시 옆으로 위치 가능
5. ★position -absolute : html 상에서 해당 element와 관계있는(relative-부모박스) element를 살펴보고 이에 상응하여 포지션 결정
   (부모 박스가 없다면 본문body에 맞춰서 포지션/ 부모 element에 설정하려면 꼭 부모 element에 relative 포지션 설정)
6. display: flex; : 부모에 적용시킨다.
   http://flexboxfroggy.com/#ko
7. pseudo-selector(가상셀렉터) : 셀렉터인테 element가 아닌 것(id나 class를 사용하지 않고 선택하는 방법)
   -> input + .box : 형제관계
   -> input > .box : 직계관계
   http://www.topdesignagencies.com/nth-test/
8. box-sizing: border-box -> padding을 추가해도 overcompensate하지 않게 함(box가 커지지 않도록 함)

Module #4 Advanced CSS

1. 애니매이션(animation) : 트렌지션으로 효과를 따로 줄필요 없이 이벤트 생성
   - 호출 : animation: 2s scaleAndRotateSquare ease-in-out infinite;
   - @keyframes identifier {
     /_키프레임은 css로 하여금 애니메이션 생성을 알림_/
     }
   -
2. 트랜지션(Transitions)
   - hover : mouseOver, active : mouseClicked, Focus : 선택된 상태일때
   - 참고사이트 : https://developer.mozilla.org/en-US/docs/Web/CSS/transition
3. 트랜스포메이션(Transformations) : html문서의 element들을 변경, 모습이 변하는 효과
   - transition: transform 1s ease-in-out;
   - transform: rotate(2turn) scale(0.5, 0.5);
     /_20deg -> 20도 회전, 5turn -> 5번 회전 _/
   - 참고사이트 : https://developer.mozilla.org/en-US/docs/Web/CSS/transform
4. 미디어쿼리(media query), 브라우저 크기를 알아내서 그것에 맞춰서 움직이는 웹-모바일 반응형
