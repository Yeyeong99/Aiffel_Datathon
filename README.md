
# Aiffel_Datathon - NET2FLEX

> 아이펠 양재 캠퍼스 2기 데이터톤
> 
> “비즈니스에 도움이 될 수 있도록 데이터 EDA를 해보자.”


## 참고
### 4 OTT Basic EDA
1. [🔴Netflix Visualizations, Recommendation, EDA🍿](https://www.kaggle.com/niharika41298/netflix-visualizations-recommendation-eda)
2. [Netflix Data Visualization - Target Ages](https://www.kaggle.com/joshuaswords/netflix-data-visualization)
3. [IMDb Top 1000 dataset](https://www.kaggle.com/hrishabhtiwari/imdb-top-1000-movies-dataset)
#
### ott와 애니메이션의 상관관계
1. [[Plotly] Ultimate Web Series EDA!](https://www.kaggle.com/foolofatook/plotly-ultimate-web-series-eda/notebook)
2. [🎬📺 Netflix is Awesome! Why? see here📈📊](https://www.kaggle.com/bhuvanchennoju/netflix-is-awesome-why-see-here/notebook)
3. [Disney+ Movies and TV Shows](https://www.kaggle.com/shivamb/disney-movies-and-tv-shows)
4. [Anime DataSet 2022](https://www.kaggle.com/vishalmane10/anime-dataset-2022)
5. [성별·연령대별 유튜브 및 넷플릭스 콘텐츠 이용행태 분석](https://mediasvr.egentouch.com/egentouch.media/apiFile.do?action=view&SCHOOL_ID=1007002&URL_KEY=018a5e18-46ce-4e45-8d90-a62dacf3c60f)
6. [📽‍️ Netflix EDA for beginners 📺](https://www.kaggle.com/marcogherbezza/netflix-eda-for-beginners)
#
### datathon_netflix
1. [Latest Netflix data with 26+ joined attributes](https://www.kaggle.com/ashishgup/netflix-rotten-tomatoes-metacritic-imdb)
2. [IMDb Top 1000 dataset](https://www.kaggle.com/hrishabhtiwari/imdb-top-1000-movies-dataset)

3. [플릭스 패트롤 : 넷플릭스 순위 확인 사이트](https://flixpatrol.com/top10/netflix/world/2021/)
4. [넷플릭스 매출 확인 2010-2021](https://www.macrotrends.net/stocks/charts/NFLX/netflix/revenue)

 

# 진행

2022.03.08~2022.03.11

# 참고 자료

[Netflix statistics: How many subscribers does Netflix have? Worldwide, US member count and growth](https://www.insiderintelligence.com/insights/netflix-subscribers/)

- Overall, Netflix still accounts for the largest portion of time consumers spend with subscription [OTT video services](https://www.insiderintelligence.com/insights/ott-vod-video-streaming-services/), though its share is again slipping as users spend time on other VOD platforms.

[Why has Netflix not been able to crack the Indian market?](http://business-standard.com/podcast/companies/why-has-netflix-not-been-able-to-crack-the-indian-market-122012500081_1.html)

[Netflix didn't fail in India; Netflix India failed everywhere](https://entrackr.com/2022/02/netflix-didnt-fail-in-india-netflix-india-failed-everywhere/#:~:text=The)

[All The Reasons Why Netflix Is Doomed](https://www.forbes.com/sites/greatspeculations/2019/08/20/all-the-reasons-why-netflix-is-doomed/?sh=53b25c20465e)

[넷플릭스 주가 20% 폭락 원인. 그리고 4분기 실적발표를 통해 알아보는 극복 방안은?](https://contents.premium.naver.com/pickool/pickooltech/contents/220121135012468hu)

### 넷플릭스 컨텐츠 순위 사이트

[TOP 10 on Netflix in the World in 2021 * FlixPatrol](https://flixpatrol.com/top10/netflix/world/2021/)

### 넷플릭스 매출 2010-2021확인

[Netflix Revenue 2010-2021 | NFLX](https://www.macrotrends.net/stocks/charts/NFLX/netflix/revenue)

### **IMDb Top 1000 dataset**

[IMDb Top 1000 Movies Dataset](https://www.kaggle.com/hrishabhtiwari/imdb-top-1000-movies-dataset)

### Latest, complete Netflix Data from 4APIs

[Latest Netflix data with 26+ joined attributes](https://www.kaggle.com/ashishgup/netflix-rotten-tomatoes-metacritic-imdb/code)

### Netflix subscribers and revenue

[Netflix subscribers and revenue by country](https://www.kaggle.com/pariaagharabi/netflix2020)

### **Anime dataset 2020, 2022**

[Anime DataSet 2022](https://www.kaggle.com/vishalmane10/anime-dataset-2022)

[Anime Recommendation Database 2020](https://www.kaggle.com/hernan4444/anime-recommendation-database-2020)

# 배경

주어진 데이터와 관련해 해결 가능한 문제를 찾기 위해 최근 기사를 살펴보던 중, 넷플릭스의 부진한 성장에 관한 기사를 다수 발견할 수 있었다.

- 1월 넷플릭스 주가 20% 폭락
- 경영진도 고객 유치 결과를 둔화 단계라고 언급.

이러한 정체기이자 성숙해진 시장 속에서 넷플릭스의 매출을 증대할 수 있는 방법을 찾기 위해 다른 ott 서비스를 함께 분석했다. 분석 전 세운 가설은 다음과 같다.

1. 컨텐츠가 매출에 가장 직접적인 영향을 미칠 것이다.(질 보다 양을 선택한 넷플릭스?)
    - 컨텐츠를 보강한다.
    - 컨텐츠를 제작한다.
2. 특정 장르가 강한 플랫폼의 경우 이용자 확보가 더 용이하기 때문에 수익성에도 긍정적인 영향을 미칠 것이다.
3. 특정 나이대의 타겟층을 가진 플랫폼의 경우 이용자 확보가 용이하기 때문에 수익성 측면에서도 긍정적이다.

주어진 기본 데이터 네 가지에서는 각 플랫폼의 장르와 수익성, 특정 시청 연령과 수익성 사이 상관관계는 파악할 수 없다. 따라서 수익성과 관계성까지 모두 파악하지 못하더라도, 장르, 시청 연령을 비롯해 다양한 feature와 관련한 기본적인 EDA를 진행하고자 한다. 그리고 넷플릭스에서 보충할 수 있는 또는 제작할 수 있는 새로운 컨텐츠를 선별해 추천하고, 분석한 데이터를 바탕으로 주어진 데이터 이후의 넷플릭스의 수익을 예측해 컨텐츠의 추가가 수익성에 어느 정도의 영향을 끼치는지 확인하고자 한다.

# 아이디어

- 나라 간의 관계 => ex) 마블이 최초 개봉국을 한국으로 삼고 한국이 성공한다 싶으면 전 세계에서 흥행할 것이다. 하는 지표로 삼는 것처럼 최초 공개를 어떤 나라로 정할지..
    - 주어진 데이터셋에선 찾기 힘듦
- 스포츠 컨텐츠 강화?
        
    ## 헤이팅스 : 응~ 안돼 (회장님이 싫어해...)
    
    - 스포츠 중계는 광고로 도배된 구린 컨텐츠. “넷플릭스는 앞으로도 광고를 도입하지 않을 생각입니다. 또 뉴스, 스포츠 등 생중계 콘텐츠 없이 TV드라마와 영화에 집중할 예정입니다.”
    
- ~~movie lens~~ IMDb에서 상위 영화를 파악해 누락된 영화 추가하기
    - 좋은 컨텐츠를 보충할 수 있는지?
- 애니가 요즘 대세라던데?...

# 역할

- 확장된 비교 분석과 모델링 적용: 정우
    - 컨텐츠의 수가 매출에 영향이 있는가
    - 양질의 컨텐츠가 매출에 영향이 있는가
    - 이를 바탕으로 Regressor 모델에 적용하여 예측된 매출액에 대한 변화를 알아보자.
    
- 4가지 비교 분석, 넷플릭스 수익성과 상관관계 확인: 예영
    - 특정 장르가 우세한 플랫폼이 있는가
    - 특정 장르의 총합과 분기별 수익 사이의 관계성
    - 시청 연령과 분기별 수익 사이의 관계성
    - 장르별 별점의 평균과 수익 사이의 관계성

- 애니메이션 비교 분석: 원규
    - 나이별 넷플릭스를 이용하는 컨텐츠 분석
    - 플렛폼별 어느 콘텐츠의 소비가 높은지 확인
    - 넷플릭스의 애니메이션 소스
    - 넷플릭스와 디즈니 비교점
    - 정리

# 내용 정리

# datathon_netflix - 정우

**Latest Netflix dataset(4API) dataset**

```
Title                        0
Genre                     1710
Tags                        67
Languages                 1935
Series or Movie              0
Hidden Gem Score          2101
Country Availability        19
Runtime                      1
Director                  4708
Writer                    4330
Actors                    1925
View Rating               7024
IMDb Score                2099
Rotten Tomatoes Score     9098
Metacritic Score         11144
Awards Received           9405
Awards Nominated For      7819
Boxoffice                11473
Release Date              2107
Netflix Release Date         0
Production House         10331
Netflix Link                 0
IMDb Link                 2303
Summary                      9
IMDb Votes                2101
Image                        0
Poster                    3638
TMDb Trailer              8286
Trailer Site              8286
dtype: int64
```

- 많은 칼럼들이 존재하기 때문에 딥러닝 모델로도 적용해본다면 흥미로웠을 것 같다.

영화와 드라마의 비교.

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%201.png)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%202.png)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%203.png)

*** 보완된 netflix 데이터에서 **태그라는 feature**가 있다.

- 장르에 표시되지 않는 디테일도 표현해준다.
- Tags(태그)라는 칼럼도 있었는데, 컨텐츠를 대표하는 간단한 키워드로 정리된 칼럼.
- 예시로 원작 소설을 바탕으로 함, 실화를 바탕으로 함과 같은 장르에 담을 수 없는 설명이 적혀있음.
- 보고 싶은 컨텐츠를 검색할 때, 부연 설명을 달아줄 때 좋아보인다. 사용자 편의에 도움이 된다.
- 추천 시스템에서도 사용하면 흥미로운 결과를 낼 수 있는 feature로 생각된다.

```python
nlp = spacy.blank('en')
series_tags = df_series_tag['Tags']
for tag in series_tags:
    doc = nlp(tag)
words = [token.text
         for token in doc
         if not token.is_stop and not token.is_punct]
rest_string = ' '
for i in words:
   rest_string = rest_string+i+' '
    
wordcloud = WordCloud(width = 1400, height = 1400, 
                background_color ='red',  
                min_font_size = 5).generate(rest_string) 
  
# plot the WordCloud image                        
plt.figure(figsize = (8, 8), facecolor = None) 
plt.imshow(wordcloud) 
plt.axis("off") 
plt.tight_layout(pad = 0) 
  
plt.show()
```

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%204.png)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%205.png)

**CUSTOM DATASET**

**( Latest Netflix dataset(4API), Netflix Subscribers and Revenue, IMDb TOP1000 )**

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%206.png)

```python
def show_plot(genre_dict, title, x_len=10, y_len=10):
    plt.figure(figsize=(x_len, y_len))
    x = list(genre_dict.keys())
    y = list(genre_dict.values())
    plt.plot(x, y, color="green")
    plt.xticks(x, rotation = 45)
    plt.ylabel("Quantity", fontsize=15)
    plt.title(title, fontsize = 18)
```

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%207.png)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%208.png)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%209.png)

그래프는 상단부터

- 분기별 총매출
- 분기별 추가된 컨텐츠(왼쪽)
- 분기별 누적 구독자(오른쪽)

아래는 왼쪽부터

- 총매출과 총구독자의 추이
- 총매출과 추가된 컨텐츠의 추이

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2010.png)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2011.png)

### **CUSTOM DATASET의 상관관계**

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2012.png)

- 2018~ 2020상반기의 데이터.
- 이미 세계적인 기업, 매우 유명한 OTT 서비스를 제공하고 있고 있는 상태에서 특정 나라가 동떨어진 매출을 보일 확률은 적다. 즉, 서로의 상관관계가 1로 수렴하도록 나오는 것이 당연하다.
- 하지만 국가 단위로 세분화된 매출로 본다면 국가별로 어떤 전략을 취해야하는지 더 자세하게 파악할 수 있을 것으로 보인다.
- 누적 구독자는 총매출을 대변하고 있다고 봐도 좋다.
- 총매출은 신규 업로드 컨텐츠와 신규 구독자와 제법 크게 관련되어 있다. - 컨텐츠의 수가 매출에 영향이 있는가
- 의외로 평점이 좋은 양질의 작품이 많은 것은 매출과 크게 관련이 없었다. - 양질의 컨텐츠가 매출에 영향이 있는가

---

### 매출 예측해보기.

```python
model=XGBRegressor(n_estimators=3000, learning_rate=0.05,
                                   max_depth=4
                  )
random_state = 2020
lasso = make_pipeline(RobustScaler(), Lasso(alpha =0.0005, random_state=random_state))
ENet = make_pipeline(RobustScaler(), ElasticNet(alpha=0.0005, l1_ratio=.9, random_state=random_state))
KRR = KernelRidge(alpha=0.6, kernel='polynomial', degree=2, coef0=2.5)
model_xgb = xgb.XGBRegressor(colsample_bytree=0.4603, gamma=0.0468, 
                             learning_rate=0.05, max_depth=3, 
                             min_child_weight=1.7817, n_estimators=2200,
                             reg_alpha=0.4640, reg_lambda=0.8571,
                             subsample=0.5213, 
                             random_state=random_state, nthread = -1)
```

- XGBRegressor를 처음 사용하였고, 결과가 만족스럽지 않아서 추가적으로 여러 모델들을 사용해보았다.
- 매우 작은 데이터로 매출 예측을 시도한 것.
- 2018/1분기 부터 2020/1분기 까지의 데이터가 training set으로 사용되고, target data는 다음 분기의 총매출로 두었다.
- test 데이터는 2020/2분기 한줄 짜리 데이터.
- test 데이터에 대한 target 데이터는 위 참고 링크 중 넷플릭스 매출 자료가 올라간 사이트의 20년도 3분기 매출을 참고하여 만들었다. (test =$ 6.43B)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2013.png)

- 2020/2분기 test 데이터에서 “Number : 업로드된 컨텐츠 수” 에 대한 칼럼을 인위적으로 증가시킨 test2 데이터를 통해 매출 예측에 어떤 변화가 있는지 살펴보았다.(제발 매출이 많이 증가하기를...)

```python
from sklearn.linear_model import ElasticNet, Lasso,  BayesianRidge, LassoLarsIC

ENet = make_pipeline(RobustScaler(), 
										ElasticNet(alpha=0.0005, l1_ratio=.9, random_state=random_state)
										)

ENet.fit(x,y)
y_pred5 = ENet.predict(test)
y_pred5 = np.int64(y_pred5)
y_pred5

ENet.fit(x,y)
y_pred6 = ENet.predict(test2)
y_pred6 = np.int64(y_pred6)
y_pred6
```

- 처음 XGBRegressor을 사용했을 때, 3억5천만 달러의 오차가 발생.
- 큰 금액의 오차이지만 오차율로는 5%. 하지만! test, test2간의 예측값 차이가 없다...
- ENet 모델을 적용했을 때, 원하던 결과를 살펴볼 수 있었다!!!
- 심지어 상당히 유사한 결과를 예측한 것(오차율 0.32%)에서 나아가, 인위적으로 컨텐츠 수를 늘렸을 때 매출도 약 1억달러가 증가했다.
- 즉, 컨텐츠의 보강이 매출에 큰? 영향을 준다고 볼 수 있다. (매입금, 제작비, 투자금 등은 고려되지 않았지만... 그래도 분기의 매출)
- 의외로 평점이 좋은 양질의 작품이 많은 것은 매출과 크게 관련이 없었다. - 양질의 컨텐츠가 매출에 영향이 있는가

### 다시 살펴볼 결론

- 총매출은 신규 업로드 컨텐츠 제법 관련되어 있다.
- 의외로 평점이 좋은 양질의 작품이 많은 것은 매출과 크게 관련이 없었다.
- 회귀 모델을 통한 학습으로 출력한 예측 결과로 새로운 컨텐츠 또는 컨텐츠 보강의 중요성을 알 수 있었다.

질적인 중요성을 확인하지 못했더라도 아이코닉한 캐릭터나 브랜드, 대중적이면서도 작품성이 좋은 영화나 드라마가 중요한 것은 부정할 수가 없다.

그래서 어떤 영화를 추가해야하고, 제작하면 좋을까?

### 좋은 영화 추가를 위해 **IMDb rating data**를 사용했다.

- 가장 대중적인 영화 평점 사이트.
- 좋은 컨텐츠가 회사의 수익으로 직결되지 않을까? 넷플릭스는 질 보다 양이라는 평가를 받는다. (뭐가 많은데 이상하게 볼 것이 없는...)
    
    ![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2014.png)
    
- 1000위에 등록된 영화도 7.6점으로 제법 높은 평점에 위치해 있다.
- 양질의 영화로 구성된 top1000 리스트와 Netflix dataset과 비교했을 때, 아직 추가되지 않은 컨텐츠들은 어떤 것들이 있고 아직도 질적으로 보충할 컨텐츠가 많지 않을까?
- 비교해본 결과 1000개의 영화 중 625편이 미등록된 컨텐츠였다.  하지만 오래된 영화가 워낙 많았고 넷플릭스 이용자의 연령층 분포를 보았을 때 90년대까지로 제한하는 것이 낫겠다고 판단했다.
- 필터링 결과 636 편의 영화 중에 344 편의 미등록된 영화들이 있었다.
- 몇 편의 영화를 직접 확인해 본 결과 넷플릭스에는 확인되지 않은 영화였으나, 슈렉과 같이 조회가 되는 영화임에도 미등록 리스트에 포함된 경우도 있다. 표기법이나 실제 업로드된 시점과 데이터과의 괴리에서 충분히 발생할 수 있는 오류다.

`['25th hour', 'breaking the waves', 'eskiya', 'match point', 'hana-bi', 'nueve reinas', 'sen to chihiro no kamikakushi', 'vozvrashchenie', 'kôkaku kidôtai', 'cowboy bebop: tengoku no tobira', 'sarfarosh', 'mysterious skin', **'(500) days of summer'**, **'once'**, 'in the name of the father', 'the last king of scotland', 'babam ve oglum', '4 luni, 3 saptamâni si 2 zile', 'the royal tenenbaums', 'auf der anderen seite', 'avengers: endgame', 'letters from iwo jima', 'the station agent', 'serbuan maut', 'adams æbler', 'lilja 4-ever', 'the father', 'tangerines', 'i am sam', 'ford v ferrari', 'persepolis', 'da hong deng long gao gao gua', 'forushande', 'diarios de motocicleta', 'fantastic mr. fox', 'lola rennt', 'darbareye elly', 'star wars: episode iii - revenge of the sith', 'tropa de elite 2: o inimigo agora é outro', 'the batman', **"ocean's eleven"**,` (...)`**'avatar'**, 'mar adentro', 'hera pheri', 'le petit prince', 'saw', 'short cuts', 'edward scissorhands', 'trois couleurs: blanc', 'jodaeiye nader az simin', 'trois couleurs: rouge', 'le scaphandre et le papillon', 'badhaai ho', 'gegen die wand', 'mononoke-hime', 'doragon bôru chô: burorî', 'detachment', 'ed wood', 'x-men: days of future past', 'asuran', 'lagaan: once upon a time in india', 'gangs of wasseypur']`

## 4 ott basic eda - 예영

### 1. 넷플릭스, 디즈니+, 아마존 프라임, HULU 데이터 비교

각 장르가 타겟으로 삼는 시청 연령은 어떻게 될까?

- 넷플릭스

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2015.png)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2016.png)

- 디즈니 +

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2017.png)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2018.png)

- 아마존 프라임

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2019.png)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2020.png)

- HULU

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2021.png)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2022.png)

- 4개의 ott 서비스를 분석한 결과, 주된 장르와 시청 대상 연령에서 차이를 보였다. 특히 가족을 중심으로 한 컨텐츠를 제공하는 디즈니의 경우 성인 연령을 대상으로 한 컨텐츠는 아예 존재하지 않았다.

### 2. 지역과 분기별 수익성의 상관관계

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2023.png)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2024.png)

지역과 분기별 수익, 컨텐츠 사이 상관관계를 살펴봤을 때 분기별 공개된 컨텐츠와 지역별 수익 사이의 상관관계는 비교적 약한 것으로 드러났다. 

### 3. 넷플릭스의 분기별 수익성과 장르, 시청 대상 연령 사이의 상관관계

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2025.png)

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2026.png)

