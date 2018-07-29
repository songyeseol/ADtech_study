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
	
### [ 과금방식 ] 

- 광고주 입장 
	- transaction = unit  
	- CPT / CPA 선호 
- 서치엔진 입장 
	- 노출 = unit 
	- CPM 선호 
- 중간 
	- 클릭 = unit 
	- CPC 선호  

- 이 세가지 모델 모두 많이 쓰임
- 검색광고에서는 CPC가 가장 많이 쓰임 


### [ 인터넷 광고 초기 ]

- 1994년 초기 시장에서는,
	- 노출당 과금방식
	- 인력 협상 과정 필요 
	- 누가 돈을 지불해야하는지 애매함 
		- 서치엔진은 광고 덕에 다른 서비스를 제공할 수 있게 되고, 
		- 광고주는 트래픽과 노출을 받을 수 있게됨 
	- 작은 계약도 거래비용이 매우 큼 
	- 타게팅을 할 수 있는 검색광고는 불가능했음

### [ 일반화된 일차가격 경매 (Generalized First-Price Auction) ] 

- Overture에 의해 만들어진 옥션 
- 키워드에 대한 CPC 과금 방식 
	- 검색 스팸을 없애고자 한 노력 
	- 서치엔진은 가장 많은 돈을 지불할 의향이 있는 광고주 순서대로 노출
- 결과:
	- 타게팅 / 작은 단위의 거래 가능 
	- 비딩가격 순서대로 결과 노출
	- 당신의 비딩 가격만큼 지출 
	- 오버츄어는 야후와 MSN의 플랫폼이 되었음 
		- 하지만 불완전한 매커니즘 
	- 입찰가 순환(bid cycle)의 문제: 경쟁하느라 모두 시간을 소모하게 되고, 매출도 떨어짐 
		- 모두가 가격을 낮추려고 노력할것
		- 예를 들어, 최저가 10원으로 시작했는데, a가 10원 입찰, b는 11원 입찰. 
		- 입찰가가 너무 많이 오르면 a,b중 1명이 최저가인 10원으로 입찰하고, 낮은 위치로 만족하게 됨. 
		- 그러면 다른 1명은 최저가보다 1원 높은 11원으로 입찰. 다시 경쟁 시작. 

		
### [ 일반화된 이차가격 경매 (Generalized Second-Price Auction) ] 

- 2002년에 구글에 의해서 도입
- 야후/오버츄어 등 GSP로 전환
- 두 가지 방법: 
	- 비드 랭킹
		- 비딩가격 순서대로 결과 노출
		- 하지만 1번 순서 광고주는 2번 순서 광고주의 비딩가격을 지불
	- 수익 랭킹
		- 예상수익을 순서대로 결과 노출 
		- 1번순서 광고주는 (2번 비딩가격 * (2번 CTR / 1번 CTR)) 만큼 지불 
		- 결국 1번은 1번비딩가격보다 적게냄 ( 1번비드 * 1번CTR > 2번비드 * 2번CTR )
		- 모든 광고주의 CTR이 동일하다면 비드 랭킹과 동일해짐 
	- 모두가 적절한 가치로 경매에 입찰하는 쪽으로 수렴 
		- 예를 들어, 100원의 가치가 있는 제품을 경매한다면, a가 100원을 입찰, b는 95원을 입찰. 
		- 그러면 a는 경매에서 1등을 하고, b의 입찰가인 95원을 지불하니 5원의 수익 발생. 
		- 만약 a가 105원을 입찰했다면, 5원의 손해를 보게됨. 
		- 따라서 모두가 적절한 가치로 경매에 입찰하게 됨. 
		
### [ VCF는 GSP가 아니다 ] 

- GSP는 Dominant strategy가 없음
- 만약 한 슬롯만 있다면 둘이 동일
- 하지만 여러 슬롯이 존재한다면 다름 
	- gsp는 비더1에게 비더2의 비드를 과금하고, 
	- vcg는 비더1의 **externality**를 과금한다.  
	
### [ VCG ] 

