# next-level-page
이때까지 배운 animation, parallax-scrolling, css 기법들을 활용하고 또 다른 기법들을 사용하여 interactive page 를 만들어본다.


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