- 넷플릭스에서 분기별로 공개된 장르의 수와 분기 별 수익성에 관해 살펴본 결과는 다음과 같았다.

```
약한 상관성:
['Reality TV', 'Cult Movies', "Kids' TV", 'Classic Movies', 'Teen TV Shows', 'Sports Movies', 'Spanish-Language TV Shows', 'Thrillers', 'Science & Nature TV', 'TV Thrillers', 'Romantic TV Shows']

상관성:
['Children & Family Movies', 'TV Horror', 'Crime TV Shows', 'Korean TV Shows', 'Anime Features', 'TV Dramas', 'Anime Series', 'TV Sci-Fi & Fantasy', 'Romantic Movies', 'Comedies', 'International TV Shows']

강한 상관성:
['TV Action & Adventure']
```

- 특히 Kid’s TV의 경우 시청 연령과 수익성 간의 관계를 살펴보았을 때도 어느 정도 상관관계를 보였다. 즉, 두 상관관계에서 모두 의미 있는 결과를 보였기 때문에 공략할 만한 시장이라고 생각된다.
- 다만 단순한 컨텐츠의 수와 수익성의 상관관계이기 때문에, 특정 장르가 업로드 되어 수익성이 증가했다는 인과관계를 설명하기 위해선 다른 근거를 보충할 필요성이 있다.

