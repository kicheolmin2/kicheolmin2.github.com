---
layout: post
category : AVR
title: lesson1 - AVR introduction
date: 2014-10-24 17:25:06 -0700
tags : [AVR, ATmega]
---

##**Atmel AVR**

**아트멜 AVR(Atmel AVR)**은 1996년 아트멜 사에서 개발된 하버드 구조로 수정한 8비트 RISC 단일칩 마이크로컨트롤러이다. 출시 당시 AVR은 프로그램을 저장하기 위해 이용한 메모리 방식을 다른 마이크로컨트롤러 처럼 ROM, EPROM 또는 EEPROM 을 사용하지 않고, 단일칩 플래시메모리를 사용한 최초의 마이크로컨트롤러중 하나이다.

<img class="irc_mi" style="margin-top: 20px;" src="http://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/ATmega8_01_Pengo.jpg/220px-ATmega8_01_Pengo.jpg" width="400" height="502">

##**AVR의 구성**

AVR은 `중앙처리장치`와 `소용량 플래시메모리`가 하나의 IC에 집적되어 있다.
AVR 하버드구조(Harvard architecture)의 변형형태로 `프로그램과 데이터 메모리가 분리`된 형태이다. 
특수 명령어로 프로그램 데이터를 데이터 영역으로 읽을 수 있다.

##**AVR의 종류**

아트멜 AVR은 AVR UC3, AVR XMEGA, megaAVR, tinyAVR 시리즈 등이 있으며, 그 중 `ATmega128`이 교육용으로 가장 흔하게 쓰인다.

##**기본적인 AVR 계열**
AVR은 6개의 기본 모둠으로 되어있다.

###**tinyAVR** - ATtiny 시리즈
    0.5 - 16 kB 프로그램 메모리
    6-32핀 패키지
    제한된 주변 장치(peripheral) 세트

###**megaAVR** - ATmega 시리즈
    4 - 512 kB 프로그램 메모리
    28 - 100핀 패키지
    확장된 `명령어 집합` (곱셈 명령어, 큰 프로그램 메모리를 처리를 위한 명령어)
    확장된 주변 장치(periheral) 세트
    
###**XMEGA** - ATxmega 시리즈
    16 - 384 kB 프로그램 메모리
    44-64-100핀 패키지 (A4, A3, A1)
    확장된 성능 (DMA, "Event System", 암호와 지원)
    확장된 주변 장치(peripheral) 세트 (ADC)

###**Application-specific AVR**
    megaAVR을 기반으로 다른 AVR 계열에서 찾을 수 없는 LCD 제어, USB 제어, 진화된 PWM, CAN, 등의 모듈 추가.
    
###**FPSLIC (AVR에 FPGA 추가)**
    FPGA 5K ~ 40K 게이트
    다른 AVR과는 달리, AVR 프로그램 코드를 SRAM에
    AVR 코어는 50 MHz 이상에서도 실행
    
###**32-bit AVRs**
    2006년에 Atmel은 32비트를 기반으로 `AVR32` 구조를 만들었다. SIMD와 DSP 명령어를 추가하여 오디오와
    비디오 처리를 할 수 있다. 32비트 계열은 ARM과 경쟁 관계에 있다. 명령어 집합은 다른 RISC와 비슷하지만
    원래 AVR이나 다양한 ARM 코어와 호환되지 않는다.
    
##**프로그래밍 인터페이스**

AVR 칩에 프로그램 코드는 여러가지 방법으로 전송할 수 있다.

###**ISP**
<img class="irc_mi" style="margin-top: 20px;" src="http://upload.wikimedia.org/wikipedia/commons/thumb/9/9f/Isp_headers.svg/220px-Isp_headers.svg.png" width="400" height="502">

ISP(in-system programming) 프로그램 전송 방식은 기능적으로 SPI 방법에 Reset 선을 추가한 것이다. PCB에 납땜 상태에서 프로그램 코드를 전송할 수 있다. AVR에서 가장 일반적인 방법이다.
Atmel AVR ISP mkII 장치는 USB에 연결하고 Atmel의 ISP 프로그램에 의해 동작한다.
AVRDUDE (AVR Downloader/UploaDEr)는 Linux, FreeBSD, 윈도, OS X에서 실행되면 다양한 하드웨어(Atmel AVR ISP mkII, Atmel JTAG ICE)로 프로그래밍을 할 수 있다.
