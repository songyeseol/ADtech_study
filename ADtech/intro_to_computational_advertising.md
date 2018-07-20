# MS&E 239: Introduction to Computational Advertising 
(September-December, 2011 - Stanford University, California)

[Class material page link](https://web.stanford.edu/class/msande239/#lecture-handouts)


# Lecture 1: Introduction  


## 1) Overview 


### [ Compututational Advertising ]

```Find the "best match" bewtween a given user in a give context and a suitable advertisement```  
주어진 컨텍스트에서 특정 유저와 적절한 광고 사이의 최적의 매치를 찾는 것  

- 컨텍스트 예시: 검색 광고, 배너 광고, 모바일, 비디오, 신문 등  


### [ 참여자 ]

- 퍼블리셔 
- 광고주
- 유저
- "매치 메이커"



### [ Key Message ]

- CA란 "BEST MATCH"를 찾는 것
- CA 시장은 매우 큼 
- 광고는 정보의 한 형태 (a form of information)
	- 최적의 광고를 찾는 것은 information retrieval 문제의 한 종류
- 새로운 적용 도메인과 새로운 기술이 매일 생겨나는 중 


## 2) 전통적인 광고 

### [ 브랜드 광고 ]

- 목표: 보기좋은 이미지를 생산하는 것 

### [ 다이렉트 마케팅 ]

- "직접적인 반응"을 유도하는 광고
- 구매, 구독, 투표, 기부 등



## 3) CA의 필요성 

### [ Computational은 이미 여러 도메인에 적용되는 중 ]

- linguistics, biology, chemistry, mechanics, economics...

즉 computational 이란,  
1) 고전 학문을 **computing capability**와 융합하는 것 
2) 문제해결을 위해 **알고리즘적으로 생각**하는 것 



### [ computational의 필요성 ]

- 전통적으로는
	- 상대적으로 적은 지면 - 잡지, 빌보드, 신분, handbill, TV 등 
	- 지면 당 높은 비용 (슈퍼볼 TV 광고에 300억 달러)
	- 개인화 불가능 
	- 광고인력의 경험, 직관에 따른 타게팅
	- ROI 측정 불가 

- 현재 Computational은 (위와 거의 반대)
	- 수많은 기회
	- 수많은 크리에이티브
	- 완전한 개인화
	- 한 광고당 낮은 비용
	- 성과 측정 가능 


### [ CA의 상대적 어려움 ]


1) 시장과 거래를 디자인하고, 유저, 광고주, 매체에게 돌아가는 가치를 극대화하는 것
2) 이 프로세스를 받쳐줄 인프라를 구축하는 것 


### [ 주요한 해결과제 ]

- 1) Represenation of user/context/ads
	- **효과적이고 효율적으로** 유저, 컨텍스트, 광고를 대표하는 것
- 2) Definition of optimization problem
	- 시장의 한계와 목표를 해결하기 위해 수학적 최적화 문제를 정의하는 것 
- 3) efficient and effective Solution:
	- **효과적이고 효율적으로** 최적화 문제를 해결하는 것 


### [ CA와 시장 디자인 ]

SYSTEMS > COMPUTATIONAL ADVERTISING > MARKET DESIGN


## 4) 시장의 기회 

- 온라인 광고의 시장규모와 변화추이? 
- 한국시장? 세계시장?
- 어떤 광고 포맷에 가장 돈을 많이 쓰는가?
- 어떤 종류의 광고주가 가장 돈을 많이 쓰는가? 
- 어떤 매체에 가장 돈이 몰리는가? 
- 가장 지배적인 플레이어는? 


### [ 왜 온라인에 돈을 쓰는가? ]

- 마케터들은 온라인 광고가 가장 안전하다고 생각
	- 성과 측정 가능
	- 효율 증대 
	- 타게팅 가능 
- 다른 미디어에 마케팅 예산을 투자하는 것 보다 온라인에 투자하는 것이 더욱 믿음직스러움  


### [ 웹 광고의 가치 ]

광고는 웹의 거대한 생태계를 서포트하는 역할  

1) 퍼블리셔 수익이 크고 작은 퍼블리셔들의 생존을 유지하게함 
2) 타게팅이 niche 시장의 비즈니스를 돌아가게 만듦 
3) 광고주 수익이 큰 스케일의 서비스를 가능하게 만듦 (페이스북, 구글, 트위터..) 

즉, 광고가 없었더라면 웹은 매우 작은 세계였을 것.  
(광고는 유저에게 직/간접적인 가치를 제공하고 있음)  


## 5) CA 산업의 랜드스케이프 


### [ 시장에 대한 기초 개념 ]

**CPM** : 천개 노출에 대한 비용  
- 주로 배너광고에 사용 (브랜드 광고)
- 미리 금액 지불 가능 (개런티드 딜리버리 Guaranteed Delivery)

**CPC** : 클릭당 비용  
- 주로 textual 광고에 사용 

**CPT/CPA** : 거래/액션당 비용 (= referral fee 혹은 affiliate fee)  
- 주로 쇼핑, 여행업체
- 하지만 요즘에는 textual 광고에도 쓰임 (위험완화)  

