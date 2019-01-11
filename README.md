# 1. Cosmetic Recommendation Model
데이터 전처리 느낀점

<텍스트 전처리>
1. 이모티콘 삭제
2. 특수문자 삭제
3. id, nickname은 unique값 확인 
- 0으로 시작하는 nickname은 앞의 0을 엑셀이 지움 (007 > 7)
- 이것을 확인 안하면 nickname "7"이 여러명 생김

(1) 화장품 사용자들의 제품 평점정보를 바탕으로 유사도를 측정하여, 유사한 사용자들간의 제품을 추천해준다.

(2) 사용된 알고리즘
  - CF(Collaborative Filtering)
  - user-based
  - Peason 유사도
  - KNNBasic

(3) 결과(K=5 기준)
  - 제품 리뷰 수가 많은 고객들일수록 차별화된 제품 추천이 이뤄진다.
