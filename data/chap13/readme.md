# 13장. 오토인코더 : 엠니스트 이미지 재현 및 분류 신경망
13장에서는 예제 실습을 위해 대표적인 필기체 숫자 이미지 데이터셋인 MNIST 데이터셋 파일들을 이용합니다.<br/>
MNIST 데이터셋 파일들은 여러 연구 사이트에서 제공되며 직접 다운로드 받아야 합니다.<br/>

## 얀 교수의 홈페이지에서 MNIST 데이터셋 다운받기
깃허브 용량 관계상 MNIST 데이터셋은 여기 수록하지 못하며 따라서 사용자별로 각자 다운로드받아야 합니다.<br/><br/>
MNIST 데이터셋은 여러 곳에서 다운받을 수 있으며 그 중 한 곳이 뉴욕 대 얀리춘(Yann LeCun) 교수의 개인 홈페이지입니다.
이 홈페이지에서 MNIST 데이터셋을 소개하는 페이지의 접근 경로는 http://yann.lecun.com/exdb/mnist/ 입니다.<br/>
이 페이지에는 압축파일을 다운로드받을 수 있는 링크 네 개가 있습니다. 이 가운데 현재 예제 실습에필요한 파일은 train-images-idx3-ubyte.gz 파일과 
train-labels-idx1-ubyte.gz 파일의 두 개입니다.
두 파일을 다운받아 압축을 풀면 각각 하나의 파일만 만들어지는데 이들 두 파일을 /data/chap13/mnist 폴더에 배치하면 실험 준비가 끝납니다.
참고로 테스트 데이터를 제공하는 다른 두 파일은 내용이 많지 않아 이용을 하지 않고 있지만 프로그램을 조금 확장한다면 함께 이용할 수 있을 것입니다.

## 주의사항
얀 교수 홈페이지에서 다운받은 파일의 압축을 풀면 파일 이름이 train-images.idx3-ubyte, train-labels.idx1-ubyte로 생성되는 경우가 있습니다.
이런 경우 파일명을 train-images-idx3-ubyte, train-labels-idx1-ubyte로 수정해 주세요.

깃허브 용량 관계상 MNIST 데이터셋은 여기 수록하지 못하며 따라서 사용자별로 각자 다운로드받아야 합니다.<br/><br/>
## 13장에서 이용하는 데이터 파일
/data/chap13/mnist/train-images-idx3-ubyte : 총 1 파일, 47MB<br/>
/data/chap13/mnist/train-labels-idx1-ubyte : 총 1 파일, 6.0KB<br/>
