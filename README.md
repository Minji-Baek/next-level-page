# next-level-page
이때까지 터득한 animation, parallax-scrolling, css 기법들을 활용하고 또 다른 기법들을 사용하여 interactive page 를 만들어본다.


## 이론

  ### JAVASCRIPT 
    - setInterval()
      ex) let interval = setInterval(myfuncm, 10000); clearInterval(interval);
      -- 특정 간격의 시간에 맞춰 반복하여 특정 함수를 동작하게 함
      -- interval의 동작을 멈추려면 clearInterval() 함수 사용
      -- js native 함수 (확장성, 범용성이 좋음)
      -- 엄밀한 시간 정확도를 보장하지 않음, (정확히 1초마다 돌진 않음)
         브라우저와 컴퓨터 성능에 따라서도 다를 수 있음
      -- setTimeout 과 조합하여 시간 흐름에 따른 함수 실행을 만들기도 함

    - setTimeout
      -- set 밀리초 이후에 딱 한번 set된 함수가 실행된다.
      -- 의도된 지연을 야기할 때

    - intersectionObserver API ?
      -- 요소가 유저의 뷰포트에 들어왔는지, 숨겨졌는지 탐지
      -- 지연 로딩 이미지, 애니메이션 발동, 유저의 활동 추적 등에 용이
      -- 요소가 화면에 들어오거나 나갈때 실행될 콜백 함수를 넘겨 객체를 만듬
      -- 관찰하고 싶은 요소를 인자로, intersectionObserver 객체의 observe 메소드를 호출하여 관찰을 시작
      -- 콜백함수의 단일 인자인 entries(요소의 노출 정도, 위치, 크기 등 포함)로 필요한 정볼르 얻는다. 배열 형태임
