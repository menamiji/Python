# 1. 라이브러리 설정
## 1-1. 한글폰트 설치
```
!sudo apt-get install -y fonts-nanum
!sudo fc-cache -fv
!rm ~/.cache/matplotlib -rf
```
- [런타임] > [런타임 다시시작] 

## 1-2. matplotlib 설치
- 파이썬에서 데이터 시각화를 위해 사용되는 라이브러리.
- matplotlib을 사용하면 그래프나 차트 등 다양한 형태의 데이터 시각화를 쉽게 만들 수 있음.

```
import matplotlib.pyplot as plt
plt.rc('font', family='NanumBarunGothic')
```

## 1-3. Pandas 설치
- 판다스는 파이썬으로 데이터를 처리하기 위한 라이브러리로 데이터 분석을 위한 효율적인 데이터 형식을 제공
```
import pandas as pd
```

### - CSV 파일 불러오기
- 판다스 read_csv()함수를 이용해 CSV 파일을 읽어와 데이터 프레임으로 변환

- **데이터프레임(DataFrame) :** 2차원 배열 형태의 데이터 구조

|컬럼1|컬럼2|컬럼3|   
|----|-----|----|  
|내용|내용2|내용3|
|내용|내용2|내용3|

- 아래와 같은 형식으로 CSV 파일을 불러올 수 있음
```
pandas.DataFrame(2차원 배열, index = 행 인덱스 배열, columns = 열 이름 배열)
```

# 2. 구글 드라이브 연결
```
from google.colab import drive
drive.mount('/content/drive')
```
- [google drive에 연결] > [엑세스 허용]