- 만약 2개의 슬롯이 존재하고, 3명의 비더가 있다면, 
	- 1 슬롯: 200클릭 / 2 슬롯: 100클릭 
	- 1 비더: 10달러 / 2 비더: 4달러 / 3 비더: 2달러
- 2번 비더: 200달러 과금 
	- 3번의 기회비용 ( $2 * 100클릭 ) 을 지불해야함 
- 1번 비더: 400달러 과금
	- 2번의 기회비용 ( $4 * (200클릭-100클릭) ) 을 지불해야함
	- 즉, 기회비용 = (i가 그 슬롯을 가지지 않았더라면 i+1이 지불했을 금액) - (i+1이 지금 지불하는 금액)

> VCG기반 과금방식을 통한 수익은 GSP방식에서 truth telling equilibrium의 전제 하에 얻을 수 있는 수익보다 낮다. 



### [ definition ]  

![image](https://user-images.githubusercontent.com/28600272/43268584-fa3d0bca-912b-11e8-8574-5e99f817caf1.png)

- 비더 k의 포지션 i에서 payoff = (i에서 예상되는 클릭수 * k가 생각하는 클릭당 가치) - 과금액 
- 과금액  = (i에서 예상되는 클릭수) * (i+1번째로 높은 비딩금액) 

즉, 위를 섞으면 
> 비더 i의 payoff = i에서 예상되는 클릭수 * ( i의 비딩금액 - i+1의 비딩금액 ) --맞나?--


### [ 검색광고에 적용해보자면.. ] 

![image](https://user-images.githubusercontent.com/28600272/43269898-cdfb514a-912e-11e8-9bc4-498e6e3e161d.png)

- 비딩금액이 높을 수록 더 높은 포지션  
- 가장 비딩금액이 낮은 비더의 비딩금액은 GSP나 VCG나 같다. 
- i포지션에서의 과금액 = (i에서 예상 클릭수 - i+1에서 예상 클릭수) * (i+1로 들어가는 비더의 비딩금액) + (i+1의 과금액)
> 무한루프 아니냐...? 거의 재귀함수..? 뭐징.

```
정리
- ad의 순서 > IR과 Econ 모두를 고려하는 것 
- GFP는 안정적이지 않음
- GSP는 정직하지 않음 
- VCG는 안정적이고 정직하나 잘 안쓰임 
```





		



# Lecture 3: Sponsored search 1

### [ 검색 광고에서 역할 ] 

- 광고주
	- 특정 비드 프레이즈에 광고 submit
	- 광고 포지션에 비딩
	- CPC 지불
- 유저
	- 서치엔진엔 '특정 의도'를 가지고 쿼리를 입력
- 서치 엔진
	- (웹 코퍼스 + 다른 데이터 소스)에 대한 쿼리를 실행
	- (광고 코퍼스)에 대한 쿼리를 실행
	- 웹 결과 + 다른 데이터 + 광고를 결합한 SERP(Search result page)를 디스플레이
- 즉, 서치엔진, 광고주, 유저는 모두 각자 다른 유틸리티를 갖는다. 
	- 서로 상충되기도, 상호보완적이기도 함 
- 상호보완되는 부분
	- 서치 엔진 & 광고주 - 더 많은 클릭을 원함 > SE는 수익, 광고주는 Volume을 얻을 수 있음 
	- 서치 엔진 & 유저 - 좋은 광고를 원함 > 좋은 광고는 유저클릭을 발생, SE는 수익 
- 상충되는 부분 
	- 높은 CPC는 SE에게는 득이 되지만 광고주는 아님
	- 연관성이 낮지만 PPC가 높은 광고는 유저들에게 좋지 않음 > 하지만 SE에게는 수익을, 광고주에게는 ROI를 높일 수 있음 

### [ 여기서 어떻게 최적화된 절충안을 찾는가? ]

- 전체 시스템의 큰 그림을 보고 장기적인 목표를 수입
- 비즈니스 특성의 변화를 반영할 수 있도록 parameterized
- 단순화 > 비즈니스 owner들이 쉽게 의사결정을 내릴 수 있도록 

- 최적화 펑션 = f(광고주 유틸리티, 유저 유틸리티, SE 유틸리티)
(convex linear combination으로 만들 수 있음, 모든 유틸리티의 가중치의 sum =1 )


### [ 좀 더 단순하게 ] 

- 장기적인 유틸리티는 파악하기도 어렵고 정량화하기 어렵다. 
- 따라서, search당 수익을 최대화하자! 
	- subject to 
		- search당 유저 유틸리티 > a
		- search당 광고주 ROI > b
- 1) 유저 유틸리티가 a보다 높은 광고들을 찾고,
- 2) b이상의 ROI를 가지는 광고를 최적화해서 보여줌 



