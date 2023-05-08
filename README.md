# Roblox-Play-Video-Text-Analysis

## Statistical and information retrieval-based keyword analysis in speech text data of metaverse activity video
(메타버스 활동 영상의 발화 텍스트 데이터에서의 통계 및 정보 검색 기반 키워드 분석)

> 현실의 사용자의 대리자인 아바타와 그 아바타들이 활동하는 공간을 디지털로 구현한 가상 세계를 메타버스라고 한다. 본 연구에서는 대표적인 메타버스 플랫폼인 로블록스에서 서로 다른 활동 종류에 따른 메타버스 참여자의 행동을 데이터화하고, 정보검색 및 통계 기법으로 분석하는 데이터 기반 연구를 시도하였다. 로블록스에서 활동 종류로서, 10개의 서로 다른 게임 종류를 선정하고, 각 게임 종류 별로 10개의 유튜브 플레이 영상을 수집하고, 플레이 영상의 음성에서 텍스트를 추출하여 데이터화하고, 단어빈도 분석, TF-IDF 분석, 통계 분석의 텍스트 마이닝 분석을 수행하였다. 게임 종류 별로 상위 10개씩 중요 키워드를 도출하였을 때, 게임 특성에 맞는 단어가 도출되었으며, 이러한 단어를 사용하여 머신러닝 분류 예측을 수행하였을 때, 예측 정확도가 향상됨을 확인하였다. 우리의 연구는 메타버스 세계에서활동을 데이터화하고 데이터 기반으로 행동 양식을 분석하는 연구의 시발점으로서 의의가 있다.

> ![로블록스플레이화면](https://user-images.githubusercontent.com/108673913/236810618-c5b68622-2d2c-471f-a70a-7c4b4837ebf2.jpg) 

<img src="https://user-images.githubusercontent.com/108673913/236810618-c5b68622-2d2c-471f-a70a-7c4b4837ebf2.jpg" width="800" height="400"/>

### 데이터설명
> 본 논문에서는 대표적인 메타버스 플랫폼인
로블록스(Roblox)에서 서로 다른 활동 종류에 따른 메타버스
참여자의 행동을 데이터화하고, 텍스트 마이닝 및 통계 기법을
적용하여 분석하는 데이터 기반 연구를 시도하였다. 로블록스
플랫폼에서 가장 인기 있는 게임 10개에 대해서 유튜브에서 각
게임에 대한 플레이 영상을 10개씩 선발하고, 영상으로부터
음성- 텍스트화(Speech to text)를 수행했다. 

- 선정한 로블록스 게임 종류

|Game Name|Genre|Number of Game|
|------|---|---|
|'Adopt Me!'|가족 롤플레잉 게임|10|
|'Meep City'|롤플레잉 게임|10|
|'Tower Of Hell'|어드벤처, 파쿠르 게임|10|
|'Piggy'|스포츠 공포 탈출 게임|10|
|'Royale High'|롤플레잉 코디 게임|10|
|'Jail Break'|범죄게임|10|
|'Murder Mystery 2'|마피아게임|10|
|'Welcome to bloxburg'|집짓기 롤플레잉 게임|10|
|'Pizza factory tycoon'|타이쿤(경영) 요리 게임|10|
|'Restaurant Tycoon'|타이쿤(경영) 게임|10|

### 분석 방법
- 단어 빈도 분석: 단어 빈도수(word count) 분석은 정보 검색 분야에서 해당글에서 특정 단어가 많이 나올수록, 글의 주제를 파악하고 있다는 전제하에, 각 문서에서 각 단어들이 나오는 빈도로 주용도를 조사하는 방법이다.

- TF-IDF 분석: TF-IDF(Term Frequency-Inverse Document Frequency, 단어 빈도-역문서 빈도)는 정보 검색 분야에서 다중 종류 문서 데이터가 주어졌을 때, 특정 단어가 각 문서에서 얼마나 중요한지를 정량화하는 방법이다. 전체 문서 집합 $D$가 주어졌을 때, 어떤 단어 $t$의 어떤 문서 $d$에서의 중요도인 $TFIDF(t,d,D)$는 다음과 같다.
$$TFIDF(t,d,D)=TF(t,d)×IDF(t,D)$$

- 피셔 정확 검정 분석: 두 개의 변수가 서로 상관관계가 있는지에 대해서 검정하는 통계적 방법으로 카이제곱 검정이나 피셔 정확 검정이 있다. 예를 들어, 전체 문서 데이터셋에서 중복을 포함하여 단어가 총 $N$번 나온다고 할 때, 각 단어가 $t$와 같은 단어인지, 게임 $g$에서 등장했는지에 조사한 빈도수의 분할표가 아래와 같다고 하자.

### Speach To Text(STT)

### 전처리

### 결과
