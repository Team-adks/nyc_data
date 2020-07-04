# An exploration of NYC open dataset

## Where to access?

https://data.cityofnewyork.us/browse 이곳에서 접속해 서치 가능하다. 현재 2873개의 데이터셋이 제공된다.

## How to filter? 

왼편의 바에서 "category", "Types", "Collection", "Agency", "Tag" 로 필터링을 할 수 있다.

Category에서는 건강, 지리, 교육 등 시에서 중시하는 데이터의 종류별로 들여다볼 수 있다.

Type에서 특기할 만한 건 "data lens page"와 "dataset"으로, 렌즈 페이지는 dataset을 기반으로 한 시각화 대시보드다. 
데이터셋에서는 말 그대로 모아둔 시 데이터를 다운받을 수 있는데, 주로 .xlsx나 .csv 포맷으로 되어 있고 크기도 작다. 크면 gb 단위 정도.
대신 메타데이터가 잘 정리돼 있고 페이지에서 데이터의 row/column을 바로 체크할 수 있어 편리하다.
모두 export랑 API 옵션을 제공한다. API는 Socrata Open Data API (SODA)를 사용한다. 

External dataset은 말 그대로 외부 기관의 데이터로 링크만 걸려 있다. 데이터를 이용하려면 따로 그 기관에 permission을 요청해야 할 수도 있다.

Collection에서는 최근 시에서 핫한(?) 주제를 항목별로 묶어놓았으며 역시 데이터셋이다.

Agency로 특정 기관에 관련된 데이터만을 필터링할 수 있는데, 기관의 성향과 관련없는 주제로 필터가 걸려 있으면 아무것도 안 나올 수 있다.
(covid-19와 브루클린 도서관...)

Tag를 누르면 리스트를 볼 수 있는데, 특히 특정 연도 (2017, 2018...) 의 데이터셋을 찾는 데 편리하다.

## What to look at?

Pros: 메타데이터 및 포맷이 정리가 잘 돼있으며 API 역시 제공된다.

Cons: 포맷이 정리가 잘 돼있으며(...) 크기가 너무 작다. NYC 데이터이므로, 한국인들이 흥미를 가질 수 있는 셋이 제한되어 있다. <s>센트럴 파크 다람쥐 센서스</s>

일단 가장 먼저 생각해볼 수 있는 건 Covid-19 관련 데이터셋인데 콜렉션을 통해 볼 때 수가 4개로 적은 편이고 크기도 크지 않다.
대시보드 정도로 보여주는 것 이상의 재미있는 마이닝을 하기는 어려워 보인다. <s>트럼프가 지원 안해주나</s>

링크는 여기: https://data.cityofnewyork.us/browse?Data-Collection_Data-Collection=COVID-19+Health+Data

일반 건강의 경우 오히려 데이터셋이 다양하다. restaurant inspection 이라든가 베이비 네임이라든가... 

링크는 여기(이하 많이 본 순서대로 정렬): https://data.cityofnewyork.us/browse?category=Health&limitTo=datasets&sortBy=most_accessed&utf8=%E2%9C%93

City data라는 점을 감안하면, 현재 서울의 문제와 겹치는 종류의 데이터셋이 흥미로울 듯.
Business나 government, education 은 한국과 뉴욕주/시의 체계가 많이 달라서 접점을 찾기는 어려울 듯하지만,
Transportation이나 Housing & development 같은 경우, 서울의 부동산 정책은 언제나 핫이슈이므로 이런 부분을 보고 비교하면 흥미를 끌지 않을까.
실제로 액세스의 규모도 건강이나 다른 토픽에 비해 큰 편.

Transportation datasets: https://data.cityofnewyork.us/browse?category=Transportation&limitTo=datasets&sortBy=most_accessed&utf8=%E2%9C%93

Housing & dev datasets: https://data.cityofnewyork.us/browse?category=Housing+%26+Development&limitTo=datasets&sortBy=most_accessed&utf8=%E2%9C%93