### [ 광고 연관성 = 유틸리티 총합의 simple proxy가 될 수 있음 ] 

- 유저들에게는 좋은 유저 경험을 제공
- 광고주에게는 더 질좋은 트래픽을 제공 (하지만 volume은 낮아질 수 있음)
- SE는 더 높은 클릭수를 통해 수익을 제공 (하지만 낮은 지면커버율로 수익이 낮아질 수 있음)

즉, "광고 연관성"은 모든 문제를 해결해주진 않는다

### [ 쿼리는 검색광고의 드라이버! ] 

- 쿼리는 유저의 의도를 대변한다
	- ad selection의 가장 큰 드라이버
	- 유저의 니즈를 정의
- "intent entropy"는 검색광고에서 매우 낮음 > 유저의 목적성을 잘 알 수 있다. 즉 유저의 의도에 대한 분류가 쉽다? 명확하다. 


### [ 쿼리의 종류 ] 


- informal
	- 뭔가에 대해 알고 싶음 (swine flu prevention)
- navigational 
	- 특정 페이지를 방문하고 싶음 (alitalia US)
- transactional 
	- 웹에서 뭔가를 하고 싶음 (New York weather)
	- 서비스에 접근 / 다운로드 / 쇼핑 등 
- gray areas 	
	- find a good hub / exploratory search "see what's there"



### [ 왜 long tail이 있는가? ] 

가설  
1) 대부분 사람들은 usual 쿼리를 입력한다; 소수가 unusual을 입력
2) 대부분의 사람들이 usual 쿼리를 입력한다; 그리고 그 사람들이 unusual쿼리도 가끔 입력한다
	- Goel 2009 연구가 두번째 가정을 증명
	- 대부분의 사람들은 popular 상품, niche 상품 모두 소비하는 경향이 있음
	- 하지만 이 비율? 정도는 다름
	


##  2. TEXTUAL AD 

광고주 > 어카운트 > 캠페인 > 애드 그룹 > 크리에이티브 + 비드 프레이즈 



### [ 광고 쿼리 관계 ] 

- 반응형 쿼리 responsive : 쿼리의 의도를 직접적으로 충족시킴
	- e.g. Realgood golf clubs
	- ad: Buy realgood golf clubs cheap!
- incidental: 유저의 의도가 쿼리에 직접적으로 명시되지 않음 
	- 연관쿼리 related : local golf course special
	- 경쟁쿼리 competitive : sureshot golf
	- 연관쿼리 associated : rolex watches for golfers 
	- 스팸쿼리 spam : vitamins 

### [ 랜딩페이지 종류 ] 

- 카테고리 : 랜딩페이지가 쿼리의 큰 카테고리를 나타냄
- 서치 트랜스퍼 : 광고주 웹페이지 내에서 서치 결과를 나타냄
	- 상품 리스트
	- 서치 aggregation
- 홈페이지
- 기타 (프로모션 등) 

## 3. ad selection

- 매치 종류
	- exact : 쿼리와 비즈 프레이즈가 정확히 매치
		- 광고주는 특정 쿼리에 특정 양을 비딩 
		- 단수형, 오타, re-order, 노이즈 = 모두 같은 쿼리 (쿼리 정규화)
	- advanced : 광고 플랫폼이 주어진 쿼리에 적합한 광고를 찾아줌
		- 광고주는 특정 쿼리에 비딩을 하는 것이 아니라 광고주가 관심있을 만한 쿼리에 비딩을 하게 됨 
		- 대부분의 트래픽은 bid가 없다. 
		- 광고주에게 비드 프레이즈는 중요하지 않다. 전환율이 높으면 되는 것! 
		- 어떻게 연관된 트래픽을 전부 커버할 수 있을까? SE의 챌린지 
