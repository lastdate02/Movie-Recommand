# movie-recommand
영화 추천 모델
* https://www.kaggle.com/tmdb/tmdb-movie-metadata
## 컨텐츠 기반 필터링
* 콘텐츠에 대한 여러 텍스트 정보들을 피쳐 벡터화
* 코사인 유사도로 콘텐츠별 유사도 계산
* 콘텐츠 별로 가중 평점을 계산
* 유사도가 높은 컨텐츠 중에 평점이 좋은 컨텐츠 순으로 추천
* id
* title
* genres
* vote_average
* vote_count : 평점을 매긴 사람의 수
* popularity : 인기도
* keywords : 영화의 키워드
* overview : 개요 설명
* https://chan-lab.tistory.com/
### 평가 횟수에 대한 가중치가 부여된 평점 계산
* 가중 평점 = (v/(v+m)) * R + (m/(v+m)) * C
* v : 개별 영화에 평점을 투표한 횟수
* m : 평점을 부여하기 위한 최소 투표 횟수 (ex. 상위 60%, 40%)
* R : 개별 영화에 대한 평균 평점
* C : 전체 영화에 대한 평균 평점
* https://www.quora.com/How-does-IMDbs-rating-system-work
