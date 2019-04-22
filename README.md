# 국가수리과학연구소 산업수학 모더레이터 역량강화 프로그램

## 계산 환경 만들기

Conda를 이용해 Jupyter를 사용한 계산 환경을 만들어서 수요일, 목요일 두 튜토리얼 세션에 같이 사용합니다.

**설치하는 데에 시간이 걸리므로 반드시 사전에 설치해 주세요.**
**무선 인터넷 환경이 좋지 않으므로 꼭 미리 설치해 오셔서 로컬 계산 환경을 사용하실 것을 추천합니다.**

### 1. Miniconda 설치

이미 Anaconda나 Miniconda를 설치하신 경우 2번으로 넘어가시면 됩니다.

[Miniconda](https://docs.conda.io/en/latest/miniconda.html) 페이지에서 맞는 설치 파일을 다운받아 설치합니다.

:warning: 만약 본인의 Windows 계정 이름이 한글이어서 `%USERPROFILE%` 경로가 "C:\\Users\\홍길동"과 같이 한글이 포함되어 있는 경우 제대로 동작하지 않을 수 있으니, 기본 옵션이 아닌 한글과 공백을 포함하지 않는 새로운 경로(예: C:\\opt\\Miniconda 등)에 설치하세요.

Windows의 경우 아래부터는 일반 명령 프롬프트(cmd)나 PowerShell이 아닌 Anaconda/Miniconda Prompt를 이용해야 합니다.

### [선택사항] Conda 업데이트

```shell
conda update -n base -c defaults conda
```

### 2. 환경 만들기

[이 저장소를 다운로드](https://github.com/dlimpid/nims-moderator-2019-04/archive/master.zip)해서 적당한 위치(주로 사용자 홈 디렉터리)에 압축을 풉니다.
Git이 이미 설치되어 있고 익숙하시면

```shell
git clone https://github.com/dlimpid/nims-moderator-2019-04.git
```

을 실행하셔도 됩니다.

Anaconda/Miniconda prompt를 실행한 후 파일을 다운받은 디렉터리에서

```shell
conda env create
```

라고 하시면 `moderator-tutorial`이라는 환경이 만들어집니다.

### 3. 환경 활성화하기

```shell
conda activate moderator-tutorial
```

:exclamation: 활성화한 후에 명령줄에 `(moderator-training)`이 보이는지 확인해 보세요.

### 4. JupyterLab 실행하기

```shell
jupyter lab
```

실행이 제대로 되지 않으면 3번으로 환경을 활성화했는지 다시 한 번 확인해 보세요.

### 5. 동작 확인

JupyterLab에서 check_env.ipynb 파일을 열고 Run -> Run All Cells를 클릭해 모든 패키지가 import되고, 그래프도 잘 나오는지 확인합니다.

## Binder 이용

:warning: 인터넷 접속이 불가능할 수 있으므로 가능한 한 로컬에 만들어 오시기를 추천합니다.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dlimpid/nims-moderator-2019-04/master?urlpath=lab)
