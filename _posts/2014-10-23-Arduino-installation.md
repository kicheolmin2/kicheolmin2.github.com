---
layout: post
title: Arduino installation
categories: [Lessons]
tags: [install, arduino, setup]
fullview: true
---

## 아두이노 설치

이번 장은 아두이노 프로그램을 설치하는 장입니다.

**아두이노 공식 홈페이지** : <a href="http://www.arduino.cc" target="_blank">http://www.arduino.cc</a><br>
**다운로드 링크** : <a href="http://arduino.cc/en/Main/Software" target="_blank">http://arduino.cc/en/Main/Software</a><br>


### 1.
아두이노 공식홈페이지에 들어가면 다음과 같은 화면이 나타납니다.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles16.naver.net/20141025_255/vkdlsvnt_14141679949306C36A_PNG/%C4%B8%C3%B31.PNG?type=w2" width="500" height="400">

### 2. 
빨간색으로 표시된 **Download** 로 들어가주세요.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles14.naver.net/20141025_189/vkdlsvnt_1414168040112PfHEE_PNG/%C4%B8%C3%B32.PNG?type=w2" width="500" height="400">
### 3.
다운로드 버튼을 누르거나, 다운로드 링크로 바로 접속하면 다음과 같은 창이 나타나는데, 스크롤을 내리면

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles9.naver.net/20141025_136/vkdlsvnt_1414168040343cLwYa_PNG/%C4%B8%C3%B33.PNG?type=w2" width="500" height="400">
### 4.
다음과 같은 부분이 나타납니다. 여기서 **Windows Installer** 나 **Windows ZIP file(for non-administrator install)** 둘 중 하나를 선택해서 다운로드 합니다.
저는 **Windows ZIP file(for non-administrator install)**을 다운받아서 진행하도록 하겠습니다.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles3.naver.net/20141025_242/vkdlsvnt_1414168041049kldac_PNG/%C4%B8%C3%B34.PNG?type=w2" width="500" height="400">
### 5.
압축 파일을 원하는 위치에 풀어줍니다.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles13.naver.net/20141025_284/vkdlsvnt_1414168145044LCq2R_JPEG/IMG_2218.JPG?type=w2" width="500" height="400">
### 6.
아두이노를 컴퓨터의 USB 포트에 연결합니다.
Windows Installer로 설치하거나, 이전에 드라이버가 설치되어 있다면 장치드라이버 소프트웨어가 자동으로 설치되지만
Windows ZIP file(for non-administrator install)을 통해 설치를 진행했다면 수동으로 드라이버를 설치해줘야 합니다.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles10.naver.net/20141025_41/vkdlsvnt_1414168041522VeSRG_PNG/%C4%B8%C3%B36.PNG?type=w2" width="500" height="400">
### 7.
드라이버 인식을 실패하신 분은 제어판 - 하드웨어 및 소리 - 장치 및 프린터로 가시면 '알 수 없는 장치'가 떠있습니다.
이 것이 아두이노이며, 수동으로 드라이버를 설치해주어야 합니다.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles14.naver.net/20141025_125/vkdlsvnt_1414168041766uoJeT_PNG/%C4%B8%C3%B37.PNG?type=w2" width="500" height="400">
### 8.
아이콘을 우클릭해서 속성을 누르면 **알 수 없는 장치 속성** 이라는 장치 속성창이 나타납니다.
들어가서 하드웨어 탭으로 들어간 후 속성버튼을 클릭합니다.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles7.naver.net/20141025_70/vkdlsvnt_1414168042044xgBvH_PNG/%C4%B8%C3%B38.PNG?type=w2" width="500" height="400">
### 9.
설정 변경 버튼을 눌러줍니다.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles6.naver.net/20141025_149/vkdlsvnt_1414168042247kThYc_PNG/%C4%B8%C3%B39.PNG?type=w2" width="500" height="400">
### 10.
방금과 같은 창으로 혼동할 수 있지만, 버튼이 다릅니다. 여기서 **드라이버 업데이트** 버튼을 눌러주세요. 

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles10.naver.net/20141025_297/vkdlsvnt_1414168042494ezcw2_PNG/%C4%B8%C3%B310.PNG?type=w2" width="500" height="400">
### 11.
**컴퓨터에서 드라이버 소프트웨어 찾아보기**를 눌러줍니다.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles11.naver.net/20141025_154/vkdlsvnt_14141680426868gQVY_PNG/%C4%B8%C3%B311.PNG?type=w2" width="500" height="400">
### 12.
찾아보기 단추를 눌러서 자신이 아두이노를 설치한 폴더 내의 drivers라는 폴더를 선택해줍니다.
그 후 다음 버튼을 눌러줍니다.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles8.naver.net/20141025_55/vkdlsvnt_1414168042931KONJY_PNG/%C4%B8%C3%B312.PNG?type=w2" width="500" height="400">
### 13.
설치 단추를 눌러줍니다.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles13.naver.net/20141025_108/vkdlsvnt_1414168043133nv7HI_PNG/%C4%B8%C3%B313.PNG?type=w2" width="500" height="400">
### 14.
설치 후 다음과 같이 Arduino Uno(COM30)과 같이 이름이 나타난다면 정상적으로 드라이버가 설치된 것입니다.
여기서 COM30이라고 되어있는데 이 것은 포트번호입니다. 이는 나중에 아두이노로 프로그램을 전송할 때 사용하는 포트로
컴퓨터마다 다를 수 있으며, 잘 기억해 주시기 바랍니다.