### 4. 넷플릭스의 분기별 수익성과 장르의 평균 별점 사이 상관관계

- 넷플릭스의 수익성과 높은 상관관계를 보이는 경우, 해당 장르를 좋은 컨텐츠라고 판단해 많은 사람이 시청했고, 그런 경과가 수익성에 영향을 미치지 않았을까 생각했다. 따라서 수익성에 영향력이 있는 컨텐츠일 경우 IMDB에서의 평점이 높을 것이라고 생각했고, 그렇다면 평점과 수익성 사이의 관계도 파악할 수 있을 것이라고 생각했다. 이러한 전제를 바탕으로 분기별 공개된 장르의 평균 별점을 구한 후, 분기별 수익성과의 상관관계를 파악했다.

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2027.png)

- 하지만 분기별 공개된 장르의 평균 별점을 구해본 결과, 위와 같이 전반적으로 평점이 크게 높지 않은 것으로 드러났다. 다만 해당 데이터는 IMDB Top 1000 데이터셋과 대회에서 주어진 데이터 사이의 교집합을 이용한 것으로, 2000개라는 적은 수이기 때문에 이를 고려해야할 것이다.

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2028.png)

- 넷플릭스의 분기별 수익성과의 상관관계가 높게 측정된 장르를 선별해, 각 장르의 평균 별점과 분기별 수익성의 상관관계를 파악했다. 그 결과, 장르별 별점과 수익성 사이의 관계는 높지 않다는 사실을 확인할 수 있었다.

