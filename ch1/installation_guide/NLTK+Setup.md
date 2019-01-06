 
# 파이썬, pip, NLTK 설치

# NLTK를 Linux Ubuntu 14.04 에 설치합니다.(추천)



```python
import sys
sys.version
sys.version_info 2_Python
```




    sys.version_info(major=2, minor=7, micro=6, releaselevel='final', serial=0)


```

Ubuntu 14.04에 파이썬을 설치

이 버전의 Ubuntu 시스템은 python 2.7.x버전을 이미 내장하며 따로 설치할 필요가 없습니다.


파이썬이 제대로 설치되었는지 확인하려면 다음 단계를 따르십시오.

Step 1: 시스템 터미널을 실행합니다.
Step 2: 아래 내용을 입력해 파이썬 버전을 확인합니다.
$ python -V
Python 2.7.6

```


```

Linux Ubuntu 14.04에 pip와 setup tools를 설치


pip가 무엇인가요?
pip는 Python으로 작성된 소프트웨어 패키지를 설치하고 관리하는 데 사용되는 패키지 관리 시스템 입니다.

시스템 터미널을 실행해 다음 명령을 실행합니다.

$ sudo apt-get install -y python-pip
$ sudo pip install -U pip
$ sudo pip install setuptools==33.1.1

pip가 성공적으로 설치되었는지 아래 입력으로 확인합니다.

$ pip -V
pip 9.0.1 from /usr/local/lib/python2.7/dist-packages (python 2.7)Next step is to install nltk package and download nltk data
```


```


NLTK 설치 단계 

시스템 터미널을 실행해 다음 명령을 실행합니다.
$ sudo pip install nltk
$ pythonAfter this now you are inside the python shell and check your nltk package install properly or not

$ python
Python 2.7.6 (default, Oct 26 2016, 20:30:19) 
[GCC 4.8.4] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>>import nltk
>>>nltk.download()


nltk data를 원하는 경로를 선택하고 Download 옵션을 클릭합니다.

다운로드 과정이 조금 오래 걸릴 수 있습니다.
1장의 그림1.4를 참조해 주세요.

또는 

파이썬 Shell에서의 과정을 원하지 않는다면, 아래 명령어로 진행할 수 있습니다.
Command : sudo python -m nltk.downloader -d PATH_OF_NLTK_DATA all
Actual command : sudo python -m nltk.downloader -d /usr/local/share/nltk_data all



```
