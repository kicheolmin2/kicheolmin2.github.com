---
layout: post
category : lessons
title: lesson2 - LED Blink
date: 2014-10-24 16:25:06 -0700
tags : [Arduino, LED, blink, Scatch]
---

####**필요한 것**
    아두이노 보드(이번 강의에서는 **UNO R3**를 기준으로 함)
    브레드보드 & 전선
    저항 330옴(또는 220 ~ 1K옴) 1개
    LED 1개
    
####**선행학습**
    저항 읽는 법
    브레드보드 사용 법
    
이번 강의는 LED를 켜고 끄는 것을 제어하는 강의입니다.
먼저 다음 그림과 같이 회로를 구성해주세요.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh3.googleusercontent.com/-LCUy3w9ySW4/VFZPurV5wII/AAAAAAAAADQ/uOPnzjhG_OU/w496-h623-no/led1.png" width="400" height="502">

####**회로**
<img class="irc_mi" style="margin-top: 20px;" src="https://lh5.googleusercontent.com/-S6Ks1PWA5wc/VFZPumwjYaI/AAAAAAAAADE/mAkL4BMQccg/w555-h623-no/led2.png" width="400" height="450">

회로로 구성하면 다음과 같이 구성됩니다.
    
    D9 PWM -- 저항 -- LED -- GND
    
LED는 극성이 있기 때문에 연결할 때 방향을 확인해야 하는데, 다리가 긴 쪽이 `9번 핀 방향(+)`, 짧은 쪽이 `GND 방향(-)`을 가리키도록 해야합니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh5.googleusercontent.com/-fnffaq6NDgA/VFZPujDEqVI/AAAAAAAAADA/6SOJiOuaM9w/w500-h600-no/led3.png" width="400" height="450">

아두이노 프로그램으로 다음 코드를 대소문자를 구분하여 한 글자도 빼지 않고 적어야 합니다.
**(중괄호가 열려있을 때 엔터를 치면 자동으로 들여쓰기(`스페이즈 2칸`)가 적용됩니다. **

####**소스코드**
    int led = 9;
    
    void setup(){
      pinMode(led, OUTPUT);
    };
    
    void loop(){
      digitalWrite(led, HIGH);
      delay(1000);
      digitalWrite(led, LOW);
      delay(1000);
    }

이 후 아두이노 보드로 업로드합니다.

####**결과**
<iframe width="720" height="438" src="http://serviceapi.nmv.naver.com/flash/convertIframeTag.nhn?vid=D95EDE81AB92D7B133CF6ADFD10800810E81&outKey=V1278f1edd080349b692d977d5a4b782b337421e889b2d4ccecb6977d5a4b782b3374" frameborder="no" scrolling="no"></iframe>

####**소스코드 분석**
    int led = 9;                        // 변수 선언
    
    void setup(){                       // pinMode 선언, led를 output으로 설정, 
      pinMode(led, OUTPUT);             // 9로 설정되었므로 디지털9번이 output으로 설정됨
    };
    
    void loop(){                        // loop문, C언어에서는 for, while과 같은 역할
      digitalWrite(led, HIGH);          // 디지털쓰기 , 9번핀을 high로 설정
      delay(1000);                      // delay를 줌 (1000ms = 1s)
      digitalWrite(led, LOW);           // 디지털쓰기 , 9번핀을 low로 설정
      delay(1000);                      // delay를 줌 (1000ms = 1s)
    }

**시각을 밀리 초 단위로 기록하기 때문에 `long` 타입의 변수를 이용합니다. int 타입은 -32,768 ~ 32,767까지의 정수를 저장할 수 있는 변수 타입이고, long 타입은 4바이트 길이의 변수로 -2,147,483,648 ~ 2.147.483.647까지의 정수를 저장할 수 있는 변수 타입입니다.**
