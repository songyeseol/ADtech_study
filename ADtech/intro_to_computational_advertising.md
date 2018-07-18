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
- + 매치 메이커



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

1) Represenation of user/context/ads: **효과적이고 효율적으로** 유저, 컨텍스트, 광고를 대표하는 것
2) Definition of optimization problem: 시장의 한계와 목표를 해결하기 위해 수학적 최적화 문제를 정의하는 것 
3) efficient and effective Solution: **효과적이고 효율적으로** 최적화 문제를 해결하는 것 


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

두 가지 종류의 온라인 배너 광고  

1) **(보장형)** 개런티 딜리버리 (GD)

representation
- 타게팅 요소를 기반으로 계약된 거래 (age, income, location...)
- 각 거래는 1) 기간, 2) 노출양이 정해져있음  

definition of the optimization problem 
- 문제: 계약금액 / 트래픽 예측 / 활성화된 거래에 대한 노출 분배  

2) **(성과형)** 논-개런티 딜리버리 (NGD) = performance graphical ads  

성과에 따른 과금 - CPM / CPC / CPA  

optimization problem definition 
- = CTR 극대화  

representation  
- 1) Reactive : 여러 지면에 게재된 특정 광고의 CTR을 관찰 > 가장 높은 CTR을 보이는 지면에 광고 노출 
- 2) Predictive : 관련된 광고, 랜딩 페이지, 광고주 정보를 사용하여 광고에 대한 여러 피쳐들을 생성 > 페이지와 광고 피쳐를 기반으로 성과 예측 
- 3) hybrid : 위 두개를 결합  


## 6) textual ad

### [ textual ad ]

1) 검색 키워드 광고 = **"스폰서 서치"**  
(aka 키워드 광고, paid search, adwords...)  
	- 광고주는 "bid phrase" 선택 
		- = 디스플레이를 할 쿼리
	- **"advanced match"** 옵션도 존재 
		- = 연관된 쿼리에 디스플레이 

2) 웹페이지의 컨텐츠에 따른 광고 = **"컨텐츠 매치"**
(aka 컨텍스트 광고, adsense)  

-> textual ad는 검색과 information retrieval과 연관이 높음  


### [ textual ad의 역사 ]

1) 1990년 후반, 알타비스타 "스폰서 서치" 모델 개발
	- 서치 엔진 유저들에게 거절당함
2) goto.com(나중에 overture가 인수)가 "유료광고에 대한 서치 엔진" 개발
	- 상업적 관심사를 가진 유저들이 이 엔진으로 감 
	- 돈이 모임
3) 구글이 "스폰서 서치" 모델 다시 개발 
	- 성공적
4) 광고주들이 충분한 볼륨을 갖지 못함 
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

1) 스폰서 서치 (sponsored search) > 쿼리를 bid phrase에 **매치**

2) advanced match > 쿼리를 bid phrase로 **번역**
- 컨텍스트, 연관성을 잡아내기 어려움 
- 과금이 잘못될 수 있음 

3) content match > 페이지에서 bid phrase를 잡아냄
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

# Lecture 3: Sponsored search 1

# Lecture 4: Sponsored search 2

# Lecture 5: Display advertising 1

# Lecture 6: Display advertising 2

# Lecture 7: Targeting

# Lecture 8: Recommender systems

# Lecture 9: Mobile, video, and other emerging formats
