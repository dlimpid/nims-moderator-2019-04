# 국가수리과학연구소 산업수학 모더레이터 역량강화 프로그램 - NumPy, Matplotlib, and Pandas 튜토리얼

[SciPy 2018 Conference](https://scipy2018.scipy.org/ehome/index.php?eventid=299527)의 세 튜토리얼

- Introduction to Numerical Computing with NumPy([강의 자료(GitHub 저장소)](https://github.com/enthought/Numpy-Tutorial-SciPyConf-2018), [강의 영상](https://youtu.be/V0D2mhVt7NE))
- Pandas .head() to .tail()([강의 자료(GitHub 저장소)](https://github.com/deniederhut/Pandas-Tutorial-SciPyConf-2018), [강의 영상](https://youtu.be/lkLl_QKLgcA))
- Anatomy of Matplotlib([강의 자료(GitHub 저장소)](https://github.com/matplotlib/AnatomyOfMatplotlib), [강의 영상](https://youtu.be/6gdNUDs6QPc))

을 한꺼번에 리뷰하는 튜토리얼의 자료 저장소입니다.

- NumPy 튜토리얼은 미리 작성된 Jupyter notebook이 없고, 슬라이드는 GitHub 저장소에서 찾으실 수 있습니다.
- Pandas와 Matplotlib 튜토리얼의 자료 중 일부를 수정하여 이 저장소에 올려 두었습니다.

## 계산 환경 만들기

Conda를 이용해 Jupyter를 사용한 계산 환경을 만들어서 수요일, 목요일 두 튜토리얼 세션에 같이 사용합니다.

**설치하는 데에 시간이 걸리므로 반드시 사전에 설치해 주세요.**
**가능한 한 로컬에 계산 환경을 세팅해서 오실 것을 추천합니다.**

### 로컬에 만들기

#### 1. Miniconda 설치

이미 Anaconda나 Miniconda를 설치하신 경우 2번으로 넘어가시면 됩니다.

[Miniconda](https://docs.conda.io/en/latest/miniconda.html) 페이지에서 맞는 설치 파일을 다운받아 설치합니다.

:warning: 만약 본인의 Windows 계정 이름이 한글이어서 `%USERPROFILE%` 경로가 "C:\\Users\\홍길동"과 같이 한글이 포함되어 있는 경우 제대로 동작하지 않을 수 있으니, 기본 옵션이 아닌 한글과 공백을 포함하지 않는 새로운 경로(예: C:\\opt\\Miniconda 등)에 설치하세요.

#### 2. 환경 만들기

[이 저장소의 environment.yml](TODO) 파일을 다운받습니다.
Anaconda/Miniconda prompt를 실행한 후 파일을 다운받은 위치에서

```shell
conda env create
```

라고 하시면 `moderator-tutorial`이라는 환경이 만들어집니다.

#### 3. 환경 활성화하기

```shell
conda activate moderator-tutorial
```

활성화한 후에 명령줄에 `(moderator-training)`이 보이는지 확인해 보세요.

#### 4. 자료 다운받기

```shell
git clone [TODO: repo 주소 넣기]
```

#### 5. JupyterLab 실행하기

```shell
(moderator-training) $ jupyter lab
```

실행이 제대로 되지 않으면 3번으로 환경을 활성화했는지 다시 한 번 확인해 보세요.

### Binder 이용

:warning: 인터넷 접속이 불가능할 수 있으므로 가능한 한 로컬에 만들어 오시기를 추천합니다.

TODO: Binder link 넣기
