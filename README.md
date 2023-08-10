# naver_news_crawler
칼부림을 키워드로 크롤링, 워드 클라우드 제작, 빈도 분석

selenium 프레임 워크를 사용하여 네이버 뉴스로 이뤄진 포맷에 대하여 뉴스 url들을 크롤링
@lru_cache 데코레이터로 url을 key 뉴스 제목과 내용을 value로 
LRU 캐싱 전략을 사용하는 캐시를 사용하여 각 뉴스별 제목 및 내용을 크롤링하여
실시간성을 조금 포기하고, 성능적 이점을 얻는 방식으로 제작
형태소 분석을 거친 뒤 워드 클라우드로 만들어보는 프로젝트이다.

수집한 정보는 csv 파일로 저장하였고, 저장했던 csv 파일을 konlpy를 활용해 한국어 형태소 분석을 진행해 보았다.
추후에 지역명과 예고 등에 가중치를 둘 수 있게 알고리즘을 설계한다면 
칼부림 예고 지역에 대한 알림을 제공할 수 있는 시스템을 만들 수 있을 것으로 기대된다.
