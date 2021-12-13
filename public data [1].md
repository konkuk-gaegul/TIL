# 공공데이터

공공데이터 포털에서 제공됨

유니코드 디코드 에러 = UTF-8이 아니라서 그럼. 엑셀에서 열린 걸로 이미 에러..

해결법은 인코딩! encoding = 'cp949' 추가!

tmp2 = pd.read_csv('/content/drive/MyDrive/data/population/201101_201312_주민등록인구기타현황(출생등록)_birth.csv', encoding='cp949')

tmp2

tmp3 = pd.read_csv('/content/drive/MyDrive/data/population/201401_201612_주민등록인구기타현황(출생등록)_birth.csv', encoding='cp949')

tmp3

tmp4 = pd.read_csv('/content/drive/MyDrive/data/population/201701_201912_주민등록인구기타현황(출생등록)_birth.csv', encoding='cp949')

tmp4

tmp5 = pd.read_csv('/content/drive/MyDrive/data/population/202001_202111_주민등록인구기타현황(출생등록)_birth.csv', encoding='cp949')

tmp5





## mission

1. 행정구역 뒤에 붙은 숫자와 괄호 제거
   - tmp['행정구역'].str.split(' ')  >> '행정구역' 열의 문자를 공백 기준으로 나누어준다.
   - tmp['행정구역'].str.split(' ').str[0]  >>  시리즈로 나온 리스트 중 index = 0 인 애들을 데려온다
   - tmp['행정구역'] = tmp['행정구역'].str.split(' ').str[0] 하면 끝~!
   - 
2. col 명의 년도, 월만 나오도록 수정
3. 인구수는 현재 문자열, 컴마를 제거하고 정수 형태로 변경
   - pd.read_csv(~~~, thousands = '  ,  ') : 컴마 제거
   - tmp11 = tmp1.col.str.replace(',', '').astype('int64')















































