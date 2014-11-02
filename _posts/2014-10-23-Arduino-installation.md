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

<img class="irc_mi" style="margin-top: 20px;" src="https://lh6.googleusercontent.com/-IAsuDXNcsJc/VFZLUFq4iNI/AAAAAAAAAA4/W0WrXLJsc9Q/w743-h477-no/1.png" width="500" height="400">

### 2. 
빨간색으로 표시된 **Download** 로 들어가주세요.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh5.googleusercontent.com/-DPZ570l5CwM/VFZLWdKoixI/AAAAAAAAACk/7MEbtxNQsWw/w629-h432-no/2.png" width="500" height="400">

### 3.
다운로드 버튼을 누르거나, 다운로드 링크로 바로 접속하면 다음과 같은 창이 나타나는데, 스크롤을 내리면

<img class="irc_mi" style="margin-top: 20px;" src="https://lh4.googleusercontent.com/-lLheadBvPgw/VFZLWRZmS-I/AAAAAAAAACY/8lPnm81Q1bg/w528-h365-no/3.png" width="500" height="400">

### 4.
다음과 같은 부분이 나타납니다. 여기서 **Windows Installer** 나 **Windows ZIP file(for non-administrator install)** 둘 중 하나를 선택해서 다운로드 합니다.
저는 **Windows ZIP file(for non-administrator install)**을 다운받아서 진행하도록 하겠습니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh6.googleusercontent.com/-T4R52JKERdk/VFZLW97KkqI/AAAAAAAAAB0/VguBmfjLn18/w629-h275-no/4.png" width="500" height="400">

### 5.
압축 파일을 원하는 위치에 풀어줍니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh4.googleusercontent.com/-S94kFrGqMHk/VFZLXb0lFrI/AAAAAAAAAB4/3JBXTd6RZ8E/w629-h472-no/5.jpg" width="500" height="400">

### 6.
아두이노를 컴퓨터의 USB 포트에 연결합니다.
Windows Installer로 설치하거나, 이전에 드라이버가 설치되어 있다면 장치드라이버 소프트웨어가 자동으로 설치되지만
Windows ZIP file(for non-administrator install)을 통해 설치를 진행했다면 수동으로 드라이버를 설치해줘야 합니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh5.googleusercontent.com/-cIshgeNfQlI/VFZLXiSCZ_I/AAAAAAAAACE/PwQnB7QbPM8/w628-h292-no/6.png" width="500" height="400">

### 7.
드라이버 인식을 실패하신 분은 제어판 - 하드웨어 및 소리 - 장치 및 프린터로 가시면 '알 수 없는 장치'가 떠있습니다.
이 것이 아두이노이며, 수동으로 드라이버를 설치해주어야 합니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh4.googleusercontent.com/-g_CZyUW58Kk/VFZLYBdqKlI/AAAAAAAAACU/RhG4GKZwMHI/w479-h475-no/7.png" width="500" height="400">

### 8.
아이콘을 우클릭해서 속성을 누르면 **알 수 없는 장치 속성** 이라는 장치 속성창이 나타납니다.
들어가서 하드웨어 탭으로 들어간 후 속성버튼을 클릭합니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh5.googleusercontent.com/-35Lg8YuGaKU/VFZLYYyhqUI/AAAAAAAAACM/YmxB7eS6J9Y/w479-h430-no/8.png" width="500" height="400">

### 9.
설정 변경 버튼을 눌러줍니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh5.googleusercontent.com/-SUpOivE2RHo/VFZLYg7sSsI/AAAAAAAAACQ/RoAHpmVuyzA/w479-h430-no/9.png" width="500" height="400">

### 10.
방금과 같은 창으로 혼동할 수 있지만, 버튼이 다릅니다. 여기서 **드라이버 업데이트** 버튼을 눌러주세요. 

<img class="irc_mi" style="margin-top: 20px;" src="https://lh6.googleusercontent.com/-QGuBPnPFlbk/VFZLT5jBZmI/AAAAAAAAAAs/IqV8ilBG7CY/w629-h456-no/10.png" width="500" height="400">

### 11.
**컴퓨터에서 드라이버 소프트웨어 찾아보기**를 눌러줍니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh6.googleusercontent.com/-PIxw-M2gMx0/VFZLT-ydj0I/AAAAAAAAAAw/znXoZUmV0wc/w629-h456-no/11.png" width="500" height="400">

