---
layout: page
title: 비즈니스를 위한 오픈 소스 소프트웨어
subtitle: 6장 배포란 무엇인가?[^1]
---

오픈소스 라이선스 조건(고지사항 전달, 소스코드 공개, 동일조건 재라이선스 요건)은 배포로 촉발된다. 거의 모든 오픈소스 라이선스에 대해서, 만약 소프트웨어를 재배포하지 않는다면, 라이선스를 행사하는 어떤 조건도 만족할 필요는 없다. 하지만, 배포란 무엇인가? 20년전에는 이러한 질문에 대답이 쉬웠지만, 매년 점점더 어려워지고 있다.

[^1]: 이번 장에 대한 이전 버젼은  "The Gift that Keeps on Giving: Distribution and Copyleft in Open Source Software Licenses," IFOSSLR Volume 4, Issue 1 (March 2012) 에 나와있다. 최초 [http://www.ifosslr.org](http://www.ifosslr.org) 사이트에 온라인으로 게시됐다. 

### 예술의 미국식 용어

GPL은 본질적으로 조건부 저작권 라이선스로, 법선택(choice-of-law) 조항이 없다. 따라서, 이론적으로 적용가능한 저작권법에 규정된 행위만이 카피레프트 조건에 대한 적용을 촉발할 수 있다. 미국에서, 저작권에 대한 상업적 핵심 권리를 배포(distribution) 혹은 발행(publication)이라고 부른다. 따라서, 미국에서 카피레프트 조건을 촉발하는 것에 대한 질문은 저작권법 아래서 배포를 구성하는 것에 대한 문제와 동일시된다.

2007년에 출시된 GPL3는 "전파(propagate)" 혹은 "전달(convey)"같은 중립적 단어를 사용해서 이런 개념에 대해 지역적 변형에 맞춰서 라이선스 국제화를 시도했다. 후계자와 달리 GPL2는 구체적으로 배포를 카피레프트 요구사항에 대한 기폭제로 명명했다.특히 리눅스 커널에 적용되는 라이선스로 GPL2는 폭넓게 사용되고 있다. 그래서 GPL2 아래 배포를 구성하는 질문은 오픈소스 세계에서 여전히 살아있고 건재하다.

미국법 아래 저작권에 대해서 열거된 권리중에 하나지만, 배포는 저작권법(Copyright Act, Title 17 of the United States Code)에 정의되어 있지 않다. Title 17은 저작권 소유자에게 배타적 권리를 부여했다. "저작권 권리를 갖는 저작물의 사본을 일반 대중에게 판매 혹은 다른 소유권 이전으로, 임대차 계약, 임대, 대출로 배포"할 권리가 있다.[^2] 법률은 "사본을 일군의 사람에게 추가로 배포, 공연(public performance), 공개(public display)을 목적으로 제공하는 것이 발행을 구성한다."[^3]라고 법률은 언급하고 있다. 하지만, 이것이 *배포(distribution)*를 정의하지는 않는다. 법규 용어가 액면 그대로 애매모호하면, 법규 해석에 대한 원칙은 법규의 입법이력을 살펴보는 것을 허용하고 있다. 1976년 하원보고(House Report)[^4]도 또한 *배포*를 정의하지 않지만, 
"유형물이 주인이 바뀌지 않는 어떤 형태의 전파(예를 들어, 공연 혹은 텔리비젼에 공개)는 발행이 아니다."[^5]라고 언급하면서, *발행*을 네거티브 방식으로 정의하고 있다. 후에 판례는 배포와 발행을 동일시 했다.[^6]

[^2]: 17 U.S.C. Section 106(3).
[^3]: 17 U.S.C. Section 101.
[^4]: H.R. Rep. No. 94-1476.
[^5]: House Report 138 참조, 1976년 U.S.C.C.A.N. 5754 재간행.
[^6]: Harper & Row Publs., Inc. v. Nation Enters., 471 U.S. 539, 552 (1985)

저작권법 106(3)절은 "저작권 소유 저작물의 사본 혹은 레코드판을 일반 대중에게 판매 혹은 다른 소유권 이전으로, 임대차 계약, 임대, 대부로 배포"할 배타적 권리를 저작권 소유자에게 부여한다. 달리 표현하면, 저작권 소유자는 일반 대중에게 판매, 기부, 임차, 저작물 구현체를 빌려줄 배타적인 권리를 갖는다.[^7] 이번절의 입법 역사에 나타나듯이, *배포* 정의는 "101절에 *발행*의 정의에 것과 사실상 동일하다".[^8] 따라서, 본질적으로 배포에 대한 배타적 권리는 저작물 발행을 제어할 권리가 된다.

[^7]: National Car Rental Sys., Inc. v. Computer Assocs. Int’l, Inc., 991 F.2d 426, 430 (8th Cir. 1993).  
[^8]: Reg. Supp. Rep., p. 19.  

#### 배포가 언제 발생한 것인지 결정하기

따라서, 미국에서 *배포*는 또다른 사람에게 유형의 사본을 제공함을 의미한다. 따라서, 배포를 구성하는 것에 대한 질문은 다음 두 질문으로 이전된다: *유형의 사본(tangible copy)*은 무엇이고, *또다른 사람(another person)*은 무엇이냐?

저작권법 아래 배포 정의를 촉발하기 위해서는 저작물이 "일반 대중(to the public)"에게 이전되어야만 된다. *일반 대중* 문구에 대한 법적 정의가 부재한 상황에서, 법원은 원고 콘텐츠를 명확하게 특정된 집단과 제한된 목적을 갖고, 판매, 배포, 복제, 유포의 권리 없이 의사소통하는 "제한"된 형태의 배포는 일반대중에 배포가 아니라는 점을 견지하고 있다.[^9]

[^9]:  White v. Kimmell, 94 F. Supp. 502, 505 (S.D. Cal. 1950); Data Cash Sys., Inc. v. JS&A Group, Inc., 628 F.2d 1038, 1042-43 (7th Cir. 1980) (concluding that “a ‘limited publication’ is really in the eyes of the law no publication at all”); John G. Danielson, Inc. v. Winchester-Conant Props., Inc., 322 F.3d 26, 36 (1st Cir. 2003); Brown v. Tabb, 714 F.2d 1088, 1091 (11th Cir. 1983); William A. Graham Co. v. Haughey, 430 F. Supp. 2d 458, 470 (E.D. Pa. 2006); Milton H. Greene Archives, Inc. v. BPI Commc’ns, Inc., 378 F. Supp. 2d 1189, 1198 (C.D. Cal. 2005); Penguin Books U.S.A., Inc. v. New Christian Church of Full Endeavor, Ltd., 288 F. Supp. 2d 544, 555 (S.D.N.Y. 2003). 

다른 말로, 만약 (1) 한정된 집단에 (2) 제한된 목적으로 (3) "판매, 배포, 복제, 유포의 권리 없이" 행해지지 않는다면 배포는 "일반적인" 발행이 된다. 저작권법의 입법역사는 "사본 혹은 레코드판이 도매업자, 방송사, 영화관 등의 집단에 제공될 때, 만약 목적이 추가 배포, 공연, 공개라면, 발행이 일어난 것"을 명확히 하고 있다. 따라서, 설사 저작물이 단 한사람 혹은 개체에 배포될지라도, 만약 수령자가 저작물 사본을 자유로이 유포, 복제, 배포, 판매한다면 발행이 성립된다는 것이 일반적 견해다.

현대 정보기술에 있어, 많은 활동이 사본 배포에 충분히 길을 잃을 정도로 근접해서 배포 정의의 경계에 도전하고 있다. GPL 준수를 위한 전략을 그날그날 꾸려가는 회사에게 GPL 아래서 배포가 무엇이냐는 질문은 엄청난 관심이 되는 것이 이러한 활동들이다.

기준점에서 출발해서, 가장 명확한 비즈니스 사례는 배포된 제품 사례다. 제품이 소프트웨어 단독 혹은 하드웨어 제품이던, 사업가는 제품을 판매한다는 것이 의미하는 것과 주인이 바뀐다는 것을 이해하고 있다. 따라서, GPL2같은 오픈소스 라이선스를 준수하려는 회사는 활동을 평가하는데 더 많은 어려움이 있다. 상업적 배포에 대한 비즈니스 사례로 판단되는 활동이 아니라, 그럼에도 불구하고 법률상 배포를 구성하는 활동이 어려움의 대상이다. 이번 장에서 법률적 사안으로 가장 명확한 것부터 가장 명확지 않은 것까지 다른 비즈니스 사례를 논의한다.

### 클라우드에서 명확한 사례

소프트웨어 전송 혹은 원격사용(ASP 혹은 SAAS 모형, 혹은 클라우드 컴퓨팅으로 불림)이 배포를 구성하는지 회사에서 종종 궁금증을 갖는다.

이것이 자유 소프트웨어 라이선싱에 대해 가장 논란이 많은 점중 하나지만, GPL2에 대해서 미국법 아래서 어려운 해석 질문은 아니다. 자유 소프트웨어 옹호자는 만약 카피레프트 요구사항에 대한 기폭제가 배포라면, 점차적으로 대중화되고 있는 클라우드 컴퓨팅 모형은 이런 요구사항을 피해갈 수 있음을 오랜기간 인식하고 있다. 이것을 종종 "ASP 구멍(ASP loophol)"이라고 부른다.[^11]

[^11]: 이 용어는 리차드 스톨만덕으로 돌리지만 정확하지 않을 수 있다. 2007년 4월 3일 *Groklaw*와 리처드 스톨만 인터뷰를 참조한다. 여기서 스톨만은 이 용어가 오해소지가 있다고 언급한다. [http://www.groklaw.net/articlebasic.php?story=20070403114157109](http://www.groklaw.net/articlebasic.php?story=20070403114157109)

GPL 3 버젼 초안을 집필하는 동안에 이 쟁점이 상당한 논쟁을 불러 일으켰다. 어느 순간, 카피레프트 요구사항을 촉발하도록 온라인 사용을 할수 있는 선택옵션을 저자가 선택하는 GPL3 변형이 제안되었다. 궁극적으로, 이런 변형은 GPL3에서 제거되고 "아페로 GPL"로 알려진 대안 라이선스 형태로 기념되고 있다. GPL3 기본 형태는 ASP 혹은 SAAS가 카피레프트 요구사항을 촉발하지 않는 것을 명확히 하고 있다. GPL3에서 카피레프트는 배포보다는 *전달(convery)*로 촉발되고, "저작물을 전달한다는 것은 다른 상대방이 사본을 받을 수 있거나 만들 수 있는 전파의 유형을 의미한다. 사본 전이없는 컴퓨터 네트워크를 통한 사용자와 단순한 상호작용은 전달이 아니다"[^12]

[^12]: GPL 3, 0절, "정의" [http://www.gnu.org/copyleft/gpl.html](http://www.gnu.org/copyleft/gpl.html). 

미국법 아래, 배포는 형태에 관계없이 사본의 실질적 이전를 요구하고 있다. 따라서, 미국법아래 SAAS 사용(사용자에 로컬 사본 이전없이 소프트웨어에 접근을 수반)은 GPL 아래 카피레프트 요구사항을 촉발시키지는 않는다.

### 극단적 사례(Edge Cases)

(명확하게 배포를 구성하는) 배포된 제품과 순수 SAAS 배포(deployment)라는 두가지 상대적으로 명확한 비즈니스 사례를 잠시 옆에 두고, 흔한 사업활동에서 제기되지만, 배포 동전의 한면 혹은 다른 면에 깔끔하게 속하지 않는 일부 극단적 사례에 눈을 돌려보자. 

- **종업원** : 회사가 이런 사례에 관해서 걱정을 하지만, 어려운 것은 아니다. 종종 고객이 기업 내부에 "내부 배포(internal distribution)" 가 카피레프트 요구사항을 촉발하는지 문의를 한다. 하지만, 현행법에서 내부 배포같은 것은 없다. 왜냐하면 회사와 회사에 소속된 종업원은 단일 법인으로 간주되기 때문이다. 따라서, 소프트웨어 사본을 동일 회사 다른 직원에게 업무를 수행하는 과정에서 직원으로서 제공하는 것은 분명히 배포가 아니다; 설사 사본 이전이 있을 수 있지만, 또다른 사람에게 이전된 것은 아니다. 자유 소프트웨어 옹호자는 때때로 이것을 *사적 사본(private copies)*을 제공한다고 부른다.

- **도급인(Independent contractor)-개인** : 회사가 종종 직원보다는 도급인으로 개인을 고용한다. 특히, 최근 부각되어 성장하는 회사는 직원 고용과 연관된 (고용세 같은) 규제력을 갖는 간접비를 회피하는데 이를 활용한다. 이런 경우에 도급인 기능은 거의 직원의 기능과 동일하다; 하지만, 도급인은 직원이 아니기 때문에, 소프트웨어 사본을 도급인에게 제공하는 것이 배포로 간주될 수 있다. 이것이 GPL2 해석에 있어 곤란한 점 중 하나고, 아래서 좀더 자세히 논의한다.

- **도급인(Independent contractor)-자문회사(consulting firm)** : 회사는 종종 소규모 자문회사를 고용해서 소프트웨어 개발, 테스트, 지원한다. 이러한 자문 독립체는 팀으로 일하는 몇 사람으로 구성되지만, 회사에 기능적 관계는 개인 컨설턴트 혹은 임직원의 기능과 유사하다. 소규모 자문회사 개개인은 법적으로 말해서 회사의 직원이 아니다. 따라서 사본을 제공하면 아마도 배포가 된다. 하지만, 사본은 공중의 이용가능성(public availability)을 의도하고 있지 않아서 자문회사 컨설턴트에게 이전은 발행이 아니므로 배포도 아니다. 이 주장은 위험이 있지만, 만약 당사자 의도를 나열하는 서면 컨설팅 동의서가 있다면 특히나, 아마도 법아래서 지탱될 수도 있다. 법적 의미에서 이런 비즈니스 사례는 도급인과 약속하는 것과 유사하다. 

- **도급인(Independent contractor)-외주(outsourcing)** : 좀더 큰 회사는 종종 소프퉤어 개발 혹은 소프트웨어 지원 같은 전체 사업영역을 외주준다. 외주인력은 명백히 임직원이라기 보다는 별도 회사다. 따라서, 사본을 외주받는 자에게 제공하는 것은 명백히 사본을 제공하는 것이 된다. 하지만, 일부 외주회사는 고객이 제어하거나 소유한 서버와 설비에 필요한 작업을 진행하는데 임대한 인력을 제공한다. 이런 경우, IT 회사는 이러한 인력에게 공급된 사본은 회사 제어 밖으로 이전된 것이 아니라는 일리있는 주장을 할 수도 있다. 하지만, 이런 주장이 미국 밖에 상주한 외주인력(대부분의 경우 그렇다)에 대해서는 덜 성공적일 수 있다. 국제적 분업이 GPL 아래 어떤 법이 배포를 결정할지 명확하지 않다.

- **클라우드 서비스 제공업자** : 아마존 웹 서비스 (Amazon Web Service, AWS) 같은 클라우드기반 컴퓨팅 서비스가 성장함에 따라, 소프트웨어를 클라우드 서비스에 올리는 것(uploading)이 배포가 되는지 회사들이 걱정한다. 이 질문이 일부 논란이 있지만, 대답은 아마도 아닐 것이다. 기술적으로 클라우드 서비스 제공업체에 사본 이전이 관련되어 있지만, 사본이 거주하는 가상 공간은 해당 회사 사용자 제어권 아래 놓여있다; 일반적으로 클라우드 서비스 동의계약에 따르면, 클라우드 계정에 저장된 정보에 대한 어떤 제어도 클라우드 서비스 제공업체에 허락하지 않는다. 그러면, 사본의 어떤 이전도 저작권법 아래에서 "일반적(general)"이 아니다. 

- **현지법인(subsidiaries)와 제휴사(affiliates)** : 회사는 종종 절세계획, 다른 나라에 현지를 통해 사업을 수행할 필요성, 혹은 특정 사업영역에 관여할 사업체 창설같은 다양한 전략적 이류로 사업을 수행할 제휴조직을 생성한다. 예를 들어, 특정 회사가 리눅스 커널 사본을 사용할 수도 있는데, 이 커널은 온라인 서비스 제공을 위한 목적으로 변형되었다. 이렇게 변형된 커널을 유럽 혹은 중국에 현지법인 혹은 제휴사에 현지 서비스 제공을 위해서 공급될 수도 있다. 세금, 규제, 혹은 다른 사유로 사업을 위해서 유럽 혹은 중국 영토에 서버를 위치시키는 것이 중요할 수 있다. 만약 수령 사업체가 해당 회사의 전액 출자된 현지법인이라면, 소유권 통합으로 인해서 사본이 회사 자체에만 주어지는 "사적 복제(private copy)"가 되고, 따라서 배포가 없었다는 좋은 주장을 펼칠 수 있다. 또한, 이런 주장이 과반수 소유 제휴사에 대해서도 강한 합리성을 갖는데 이유는 부모회사가 효과적으로 제휴사에 대한 제어를 하기 때문이다.[^14] 

[^14]: 추가적으로 GPL 카피레프트 요구사항은 2진 수령자가 소스 코드 사본을 구하도록 허락한다. 여기서 수령자는 과반을 소유한 제휴가사 된다. 이 쟁점은 고려할 가치가 없을 수 있다; 수령자가 단순하게 절대로 요청을 하지 않을 것이다. 

하지만, 만약 수령업체가 과반을 점하지 못하는 제휴사라면, 배포가 발생했는지에 대해서 좀더 심각한 걱정에 직면하게 된다. 이 시나리오가 꽤 흔하다. 특히 인도 혹은 중국처럼 국경 내부에서 영업하는 외국인 소유 사업에 대해서 상당한 제약을 가하는 경우에 영토안에서 과반을 점하지 못하는 사업체를 운영할 수 밖에 없다.

- **인수합병(Mergers and Acquisitions)**: 인수합병과 연관된 법률운용(operation of law)에 의한 양도 주제에 대해 미국법은 별나고 반직관적일 수 있다. 양도계약 혹은 라이선스(assignment of a contract or license)은 계약 당사자가 다른 계약 당사자에게 권리를 이전할 때 발생한다. 따라서, 예를 들면, 만약 한 기업이 다른 기업과 합의에 들어가면, 합의 결과를 다른 기업에 이전할 수도 있다 - 합의가 그것에 관해서 언급하는 바에 따라. 계약은 일반적으로 미국법 [^15] 아래서 양도가능한 것으로 간주되지만, 지적재산 라이선스는 다른 법규정의 적용받는다. 일반적으로, 특허 라이선스와 독점적이지 않은 저작권은 양도할 수 없다. [^16] 따라서, 만약 기업이 특허에 독점적이지 않은 라이선스를 수취한다면, 라이선스 합의가 명시적으로 이전을 허락하지 않는다면, 또다른 기업에 라이선스를 이전할 수 없다. 

[^15]: 특별한 유형의 계약을 제외하고, 양도는 인적용역 혹은 인적 요구사항에 대한 계약처럼 계약의 기본적 속성을 변경한다. Restatement (Sec-
ond) Contracts, Section 317 참조.
[^16]: 특허에 대해서  PPG Indus. Inv. v. Guardian Indus. Corp., 597 F.2d 1090 (6th Cir. 1979) 참조한다. 법이 충돌나지만 저작권에 대해서 예를 들어 SQL Solutions, Inc. v. Oracle Corp., 1991 U.S. Dist. LEXIS 21097 (N.D. Cal. 1991)을 참조한다. 이것은 미발표된 결정이고  Trubowich v. Riverbank Canning Co., 182 P.2d 182 (Cal. 1947)에 나온 캘리포니아 대법원 견해에 거의 틀림없이 반한다. 

문제를 좀더 복잡할 수도 있는데, 법률운용에 의한 양도가 될 수 있는 인수(심지어 목표기업체가 회생하는 후진형 삼각합병(reverse triangular merger)같은 거래조차도)를 지지하는 법원이 있다.  라이선스 피허가자가 인수 전과 후에 동일한 회사라도, 라이선스를 거래 후에 행사할 수 없을 수 있다. 배포의 정의에 대해서 법규가 영향을 끼칠 수도 있다. 만약 제어 변경이 법률운용에 의한 양도라면, 사본을 다른 기업체에 제공하는 것이 되고 따라서 카피레프트 의무를 촉발하는 배포가 된다고 논리적으로 결론낼 수도 있다. 자산매각 같은 특정 형태의 M&A 거래의 실시가 명백하게 양도가 되고, GPL 2 아래서 배포가 될 것이라는 점을 명심한다.

- **제품화(Productization)** : 이 비즈니스 사례는 법적 관점에서 볼 때 복잡하지는 않지만, 오픈소스 준법준수를 용케 해내는 회사가 자주 걸리는 덫이라 배포 분쟁의 논의에서 언급할 가치가 있다. SAAS 솔류션을 제공하는 회사는 GPL 준수를 확실히 하도록 제품을 배포하지 않는 사실에 의존하는 경향이 있다. 단순히 배포가 없는 경우조차도 요구사항을 갖는 아페로 GPL(AGPL) 같은 라이선스를 회피함으로써 준수를 업무를 수행한다. 하지만, 이런 접근법은 위험한 전략일 수 있다. 법적 기술적 세부사항에 집중하지 않는 사업개발 관리자에게, 트랜잭션(transaction)이 배포선을 넘어 걸려 쉽게 넘어지게 할 수 있다. 예를 들어, SAAS 서비스를 제공하는 회사는 매우 규제가된 시장(의료 혹은 금융같은)에서 운용되는 고객과 업무를 진행할 수 있다. 이런 경우 SAAS 서비스 제공이 고객 소유 부지에 있는 혹은 고객이 제어하는 서버에 전용 설비로 운용되어야 한다. 이런 요구는 보안 혹은 규제당국의 감사 우려에서 기인된다. 사업관점에서, SAAS 제품의 사적 인스턴스(private instance)는 기술적인 세부사항이다. 하지만, 물론 사본을 고객에게 제공하는 것은 배포가 될 것 같다. 만약 회사의 오픈소스 준수전략이 SAAS 모형 맥략에서 배포를 삼가는 것이라면, 회사는 합리적인 시간 내에서 준수 제품을 인도할 수 없음을 발견하게 된다 - 대체로 GPL과 비GPL 코드가 섞여 있거나, 제품에서 오픈소스 구성요소를 적절하게 추정하기 못하기 때문이다.

이런 극단적 사례를 명심하고서, 배포 현안을 관장하는 모범사례와 GPL 2의 의미에 대한 외적 증거에 관심을 돌려보자.

### FSF 관점

자유소프트웨어재단(Free Software Foundation, FSF)에서 공포한 GPL 2 FAQ에는 카피레프트 요구사항을 촉발하는 배포가 무엇인가에 대한 재단이 생각이 나타나 있다. 예를 들어, FAQ 중 하나는 다음과 같다:

> **Is making and using multiple copies within one organization or company “distribution”?** {.callout}
>
> No, in that case the organization is just making the copies for itself. As a consequence, a company or other organization can develop a modified version and install that version through its own facilities, without giving the staff permission to release that modified version to outsiders. 
> However, when the organization transfers copies to other organizations or individuals, that is distribution. *In particular, providing copies to contractors for use off-site is distribution [emphasis added].*[^17]


[^17]: [http://www.gnu.org/licenses/old-licenses/gpl-2.0-faq.html#InternalDistribution](http://www.gnu.org/licenses/old-licenses/gpl-2.0-faq.html#InternalDistribution). 동일한 FAQ가 GPLv3 FAQ에도 나온다([http://www.gnu.org/licenses/gpl-faq.html#InternalDistribution](http://www.gnu.org/licenses/gpl-faq.html#InternalDistribution)).

또한 FAQ는 단체와 과반을 소유한 현지법인 사이 이전도 논의한다:

> **Does moving a copy to a majority-owned, and controlled, subsidiary constitute distribution?** {.callout} 
> Whether moving a copy to or from this subsidiary constitutes “distribution” is a matter to be decided in each case under the copyright law of the appropriate jurisdiction. The GPL does not and cannot override local laws. US copyright law is not entirely clear on the point, *but appears not to consider this distribution* [emphasis added]. 
> If, in some country, this is considered distribution, and the subsidiary must receive the right to redistribute the program, that will not make a practical difference. The subsidiary is controlled by the parent company; rights or no rights, it won’t redistribute the program unless the parent company decides to do so. [^18]

[^18]: [http://www.gnu.org/licenses/old-licenses/gpl-2.0-faq.html#DistributeSubsidiary](http://www.gnu.org/licenses/old-licenses/gpl-2.0-faq.html#DistributeSubsidiary). 동일한 FAQ가 GPLv3 FAQ에도 나온다 ([http://www.gnu.org/licenses/gpl-faq.html#DistributeSubsidiary](http://www.gnu.org/licenses/gpl-faq.html#DistributeSubsidiary)).

상기 FAQ에서, FSF는 적어도 미국에서는 과반을 소유하고 과반수 지배하는 현지법인으로 혹은 현지법인으로부터의 이전은 배포를 구성하지 못한다. 더 나아가, FSF는 분석 목적으로 두 독립체가 효과적으로 한 독립체인지를 판단하는데 다른 조직체에 대해서 한 조직체의 효과적인 제어에 가중치를 준다.

기밀유지 협약서(nondisclosure agreement, NDA) 아래 변경된 GPL 코드 제공에 관한 GPL2 FAQ에 논의도 있다.

> **Does the GPL allow me to develop a modified version under a nondisclosure agreement?** {.callout}
>
> Yes. For instance, you can accept a contract to develop changes and agree not to release your changes until the client says OK. This is permitted because in this case no GPL-covered code is being distributed under an NDA. 
> You can also release your changes to the client under the GPL, but agree not to release them to anyone else unless the client says OK. In this case, too, no GPL-covered code is being distributed under an NDA, or under any additional restrictions. 
> The GPL would give the client the right to redistribute your version. In this scenario, the client will probably choose not to exercise that right, but does have the right.[^19]

[^19]: [http://www.gnu.org/licenses/old-licenses/gpl-2.0-faq.html#DevelopChangesUnderNDA](http://www.gnu.org/licenses/old-licenses/gpl-2.0-faq.html#DevelopChangesUnderNDA). 동일한 FAQ가 GPLv3 FAQ에도 나온다([http://www.gnu.org/licenses/gpl-faq.html# DevelopChangesUnderNDA](http://www.gnu.org/licenses/gpl-faq.html# DevelopChangesUnderNDA)).

많은 회사들이 배포 질문이 혼동스럽다는 것을 발견하는데 이유는 FAQ가 혼동스럽기 때문이다. 상기 FAQ에서, FSF는 두가지 다른 시나리오를 고려한다: (1) 도급업자(contractor)가 변경된 코드를 공중에게 일반적으로 고객쪽을 향해서 출시한다. 그리고 (2) 도급업자는 GPL 아래 고객에게 변경된 코드를 출시하고, 도급업자는 변경된 코드를 그밖의 누구에게도 출시하지 않겠다고 약속한다. 불행하게도, 해당 FAQ 절에는 "변경된 버젼(modified version)"이 도급업자 자신의 GPL 코드 변경을 언급하는지, 고객에 의해서 이미 변경될 수 있는 GPL 코드인지, 제3자 코드의 변경인지 명시하고 있지 않다. 분명하게, 이런 세가지 상황은 다르게 분석될 수 있다. 만약 FAQ에서 언급한 GPL 코드가 고객 혹은 도급업자가 소유한 것이라면, 사소한 질문이 된다; 분명히, GPL 코드 소유자는 적합성을 보고서 GPL 조건 혹은 GPL 조건이 아닌 것으로 코드 전달을 선택할 수 있다. 왜냐하면 (라이선스 허가자로서) 저자는 GPL 카피레프트 준수의무에 구속되어 있지 않다 - 단지 라이선스 피허가자만 구속된다. 만약 FAQ가 제3자 코드에 대한 변경을 언급한다면, 설사 최초 코드 전달이 배포를 구성하고 있다고 하더라도, 해당 배포는 GPL 카피레프트 의무를 촉발하지 않는 것을 암시한다.

FSF에서 공포한 다른 정보는 상기 FAQ 구성요소는 제3자 코드를 다루려는 의도는 없다고 제시하고 있다. 하지만, 단연코 이것이 가장 흔한 상황이다: 회사는 GPL 코드 일부를 사용하고자 하지만 변경이 필요해서, 도급을 전제로 코드를 변경할 전문가를 수소문한다. 사실, 이런 시나리오가 너무 일반적이라 오픈소스 소프트웨어의 장점 중의 하나로 내세워지고 있다. 하지만, 회사는 소프트웨어를 전혀 배포할 계획이 없을 수 있다. 따라서, 만약 코드를 컨설턴트에게 제공하는 것이 카피레프트 요건을 촉발하는 배포가 된다면, 회사는 컨설턴트를 고용하지 않을 것 같다.

FSF 관점은 몇가지 이유로 인해서 문제가 있다. 먼저, 실무적인 문제: 단순히 컨설턴트를 고용하는 회사는 사내개발과 도급개발 사업방식을 구별하지 않는다. 회사는 이런 차이에 기반하여 완전히 다른 GPL 준수 방식과 마주하길 예상하지 않는다. FSF 관점은 사업기대에 위배되기 때문에, 부주위한 사람을 위한 함정이다. 둘째로, 법적 문제: 개발목적으로 코드를 공급하는 것은 일반적인 발행 혹은 재배포의 개념보다는 "원고 콘텐츠를 명확하게 특정된 집단과 제한된 목적을 갖고, 판매, 배포, 복제, 유포의 권리 없이 (즉, 저작권법 아래서 발행이 아님)의사소통하는" 것에 좀더 가깝다. 따라서, 이러한 이전은 법률아래서 배포가 아니라는 강한 주장이 된다.

### 국제적 관점

여기서 분석되는 배포 질문은 대체로 미국법에만 볼 수 있는 독특한 것이라는 점을 명심하는 것이 중요하다. GPL2에는 준거법 선택(choice-of-law) 조항이 없고 조건부 저작권 라이선스이기 때문에, 지방 저작권법을 경유하여 보호되는 것이 좌우된다. 해당 쟁점과 연관된 국제 저작권법의 전체적인 논의는 이번 장 법위밖이지만, 이 질문에 대해서 미국밖에서 다른 대답을 갖을 듯 하다. 
베른협약(저작권의 국제적 보호를 목적으로 체결된 협약, Berne Convention for the Protection of Literary and Artistic Works)과 WIPO 저작권 조약(WIPO Copyright Treaty)에서 상술한 바에 의하면 문학작품을 "이용가능하게(make available)" 권리를 준비하고 있다. 이것은 배포에 대한 미국 개념보다 더 넓고, 더 중요하는 SAAS 제공도 포함할 수 있다. 따라서, 미국밖에 활동에 기반한 카피레프트 의무준수에 대한 촉발점이 미국내 활동보다 더 낮은 문턱을 의미할 수 있다.

### 계약문서 작성과 거래 구조화(deal structuring)에 대한 모범사례

사적영역 개업 변호사가 배포 쟁점에 대한 보통법(common law)에 명료성을 기다리듯이, 문서 작업을 하고 업무를 구조화해서 향후 법원이 배포 질문에 관한 판결을 내린다면 고객의 의도를 명료하게 하거나  결과 불확실성을 최소화 하고자 한다. 만약 상반되는 법원 선고가 있다면 그러한 업무가 모든 배포 쟁점을 처리할 수는 없다. 하지만 배포 쟁점을 평가하는데 거래와 직접 연관되지 않은 것들이 나중에 호출될 때, 이런 것이 청구신청을 억제하고, 의도에 대한 증거를 제공하거나 혼란을 줄이는데 도움이 될 수 있다.

#### 개발 합의서(Development Agreements)

개발활동이 배포가 되는가에 관한 혼란을 회피하고자, 개발합의서에 다음과 같은 문구추가를 고려해보자:

- **"도급업자는 고객 제어 아래 있는 시스템과 설비에서만 개발 서비스를 수행한다.** 이 문구는 고객이 제어하는 서버로 작업범위를 제한한다. 배포가 일어났는지에 관해서 다루는데, 이론은 설사 도급업자가 개별인이라고 하더라도, 어떤 소프트웨어 사본도 이전될 수 없다는 것이다.
- **"고객을 위해서만, 전적으로 고객에 지시한 대로, 개발 서비스를 수행하고 다른 어떤 사람이나 독립체에게 어떤 소프트웨어 사본도 이용가능하지 못하게 한다는 사실을 도급업자는 인정한다."** 이 문구는 사본이 사적 목적임을 언급함으로써 FSF FAQ가 배포로 되는 상황을 다루고 있다.

이러한 접근법이 매력적인데 이유는 관례적인 기밀 조항과 개발합의서에 "직무저작물(work made for hire)" 조항을 따르고 있기 때문이다. *CCNV v. Reid* [^20] 아래 "직무저작물(work made for hire)"로 저작물 처리를 지원하는데 개발활동에 대한 고객 제어를 나열하고 있다.

[^20]: *Community for Creative Non-Violence v. Reid,* 490 U.S. 730 (1989)

#### 인수 합병

#### SAAS 합의서

#### 회사간 합의서(Intercompany Agreements)

### 지속되는 수수께끼

미국 연방법원이 조만간 배포 질문에 대답을 제시할 것 같지는 않다. 지금까지 가져온 오픈소스 시행법령은 이런 질문을 다루지 않았다. 
(GPL2 아래 2차 저작물 범위와 특허법과 오픈소스 라이선싱의 상호작용 같은) 다른 자극적인 쟁점이 오픈소스 법에서 여전히 명확하지 않은 상황에서, 논쟁은 아직 무르익지 않았다. 또한, GPL2 아래 코드를 출시하는 저자 대부분은 회사간 합의서와 인수 혹은 합병 같은 쟁점에 단순히 초점을 맞추지 않고 있다. 이유는 주로 저자들이 기업 전략가라기 보다는 기술자이기 때문이다. 만약 GPL 저자가 