- 실행방법
	- 데이터베이스 lookup
		- : 쿼리 q에 대해서 광고는 record, 비드 프레이즈는 attribute
	- 유사도 서치
		- : 쿼리 q에 대해 광고는 ad corpus안의 document, 비드 프레이즈는 meta-datum 
- 2 phases of  selection
	- ad retrieval
		- : ad corpus 전체에서 가장 viable한 후보를 뽑음
	- ad reordering
		- : 후보들을 가지고 더 정교한 scoring function으로 순서를 정함 
		- retrieval score 뿐만 아니라 비딩액을 고려하여 순서를 정함 
- reordering 종류 
	- 반응형
		- : 클릭테이터를 활용
	- 예측형
		- : 광고 지면 위치에 쌓인 데이터를 활용하여 성과를 예측 
		- 광고의 다양한 피쳐들을 추출 > 각 피쳐들의 가중치를 찾아냄 > 예측에 활용 
		- 광고에 대해 충분한 정보가 있다면 reactive, 아니라면 predictive 사용 
- 사용되는 데이터(주로 예측형에) 
	- unsupervised
	- click data
		- 볼륨이 매우 크기때문에 샘플링 필요할수도
		- 바이너리 (클릭 or no click)
		- CTR은 주로 매우 낮음 
		- 사람들은 광고가 연관성이 높아도 클릭하지 않음 
		- 노이즈 많음 
	- relevance data
		- Editorial 리소스가 많이 필요함
		- 에디터들은 연관성에 대한 확실하고 정밀한 기준이 필요함 
		- 에디터들은 모든 도메인과 유저 니즈를 이해할 수 없음 

### [ 광고주의 딜레마 ] 

- broad 쿼리? vs. 컨셉 쿼리? 
	- 먄악 내 광고가 "good prices on seattle hotels"라면, 
	- seattle이라는 단어를 가진 쿼리에 비드를 할 것 
	- 하지만 alaska cruises start point는 나에게 유의미한 쿼리가 될 수 있고,
	- seattle's best coffee chicago는 나에게 무의미한 쿼리가 될 수도.
	- 따라서 시애틀을 여행 목적지로 나타내는 쿼리에 비딩하는 것이 중요

## 4. query rewriting

### [ 유저 세션 ] 

- 유저는 task를 완수하기위해 SE사용
- task는 ( 쿼리들 입력 + 브라우징) 의 단계를 거침 
- 쿼리를 재입력하는 것을 보고 쿼리 스트림을 알 수 있음
- 재입력에 적합한 쿼리를 어떻게 파악하는가?
	- 유저가 직접 입력한 재입력 쿼리를 관찰 (유저의 지식을 활용해랏!)
	- 재입력 쿼리의 가치를 정하기 위해 해당 쿼리의 다양한 인스턴스를 관찰 

![image](https://user-images.githubusercontent.com/28600272/43365055-9a8d3dac-9361-11e8-9e71-48c79dc9b33e.png)



### [ 재입력 쿼리 종류 ] 

- swich tasks
- insertions
- substitutions
	- 많은 substitution이 많은 유저에 의해서 반복됨 
- deletions
- spell correction
- mixture
- specialization
- generalization
- others


### [ 해결과제 ]

- "세션 바운더리"를 찾는 것이 문제 
	- time period 
	- 쿼리 유사도나 레이블 세트를 기반으로 계산 
- 재입력 쿼리의 종류 
- 재입력 쿼리 파악하려면 높은 빈도를 보여야만 함 






 


# Lecture 4: Sponsored search 2

# Lecture 5: Display advertising 1

# Lecture 6: Display advertising 2

# Lecture 7: Targeting

# Lecture 8: Recommender systems

# Lecture 9: Mobile, video, and other emerging formats