### 15.
아두이노 설치폴더로 가서 arduino.exe 파일을 더블 클릭하면
<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles12.naver.net/20141025_235/vkdlsvnt_1414168043584VRXiE_PNG/%C4%B8%C3%B315.PNG?type=w2" width="500" height="400">
다음과 같은 창이 나타나며, 창이 뜨면 다음 코드를 띄어쓰기, 대문자 모두 구분하여 적어봅시다.

####코드
    void setup(){
    }
    
    void loop(){
    }

그리고 왼쪽 위의 **v** 표시 (체크 버튼)을 누릅니다. 이 버튼은 문법에 맞게 적었는지 체크하고 아두이노가 알 수 있는 코드로 번역하는 것입니다. 이 것을 **컴파일(Compile)** 이라고 합니다. 아두이노 프로그램에서는 **확인(check)** 라고 되어있습니다.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles7.naver.net/20141025_38/vkdlsvnt_1414168043788PQAms_PNG/%C4%B8%C3%B316.PNG?type=w2" width="500" height="400">
### 16.
_메뉴 - 도구 - 보드_에서 여러분이 가지고 있는 보드를, (저의 경우 Arduino Uno)
_메뉴 - 도구 - 시리얼포트_에서 제어판의 장치 및 프린터 창에서 확인했던 _COMxx_ 번호를, (저의 설치과정에는 COM30)
을 설정해 줍니다.

그 후 이번엔 체크버튼 옆의 **화살표 버튼**을 눌러줍니다. 이 것은 아두이노로 코드를 업로드 하는 것입니다.

<img class="irc_mi" style="margin-top: 20px;" src="http://postfiles13.naver.net/20141025_220/vkdlsvnt_1414169381095toqfa_JPEG/IMG_2220.JPG?type=w2" width="500" height="400">
### 17.
업로드를 하면 아두이노의 Tx, Rx의 LED가 깜빡입니다. LED의 색깔은 다를 수 있습니다.
Tx : Transmitt라는 뜻으로 아두이노가 데이터를 전송하고 있다는 뜻
Rx : Recieve라는 뜻으로 아두이노가 데이터를 받고 있다는 뜻입니다.

업로드가 끝나면 Tx, Rx에 불이 꺼지고, 프로그램에는 _업로드 완료_라는 문구가 나타납니다.

아두이노에 아무 일도 안일어날텐데, 이는 제어하는 코드를 아무 것도 넣지 않았기 때문입니다.
C언어에서 만든 파일들을 _Project_ 라고 부르는데, 아두이노에는 _프로젝트_대신에 _스케치_라는 말을 사용합니다.
이는 간단하게 할 수 있다는 의미를 가지고 있다고 **Massimo banzi**가 언급을 잠깐 했습니다.
위에서 만들었던 스케치는 _널 스케치_라고 하는데 이는 _0_이라고 생각하면 안되고, 공집합같은 개념이라 생각하면 됩니다.

다음 강의에서는 LED를 깜빡이는 예제를 분석하겠습니다.