### [ 배너 광고 ] 

> 두 가지 종류의 온라인 배너 광고  

- 1) **(보장형)** 개런티 딜리버리 (GD)
	- representation
		- 타게팅 요소를 기반으로 계약된 거래 (age, income, location...)
		- 각 거래는 1) 기간, 2) 노출양이 정해져있음  
	- definition of the optimization problem 
		- 문제: 계약금액 / 트래픽 예측 / 활성화된 거래에 대한 노출 분배  


- 2) **(성과형)** 논-개런티 딜리버리 (NGD) = performance graphical ads  
	- 성과에 따른 과금 - CPM / CPC / CPA  
	- optimization problem definition 
		- = CTR 극대화  
	- representation  
		- 1) Reactive : 여러 지면에 게재된 특정 광고의 CTR을 관찰 > 가장 높은 CTR을 보이는 지면에 광고 노출 
		- 2) Predictive : 관련된 광고, 랜딩 페이지, 광고주 정보를 사용하여 광고에 대한 여러 피쳐들을 생성 > 페이지와 광고 피쳐를 기반으로 성과 예측 
		- 3) hybrid : 위 두개를 결합  
	

## 6) textual ad

### [ textual ad ] 

- 1) 검색 키워드 광고 = **"스폰서 서치"** (aka 키워드 광고, paid search, adwords...)  
	- 광고주는 "bid phrase" 선택 
		- = 디스플레이를 할 쿼리
	- **"advanced match"** 옵션도 존재 
		- = 연관된 쿼리에 디스플레이 

- 2) 웹페이지의 컨텐츠에 따른 광고 = **"컨텐츠 매치"** (aka 컨텍스트 광고, adsense)  

-> textual ad는 information retrieval과 연관이 높음  


### [ textual ad의 역사 ] 

- 1) 1990년 후반, 알타비스타 "스폰서 서치" 모델 개발
	- 서치 엔진 유저들에게 거절당함
- 2) goto.com(나중에 overture가 인수)가 "유료광고에 대한 서치 엔진" 개발
	- 상업적 관심사를 가진 유저들이 이 엔진으로 감
	- 돈이 모임
- 3) 구글이 "스폰서 서치" 모델 다시 개발
	- 성공적
- 4) 광고주들이 충분한 볼륨을 갖지 못함
	- 좀더 많은 노출을 위해 "컨텐츠 매치" 등장
 


## 7) ad selection

### [ 광고 선택의 목표 ]

- 각 참여자는 효용을 느끼는 부분이 다름  
	- 광고주: ROI와 Volume
	- 유저: 연관성 (relevance)
	- 퍼블리셔: 노출/검색당 수익
	- 애드 네트워크: 수익 및 성장 

- **모두의 효용을 높일 수 있도록 최적화 필요**

### [ textual ad selection ] 

- 1) 스폰서 서치 (sponsored search) > 쿼리를 bid phrase에 **매치**

- 2) advanced match > 쿼리를 bid phrase로 **번역**
	- 컨텍스트, 연관성을 잡아내기 어려움 
	- 과금이 잘못될 수 있음 

- 3) content match > 페이지에서 bid phrase를 잡아냄
	- 컨텍스트, 시맨틱, 연관성 잡아내기 어려움 

### [ textual ad schema ] 

광고주 > account > 캠페인 > ad group > creative / bid phrase


### [ 정보로서의 광고 ] 

```최적의 텍스츄얼 광고를 찾는 것은 여러 가지 모순되는 효용 기능을 가진 정보 검색 문제이다.```

- representation: 광고를 IR의 '문서'라고 생각하면 됨 
- optimization/solution: ad corpus위에서 쿼리를 평가하여 광고를 추출 

예시) 

- ad corpus 
	- textual ad
		- bid phrase / title / creative / url / landing page
	- graphical ad
		- advertiser-supplied meta data / url / landing page / content of page with clicks 
- query feature 
	- search keyword / outside knowlege expasion / context feature 
- context feature (sponsored search)
	- location / user data / previous search
- context feature (content match)
	- location / user data / page topic / page keyword 





# Lecture 2: Marketplace design


### [ 광고주는 어떤 유저를 찾는가? ]
 
- qualified
	- 비즈니스에 기반한 확실한 속성에 따른 유저 선택
	- 예: 미국에서만 판매되는 차 모델 -> 적당한 수입을 가진 미국시민 
- receptive
	- 광고주 메세지에 어느정도 관심이 있는 사람
	- 예: 스키 광고에 관심있는 사람들은 주로 자전거 광고에도 관심이 있음
- reponsive
	- 광고주가의 의도한대로 반응할 경향을 보이는 유저 
	- 퍼포먼스 광고주들의 목표 = 반응률
	- 브랜드 광고주들의 목표 = 빠른 반응률 
	- 예: 클릭율, 전환율, 

### [ 광고는 attention을 위한 시장이다! ] 

