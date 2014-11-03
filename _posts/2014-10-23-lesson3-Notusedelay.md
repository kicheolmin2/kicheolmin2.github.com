---
layout: post
category : lessons
title: lesson3 - LED Blink (Not use delay)
date: 2014-10-24 17:25:06 -0700
tags : [Arduino, LED, blink, delay]
---

####**필요한 것**
    아두이노 보드(이번 강의에서는 **UNO R3**를 기준으로 함)
    브레드보드 & 전선
    저항 330옴(또는 220 ~ 1K옴) 1개
    LED 1개
    
####**선행학습**
    Lesson2 - LED Blink
    
이번 강의는 LED Blink 예제와 결과는 동일하지만 내부적으로 시간 지연 함수 delay()를 사용하지 않습니다.
delay() 함수에 의하여 지연되는 동안에는 아두이노가 모든 입출력을 수행할 수 없기 때문에, 온도, 습도, 조도, 거리 등의 센서 입력을 받는 프로그램의 경우에는 문제가 발생할 수 있습니다.
따라서 LED를 동작시키면서 동시에 다른 센서 입출력이 필요한 경우에는 다음과 같이 delay() 함수를 사용하지 않는 코드로 변경시켜야 합니다.
LED 상태를 최종적으로 변경시킨 시각과 현재 시각을 계속 비교하여 지정한 시간 간격 이상이 되면 LED 상태를 변경시켜 ON, OFF 시키고 동시에 다른 입출력도 할 수 있도록 합니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh3.googleusercontent.com/-LCUy3w9ySW4/VFZPurV5wII/AAAAAAAAADQ/uOPnzjhG_OU/w496-h623-no/led1.png" width="400" height="502">

####**회로**
<img class="irc_mi" style="margin-top: 20px;" src="https://lh5.googleusercontent.com/-S6Ks1PWA5wc/VFZPumwjYaI/AAAAAAAAADE/mAkL4BMQccg/w555-h623-no/led2.png" width="400" height="450">

회로는 이전 강의 `Lesson2 - LED Blink`와 같습니다.
    
    D9 PWM -- 저항 -- LED -- GND
    
####**소스코드**
    int led = 9;
    
    `int ledState = LOW;`
    `long previousMillis = 0;`
    `long currentMillis = 0;`
    `long interval = 1000;`
    
    void setup(){
      pinMode(led, OUTPUT);
    };
    
    void loop(){
      `currentMillis = millis();`
      
      `if((currentMillis - previousMillis) > interval) {`
        `previousMillis = currentMillis;`
        `if(ledState == LOW){`
            `ledState = HIGH;`
        `}`
        `else {`
            `ledState = LOW;`
        `}`
        
        `digitalWrite(led, ledState);`
    }

`빨간색`으로 표시한 부분이 이전 강의에서 달라진 소스 부분입니다.

####**결과**
<iframe width="720" height="438" src="http://serviceapi.nmv.naver.com/flash/convertIframeTag.nhn?vid=D7AF6942C12570C76CF6F85F5DA177373136&outKey=V12751952c04ef203a2553eac689da638f98cc92c6f4b2d50fc4a3eac689da638f98c" frameborder="no" scrolling="no"></iframe>

####**소스코드 분석**
    int led = 9;                                          //9번 핀 사용을 위한 변수 선언
    
    `int ledState = LOW;`                                 //led의 상태를 저장해두는 변수
    `long previousMillis = 0;`                            //led 상태가 변경된 마지막 시간을 저장하는 변수, 밀리초 저장을 위한 long타입
    `long currentMillis = 0;`                             //현재 시각을 밀리 초 단위로 저장하는 변수
    `long interval = 1000;`                               //지연시킬 시간 입력 **delay(1000)**과 같음
    
    void setup(){
      pinMode(led, OUTPUT);                               //9번핀을 출력핀으로 설정
    };
    
    void loop(){                                      
      `currentMillis = millis();`                         //현재 시각을 밀리초 단위로 저장
      
      `if((currentMillis - previousMillis) > interval) {` //현재시각 - 이전설정시각 의 차이가 interval보다 크면
        `previousMillis = currentMillis;`                 //이전설정시각은 현재시각으로 설정하고
        `if(ledState == LOW){`                            //state가 LOW였다면
            `ledState = HIGH;`                            //HIGH로 변경
        `}`
        `else {`                                          //state가 HIGH였다면
            `ledState = LOW;`                             //LOW로 변경
        `}`
        
        `digitalWrite(led, ledState);`
    }
