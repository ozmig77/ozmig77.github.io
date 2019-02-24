# subway_seoul
simple d3 project

### 서울지도 d3로 그리기
https://www.lucypark.kr/blog/2015/06/24/seoul-matzip-mapping/
### 지하철 위도 경도 정보
http://data.seoul.go.kr/dataList/datasetView.do?infId=OA-118&srvType=A&serviceKind=1
- 지도밖의 점들은 날리는것이 맞을것 같다.
### 지하철 노선 색
https://ko.wikipedia.org/wiki/%ED%8B%80:%ED%95%9C%EA%B5%AD_%EC%B2%A0%EB%8F%84_%EB%85%B8%EC%84%A0%EC%83%89

### Data
- 서울시 지하철 호선별 역별 시간대별 승하차 인원 정보 (월별) 2015-1 부터 2019-1까지
http://data.seoul.go.kr/dataList/datasetView.do?infId=OA-12252&srvType=S&serviceKind=1

- 서울교통공사 연도별 일별 시간대별 역별 승하차 인원 (2008년 ~ 2017년 7월)
https://data.seoul.go.kr/dataList/datasetView.do?infId=OA-12921&srvType=F&serviceKind=1&currentPageNo=1

- 서울시 지하철호선별 역별 승하차 인원 정보 (일단위)
https://data.seoul.go.kr/dataList/datasetView.do?infId=OA-12914&srvType=S&serviceKind=1


### data/seoul_metro2018.json 
```
[2018년] (역별 list)
station_nm: 역이름
lng: 경도
lat: 위도
line_num: 노선이름
data: (월별 list)
  - month
  - nums (시간별 list)
     tuple
     - time 
     - ride 승차
     - alight 하차
```

### TODO
~~1. mouse 툴팁~~
~~2. 스크롤 하면 변환되게~~

