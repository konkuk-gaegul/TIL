# MATPLOT

역시 기본

import numpy as np

import pandas as pd

import matplotlib.pyplot as plt

import seaborn as sns

## 	시각화

1. 자료 분석의 기본은 통계와 그래프!
   - 통계는 수치를 통해 자료를 이해함
   - 그래프는 자료에 대한 직관적인 이해
2. 시각화 하는 방법은 정해져 있다.
   - 자료(변수)의 형태와 개수에 따라서, 그릴 수 있는 그래프는 결정되어 있다.
     - 1변수,  다변수(2변수 이상)
     - 통계에선 3변수 이상은 다루지 않는다.
     - 현재 빅데이터는 아주아주 많은 변수를 다룬다.

### 		matplot

1. 가장 기본적인 시각화 lib
2. 파이썬에서 제공하는 대부분의 시각화 lob들도 matplotlib를 기반으로 구현

### 		seaborn

1. matplotlib를 기반으로 만들어진 lib
2. 사용하기 쉽고, 예쁘게 만들어져있음
3. 주로, 자료의 시각화에 많이 사용

### 		plotly

1. 장점은...예쁘고 사용하기 편하다. 특히 3차원 그릴때 편함



## 	한글화

1. matplotlib는 한글을 지원하지 않는다
2. 폰트 설정을 위한 라이브러리 임포트
   - from matplotlib import font_manager, rcParams
3. 한글 표현이 가능한 폰트를 설치
   - !apt-get install fonts-nanum*

4. 폰트 확인하고 고르기
   - font_manager.findSystemFonts(fontext='ttf')
5. 폰트를 변경
   - rcParams[ 'font.family'] = 'NanumGothic'
6. '-' 부호깨져서 나오기 때문에 같이 설정
   - rcParams[ 'axes.unicode_minus'] = False
   - font_manager._rebuild()
7. 위의 것들을 런타임 재시작 후 다시 실행





































