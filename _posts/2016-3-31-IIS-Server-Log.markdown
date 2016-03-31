---
layout: post
title:  "IIS Server Log"
date:   2016-3-31 15:00:00
categories: jekyll update
---


**IIS Server Log** 
Posted on 2016-3-31 by juddammu

IIS 서버를 처음 접하다 보니 로그가 어디에 쌓이고 있는지 확인할 필요가 있었다.

>**%SystemDrive%\inetpub\logs\LogFiles**

여기서  **%SystemDrive%** 는 **C 드라이브**를 말한다.

IIS(인터넷 정보서비스)관리자 에서 자신의 서버를 선택하면 서버 홈에

**'로깅'** 이 있다. 선택하여 들어가면 로그파일에 대해 설정할 수 있다.

로그 이벤트 대상을 아래와 같다.

- 로그 파일만(L)
- ETW 이벤트만(T)
- 로그 파일과 ETW 이벤트 모두(A)

default 로 로그 파일만이 선택 되어 있었는데,  보안이슈로 인해서

로그 파일과 ETW 이벤트 모드 쌓도록 설정하였다.

ETW는 **Event Tracing for Windows** 즉 윈도우를 위한 이벤트 추적 이라고 한다. 

<img src="../data/img/iis_server_log.PNG" align=left>