### 원규

- 넷플릭스에서 애니메이션 장르의 나이 타겟팅이 어린이 뿐만 아니라 장년층까지 가능성이 있는것을 볼 수 있었다. (자료는 복수응답이 가능한 시청비율 연령대입니다.)
    - 가장 높은 비율을 보인건 10~18살 사이이고 값이 줄어나가다가 60대가 되어서 약간 상승
    - 50~60대를 제외하고 매우 낮은 수치도 아니라서 가능성이 있다고 생각된다.
    
    ![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2029.png)
    
- 플렛폼들의 어떤 컨텐츠가 주요 소비되는지 볼 수 있는 지표들이다.
    - 그래프를 보게되면, 애니메이션은 영화, 드라마, 코미디에 이어 4번째로 많은 시리즈를 가지고 있다.  시리즈의 이점은 장기적으로 고객을 잡아 둘 수 있다는 점인데, 이러한 점을 활용해 충성고객을 만들 수 있다.
    
    ![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2030.png)
    
    - (로튼토마토 기준) 평점 그래프를 보면 애니메이션 바는 평균 평점 위에 있는것을 볼 수 있다.
    - 물론 평균이라 별로인  자료가 있을 수 있지만,  그 수에 비에 좋은 평가를 받은 작품이 많다는 증거이기도 하다.
    
    ![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2031.png)
    
