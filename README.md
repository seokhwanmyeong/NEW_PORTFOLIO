## 명석환의 PORTFOLIO에 오신 것을 환영합니다.

 이 페이지는 명석환의 포트폴리오를 담은 페이지 입니다.
 

##### [LuckShop](https://seokhwanmyeong.github.io/LuckShop/luckshop/index.html)

처음으로 만든 외국사이트 리뉴얼한 사이트입니다.

디자인컨셉: 심플한 가정제품 판매 쇼핑몰

-개발과정-
레이아웃 : 거의 모든 레이아웃을 float를 사용해 제작하였습니다. (float해제는 clearfix class사용)
모션 : css3의 가장 핵심적인 기술인 transition,transform,box-showdow 등을 자주 사용하여 만들었고 특히 gnb부분은
자주 쓰이는 jquery slideToggle을 사용하지 않고 오로지 css3기능으로만 제작하였습니다.
슬라이더는 bxSlide 플로그인으로 사용해 만들었습니다.
반응형 : pc버전 , 태블릿버전, moblie 버전 3가지로 미디어쿼리를 사용해 제작 하였습니다.


-느낀점-
반응형 홈페이지를 제작할 때 float의 width값을 정해진 px값보다 %로 넣어야지 미디어쿼리 작성할때 훨씬 편하다는 걸 느꼈습니다.
css3의 여러가지 기능들이 아직 익스 9이하부터는 적용되지 않는 부분이 있었습니다(ex. transform:translate(-50%))등
float해제방법으로는 5가지정도가 있지만 가장 보편적으로 사용되는게 float사용한 부모에게 overflow:hidden을 주는 방법인데
모션 제작할때 조금 제약을 받은것같아 clearfix사용한 해제사용 방법이 개인적으로는 가장 좋았던 것 같습니다.



###  printbakery

학원을 다니고 처음만든 사이트로 기존의 printbakery를 리모델링한 사이트입니다.

디자인컨셉: 미술용품 판매 사이트

-개발과정 -
레이아웃 : showBox와 마찬가지로 모든 레이아웃을 position으로 구분 지어 제작하였습니다.
모션 : css3의 rotate를 이용하여 반응형으로 되었을때 180도나 360도로 회전하는등 여러가지 모션을 걸어보았습니다.
반응형: pc버전 , 태블릿버전, moblie 버전 3가지로 미디어쿼리를 사용해 제작 하였습니다.



#####  [WALKERHILL](https://github.com/seokhwanmyeong/WALKERHILL)

기존의 WALKERHILL를 리모델링한 사이트입니다.

디자인컨셉: 호텔 예약 사이트

-개발과정 -
레이아웃 : position을 사용한 색다른 레이아웃 사이트를 구성,제작해 보았습니다.
메뉴 communiny , 워커힐 리워즈 가입부분을 눌러보면 회원가입,게시판 테이블을 직적 작성하였습니다.
모션: css3의 rotate를 이용하여 반응형으로 되었을때 180도나 360도로 회전하는등 여러가지 모션을 걸어보았습니다.
반응형 : pc버전 , 태블릿버전, moblie 버전 3가지로 미디어쿼리를 사용해 제작 하였습니다.



###  Ajax

-Ajax 연동-
url : target, beforeSend : function(){ console.log("데이터 불러오기전까지 이구문이 실행") },
success : function(data){ console.log(data); $(".showBox").html(data); },
error : function(){ }
데이터를 불러오기 전까지 실행할 구문,데이터가 성공적으로 불러와지면 실행할 구문,데이터 불러오기 실패구문로 나뉘어
한 index.html 안에 10개의 html페이지를 불러오기 하였습니다.



### showbox

-레이아웃-
웹접근성 요소에서 시각장애인들은 태그를 위에서부터 차례대로 읽어야하는데 float으로 제작할시 gnb같은 우선순위가 높은 태그들을 위에 쓸수 
없는 부작용이 있는것 같아서 모든 레이아웃을 position으로 구분 지어 제작하였습니다.
sub 페이지가 많아 header,footer부분은 php구문의 include을 사용하여 공통되게 제작하였습니다.

-모션-
global navigation , slide , setinterval , 자주쓰이는 tab 메뉴 등 거의 모든 모션들을 플로그인을
사용하지않고 제이쿼리를 사용하여 직접 로직을짜서 제작하였습니다. 웹 접근성 : 이미지에 alt값 , a태그에 title값 , 모든테이블에 summary, caption, form태그에 fieldset,legned, input 태그에 label for, id연결, 모든 페이지마다 skip naigation 적용, 모든 버튼은 a 태그로 코딩, -reset.css에서 a태그에 outline:1적용 -스킵네비, gnb, 슬라이더, 탭메뉴 (포커스이동구현)으로 최대한 접근성에 맞게 제작 하였습니다. 반응형: pc버전 , 태블릿버전, moblie 버전 3가지로 미디어쿼리를 사용해 제작 하였습니다.

-느낀점-
함수를 작성하고 매개변수를 통한 통로로 이동시켜야하는데, 매개변수의 개념과 전역변수와의차이, 서로 쓰이는 상황들이 어떻게 쓰이는지 어려웠습니다. 또, 제이쿼리 선언 방법의 여러 방법 gnb navigation 제작할때 slideToggle을 사용하였는데 왜 제이쿼리 stop()메소드에 ture,ture을 넣어야하는지,
큐에 쌓여서 대기중이던 애니메이션 효과들이 제거되서 사용되지 않는다고 해서 중복되지 않는다고 하는데..
이런등이 제작하면서 여러가지 어려움이 많았습니다.

-- 신입 포폴 준비할때라, 지금은 슬라이드기능과 게시판기능이 작동하지 않습니다. 추후에 추가 하도록 하겠습니다. --


