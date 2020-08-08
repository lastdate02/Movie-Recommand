# movie-recommand
* 데이터 출처 : https://www.kaggle.com/tmdb/tmdb-movie-metadata

## Data
* id
* title
* genres
* vote_average
* vote_count : 평점을 매긴 사람의 수
* popularity : 인기도
* keywords : 영화의 키워드
* overview : 개요 설명

## Environmnent
Python 3.7 / Windows 10 / RAM 8gb / i5-8300H / GTX 1050

## Library
* Scikit-learn

## Model
* 컨텐츠 기반 필터링
* 콘텐츠에 대한 여러 텍스트 정보들을 피쳐 벡터화
* 코사인 유사도로 콘텐츠별 유사도 계산
* 콘텐츠 별로 가중 평점을 계산
* 유사도가 높은 컨텐츠 중에 평점이 좋은 컨텐츠 순으로 추천

## References
* https://www.quora.com/How-does-IMDbs-rating-system-work
* https://chan-lab.tistory.com/