### 12.
찾아보기 단추를 눌러서 자신이 아두이노를 설치한 폴더 내의 drivers라는 폴더를 선택해줍니다.
그 후 다음 버튼을 눌러줍니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh6.googleusercontent.com/-UpPPNkI4Coc/VFZLUk6SGHI/AAAAAAAAABM/rHvxScOj-uo/w629-h456-no/12.png" width="500" height="400">

### 13.
설치 단추를 눌러줍니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh6.googleusercontent.com/-uLbqPL3Q2Vs/VFZLU-nq1AI/AAAAAAAAABk/0n__jfhPFpk/w628-h292-no/13.png" width="500" height="400">

### 14.
설치 후 다음과 같이 Arduino Uno(COM30)과 같이 이름이 나타난다면 정상적으로 드라이버가 설치된 것입니다.
여기서 `COM30`이라고 되어있는데 이 것은 포트번호입니다. 이는 나중에 아두이노로 프로그램을 전송할 때 사용하는 포트로
컴퓨터마다 다를 수 있으며, 잘 기억해 주시기 바랍니다.

### 15.
아두이노 설치폴더로 가서 arduino.exe 파일을 더블 클릭하면
<img class="irc_mi" style="margin-top: 20px;" src="https://lh5.googleusercontent.com/-Pi8_MZ933e8/VFZLVB4altI/AAAAAAAAABI/V0UIkvnI5Ww/w500-h600-no/14.png" width="500" height="400">
다음과 같은 창이 나타나며, 창이 뜨면 다음 코드를 띄어쓰기, 대문자 모두 구분하여 적어봅시다.

####코드
    void setup(){
    }
    
    void loop(){
    }

그리고 왼쪽 위의 **v** 표시 (체크 버튼)을 누릅니다. 이 버튼은 문법에 맞게 적었는지 체크하고 아두이노가 알 수 있는 코드로 번역하는 것입니다. 이 것을 **컴파일(Compile)** 이라고 합니다. 아두이노 프로그램에서는 **확인(check)** 라고 되어있습니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh6.googleusercontent.com/-AOzWw9wOla8/VFZLViUunlI/AAAAAAAAABU/59vgc9IN3Qs/w500-h603-no/15.png" width="500" height="400">

### 16.
`메뉴 - 도구 - 보드`에서 여러분이 가지고 있는 보드를, (저의 경우 Arduino Uno)
`메뉴 - 도구 - 시리얼포트`에서 제어판의 장치 및 프린터 창에서 확인했던 `COMxx` 번호를, (저의 설치과정에는 COM30)
을 설정해 줍니다.

그 후 이번엔 체크버튼 옆의 **화살표 버튼**을 눌러줍니다. 이 것은 아두이노로 코드를 업로드 하는 것입니다.

<img class="irc_mi" style="margin-top: 20px;" src="https://lh6.googleusercontent.com/-tZ0AoK-d6p4/VFZLV-Lf2aI/AAAAAAAAABg/tMh1G6yw6D0/w629-h472-no/16.jpg" width="500" height="400">

### 17.
업로드를 하면 아두이노의 Tx, Rx의 LED가 깜빡입니다. LED의 색깔은 다를 수 있습니다.
Tx : Transmitt라는 뜻으로 아두이노가 데이터를 전송하고 있다는 뜻
Rx : Recieve라는 뜻으로 아두이노가 데이터를 받고 있다는 뜻입니다.

업로드가 끝나면 Tx, Rx에 불이 꺼지고, 프로그램에는 `업로드 완료`라는 문구가 나타납니다.

아두이노에 아무 일도 안일어날텐데, 이는 제어하는 코드를 아무 것도 넣지 않았기 때문입니다.
C언어에서 만든 파일들을 `Project` 라고 부르는데, 아두이노에는 `프로젝트`대신에 `스케치`라는 말을 사용합니다.
이는 간단하게 할 수 있다는 의미를 가지고 있다고 **Massimo banzi**가 언급을 잠깐 했습니다.
위에서 만들었던 스케치는 `널 스케치`라고 하는데 이는 `0`이라고 생각하면 안되고, 공집합같은 개념이라 생각하면 됩니다.

다음 강의에서는 LED를 깜빡이는 예제를 분석하겠습니다