- 넷플릭스는 기존에 인기가 있었던 애니메이션 시리즈를 사와 스트리밍 한다.
    - 애니메이션 모음 데이터와 넷플릭스 데이터 교집합에 있는 애니메이션들은 사와서 스트리밍을 하는 방식 인데, 평가가 좋게 나온다.
    
    ![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2032.png)
    
- 넷플릭스를 맹추격 하고 있는 디즈니는 자체 ip를 많이 가지고 있고, 소비자 충성심이 높다.
    - 표를 보면 알겠지만, 옛날에 개봉했던 애니메이션을 재개봉하거나, 영화화 해서 상영한다.
    
    ![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2033.png)
    
- 그래서 넷플릭스와 디즈니를 비교해보자면
    - 먼저 넷플릭스와 디즈니가 가지고 있는 애니메이션의 수가 어느정도 되는지 파악해봤다.
    - 애니메이션 수는 넷플릭스가 앞서간다.
    
    ![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2034.png)
    
    - 그럼 평균 등급은 어느정도로 나왔는지 확인해보았다.
    - 아주 근소한 차이로 넷플릭스가 더 좋은 점수를 받았다.
    
    ![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2035.png)
    
- 정리
    - 애니메이션장르는 생각 외로 여러 나잇대를 대상으로 삼을 수 있다.
    - 플랫폼들에서 애니메이션수는 생각 외로 많았고, 평가도 준수한 수준이다.
    - 넷플릭스는 평이 좋았던 애니메이션들을 사온 후 스트리밍을 하는데, 이는 그 애니메이션을 좋아했던 팬들을 잡을 수 있게 해준다.
    - ott 디즈니는 디즈니 자체가 가지고 있는 ip를 활용해서 자체제작을 하는 편인데, 소비자 충성심이 높기 때문에 이러한 시도를 해도 성공할 수 있는 것 같다.
    - 아직까지는 디즈니가 넷플릭스에 비해 평점과 애니메이션 콘텐츠 수는 적지만, 판권을 사와야 하는 입장보다 자체 ip를 활용한 제작이 훨씬 더 경제적인 것 같다.
    
    (기사 참고 - 넷플릭스 미야자키 하야오 [https://www.bizhankook.com/bk/article/19690](https://www.bizhankook.com/bk/article/19690))
    
    - 최근 넷플릭스에서 게임 ip를 활용한 제작 애니메이션 아케인이 매우 큰 인기를 끌었다.
    
    이런 성공을 밑거름 삼아 다른 플렛폼과 차별화된 애니메이션을 제작하면 더 많은 나이 층을 공략 할 수 있다고 생각한다.
    
    ![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2036.png)
    

# 그래서 어떠한 컨텐츠를 제작하면 좋을까?

![Untitled](https://github.com/Yeyeong99/Aiffel_Datathon/blob/main/README%20images/Untitled%2037.png)

```
약한 상관성:
['Reality TV', 'Cult Movies', "Kids' TV", 'Classic Movies', 'Teen TV Shows', 'Sports Movies', 'Spanish-Language TV Shows', 'Thrillers', 'Science & Nature TV', 'TV Thrillers', 'Romantic TV Shows']

상관성:
['Children & Family Movies', 'TV Horror', 'Crime TV Shows', 'Korean TV Shows', 'Anime Features', 'TV Dramas', 'Anime Series', 'TV Sci-Fi & Fantasy', 'Romantic Movies', 'Comedies', 'International TV Shows']

강한 상관성:
['TV Action & Adventure']
```

- 실제로 넷플릭스에서 흥행한 작품을 살펴봤을 때 어느 정도 유의미한 상관관계를 보여준 장르에 해당하는 작품 (종이의 집(TV Action&Adventure), 오징어 게임, 루팡 (Crime) 등)이 순위권에 있는 것을 확인할 수 있었다.

- 시청 연령을 대상으로 수익성과의 상관관계를 계산했을 때 또한 Kids가 유효한 상관관계를 보이는 것으로 나타났다. 장르 상에서 ‘Kid’s TV’의 상관관계 또한 높게 나왔기 때문에, 두 상관관계를 고려했을 때 어린이를 대상으로 하는 컨텐츠에 집중하는 것도 한 방법이 될 수 있다고 생각한다.

---
