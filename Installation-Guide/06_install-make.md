# **MTA 모듈 설치**

## Change Log

### - 2020-06-25
  - INIT

---

## **Introduction**
MTA를 빌드하기 위해서는 먼저 `make` 명령어를 사용해야 합니다.  
아래의 방법으로 `make`를 설치합니다.

## **1. chocolatey - 윈도우 패키지 관리자 설치**

chocolatey 공식 링크 : [https://chocolatey.org](https://chocolatey.org)

chocolaty은 윈도우에서 사용하는 패키지 관리자 입니다.  
설치 하실 때 관리자로 설치를 하셔야 제대로 설치가 되므로 마우스 오른쪽 버튼을 클릭하여 관리자 모드로 실행하시기 바랍니다.  
윈도우 기본 프로그램은 아니고 다음과 같은 명령을 통해 설치해야 합니다.  

```bash
@powershell -NoProfile -ExecutionPolicy unrestricted -Command "iex ((new-object net.webclient).DownloadString('https://chocolatey.org/install.ps1'))" && SET PATH=%PATH%;%systemdrive%\chocolatey\bin
```

설치가 되면 명령 프롬프트에서 명령을 통해 프로그램을 설치 할 수 있습니다.

- make 설치 명령어

```
choco install make
```

> ### **make란?**  
> SHELL에서 컴파일을 해보셨다면, make 명령어로 compile을 실행하는 경우를 자주 보셨을 것입니다.  
> Makefile이 있는 디렉토리에서 make 만 치면 compile이 실행된다?? 어떻게 이런 일이 일어날 수 있는 것일까요?  
> 왜냐하면 make는 파일 관리 유틸리티 이기 때문이지요.  
> 파일 간의 종속관계를 파악하여 Makefile( 기술파일 )에 적힌 대로 컴파일러에 명령하여 SHELL 명령이 순차적으로 실행될 수 있게 합니다.