- attention은 다른 상품과는 달리, match가 중요하다.
	- 다른 상품) 차 판매자에게는 누가 차를 사는지는 중요하지 않다. 
	- attention) 광고주입장에선 **누구의 attention**인지가 중요하고, 유더입장에서는 **어떤 광고**인지가 중요함.  

## (1) 스폰서 검색 광고 (paid search)

### [ 퍼블리셔, 광고주, 유저 + 매치 메이커 ] 

- 퍼블리셔: 검색 결과 페이지의 주인
- 주로 퍼블리셔와 매치메이커가 같지만, 다를 수 있음

### [ 스폰서 서치에서의 상호작용 ] 

- 광고주
	- 특정 bid phrase에 대해 광고를 제출 
	- bid for position
	- CPC 
- 유저
	- 서치엔진에서 쿼리를 날림
- 서치 엔진
	- **웹 코퍼스 + 다른 데이터소스**에 대해 쿼리를 실행
	- **광고 코퍼스**에 대해 쿼리를 실행
	- 웹결과, 다른 데이터, 광고 결합한 결과 페이지 보여줌 


## (2) 스폰서 광고 해결문제 1: ad retrieval

- 일단 광고주는 키워드/프레이즈에 비딩을 함 

- 유저의 쿼리에 서치엔진은 다음을 제공함:
	- **exact match** 
		- 광고주는 특정한 쿼리에 대한 특정 노출양으로 비딩
	- **advanced match**
		- 광고주는 특정 쿼리에 비딩을 하는 것이 아니라, 광고주와 관련된 쿼리에 노출됨 
		- 볼륨이 많아야하고, new/rare 쿼리가 보장이 되어야함 (tail 쿼리에 대해 광고)
	- **phrase match** 
		- 쿼리의 서브프레이즈 = 비드 프레이즈에 맞다면 노출
		- 쿼리: fresh red flowers / 비드프레이즈: red flowers

## (3) 스폰서 광고 해결문제 2: 광고의 순서와 과금 

### [ 게임 이론 ] 

: 한 게임은 모든 경기자들의 선택에 달려 있기 때문에 각 경기자는 선택을 잘하기 위해 다른 경기자들이 선택할 수 있는 것을 예측하려고 한다. 어떻게 하면 상호의존적인 전략적 계산을 합리적으로 할 수 있을까 하는 것이 게임이론의 주제이다. 

- auction theory 
	- 경매시장에서 사람들이 어떻게 행동을 하는지에 대한 이론 
- mechanism design 
	- 경쟁이 공정하지 않고 개인들의 의사결정이 한정된 정보에 기반할 경우 어떠한 과정을 통해 결과가 도출되는가에 대해 다룬 이론
- dominant strategy
	- 상대의 선택에 상관없이 주어진 플레이어에게 더 좋은 결과를 가져다 줌 
- optimal strategy
	- 어떤 목적함수를 최대화하는 전략
- nash equilibrium
	- 게임의 플레이어가 타인이 취하는 전략을 기초로 자신의 이익이 최대가 되도록 행동하고 또한 이것이 모든 플레이어에게 공통될 때, 이 균형상태를 내시균형


### [ 경매 종류 ] 


1) first-price sealed bid (최고가밀봉호가경매)
	- 모두가 밀봉된 봉투에 가격 기재하고 제출 
	- 최고가격 제시한 사람이 이김 
	- 경락자가 제시한 금액 지불 
2) second-price sealed bid auction (Vickrey auction)
	- 최고가밍봉호가경매와 경매방식을 동일
	- 두번째로 높은 비딩금액을 경락자가 지불 
3) open ascending-bid auction (English auction)
	- 경재진행자가 점차적으로 금액을 높임
	- 가장 마지막까지 남아있는 사람이 경락자
4) open descending-bid auction (Dutch auction)
	- 경매진행자가 점차적으로 금액을 낮춤 
	- 첫번째로 콜을 부른 참여자가 경락자 

### [ 스폰서 검색 경매 ] 

- 서치 엔진 
	- 광고 지면을 판매하기 위해 키워드 경매를 진행
- 광고주
	- 한 클릭당 지불할 의향이 있는 금액을 비딩 
- 서치엔진은 내림차순으로 광고들을 정렬
	- 비딩 금액이 광고 위치의 "key determinant" 
	- CTR은 부수적인 determinant
	

### [ 인터넷 광고 시장의 특이점 ] 

- market design 측면 
	- 비딩이 끊임없이 일어남 
- featured of the enviroment 측면 (쉽게 변하지 않는 특성)
	- 서치엔진은 효과적으로 "flows"를 판매 (click/hour)
	- 사용되지 않는 capacity는 낭비됨
	- 하지만 유저 입장에서 효용성은 과도한 광고랑 반비례 
	




# Lecture 3: Sponsored search 1

# Lecture 4: Sponsored search 2

# Lecture 5: Display advertising 1

# Lecture 6: Display advertising 2

# Lecture 7: Targeting

# Lecture 8: Recommender systems

# Lecture 9: Mobile, video, and other emerging formats
