# keras_cnn_mnist_kor
한글로 된 keras를 이용한 cnn-mnist 데모입니다. 

# Convolutional Neural Network, MNIST DEMO

> 본 데모는 CNN을 쉽게 돌려볼 수 있는 교육용 자료로서, 김인식(insik92@gmail.com)에 의해 작성되었습니다.


MNIST는 손으로 쓴 숫자가 있는 이미지 데이터셋입니다.

Convolutional Neural Network (이하, CNN)은 Neural Network의 한 종류입니다.

CNN model을 이용하여 손글씨 숫자를 분류하는 분류기를 만들어 봅니다.

자세한 설명은 다음 블로그를 참고해보세요. 

> (Part 4) Keras 설치 & MNIST 예제 실행
> http://blog.daum.net/goodgodgd/22


## 준비사항
본 DEMO를 실행시켜보기 위해서는 아래의 준비사항들을 모두 완료해야 합니다. 각각에 대해 잘 모르겠으면 순서대로 진행해주시면 됩니다.

* python2
> 간편설치를 위해, anaconda python을 설치하세요. https://www.continuum.io/downloads

* g++ compiler
> MinGW를 설치하세요. anaconda python을 설치했다면 cmd를 키고 다음 명령을 실행합니다. "conda install mingw libpython"
>
> MinGW의 경로를 시스템 환경변수에 추가하세요. 예) C:\Users\USERNAME\Anaconda2\MinGW
>
> USERNAME에 윈도우 사용자 이름을 입력하세요. 
> 
> 주의: 아나콘다를 쓰지 않고 직접 설치할 때 64bit윈도우에는 MinGW64를 설치해야 합니다.

* python theano package
> https://github.com/Theano/Theano 에 들어가 Download Zip 클릭
>
> 압축 풀고 해당 디렉토리에 들어가 cmd를 키고 python setup.py develop 명령을 실행
>
> 자세한 사항은 http://deeplearning.net/software/theano/install.html#bleeding-edge-install-instructions 참고

* python keras package
> cmd를 열고 pip install keras 명령을 실행

* 혹시 다른 python package가 필요한 경우 다음 명령을 실행하세요
> pip install PACKAGENAME
>
> 예) pip install pandas
> 
> 예2) pip install h5py

* 또 다른 설치 참고 링크: http://stackoverflow.com/questions/34097988/how-to-install-keras-and-theano-in-anaconda-python-2-7-in-windows