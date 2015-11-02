---
layout: page
title: 비즈니스를 위한 오픈 소스 소프트웨어
subtitle: 5장 조건부 라이선싱
---

오픈소스 라이선스는 조건부 라이선스(conditional license)다. 이 개념이 오픈소스 초보자가 이해하기 가장 어려운 것 중 하나고 
개념이해의 중요성을 주장하는 것이 단순히 엄격하게 규칙을 찾는 것은 아니다. 이런 개념에 대한 불명확함으로 인해 오픈소스 라이선싱에 대한 심각한 오해가 분명히 드러나고 있다. 플라톤 동굴의 비유처럼, 조건부 라이선스에 관한 오해가 실제적 위험보다 더 커다란 공포를 불러일으키고 있다. 일부 사람은 GPL을 "바이러스(viral)"로 칭하지만, 이 단어의 사용은 단지 정치적 부정확과 미사여구에 불과한다; 오픈소스 소프트웨어를 사용에 동반된 위험을 과정한다. 오픈소스 라이선스 논의에서 *바이러스(viral)* 단어를 제거는 오래전에 행해졌어야 하는데 이유는 이 단어가 오픈소스 라이선싱 원칙에 대한 이해를 왜곡하고 제한하기 때문이다.[^1]

[^1]: 저자는 이 단어가 일반적으로 자유 소프트웨어와, 특히 GPL과 어떻게 연관되기 시작했는지에 관해서 몇가지 이야기를 들었다. 하지만, 확증할 수가 없어서 여기서 언급하지는 않는다.


### 바이러스가 아니고 버그다

저자가 고객으로부터 가장 받는 질문 하나는 "오픈소스가 자사의 독점 코드를 어떻게 오염시키지 못하도록 만들 수 있을까요?" 대답은 쉽다: 오픈소스는 귀사의 독점 코드를 오염시킬 수가 없습니다. 단순하게 오픈소스가 독점적 코드를 오염시킬 수 있는 그럴듯한 법적 논쟁이 없다. 하지만, 이번 장에서 왜 오해가 없어지지 않고 지속되는지, 왜 조건부 라이선싱 모형이 GPL 위반에 대해 최악의 시나리오를 제한하는지, 이런 질문을 자세하게 살펴볼 것이다. 

GPL 코드를 독점 코드와 통합하고 나서 GPL이 아닌 다른 조건으로 조합된 코드를 배포하면 GPL 위반이 가능하다. 머리속에 바이러스가 춤을 추는 상상을 하는 개발자는 GPL과 독점 코드가 조합되어 단일 프로그램이 되면, GPL 라이선싱 조건이 독점 코드를 "감염(infect)"시켜서 독점 코드가 자동으로 GPL로 라이선스된다는 걱정을 한다. 그리고 나서 개발자는 본인 독점 소스코드를 제공할 의무를 지게된다고 걱정을 한다.

대부분의 독점코드 개발자에게 이것은 그저 선택의 문제가 아니다. 이렇게 하게 되는 것은 독점 코드의 가치를 평가절하함으로써 주주(shareholder)에 대한 선량한 관리자의 주의의무를 위반할 뿐만 아니라, 제3자 라이선스도 아마 위반하게 된다. 특정 회사의 독점적 제품은 통상 독점 조건아래 2차 라이선스되는 제3자 소프트웨어를 포함한다. 따라서, 설사 원한다고 하더라도, 특정 회사가 해당 제품을 GPL로 변경할 권리는 없다.

하지만, "감염(infection)"이 카파레프트가 동작하는 방식은 아니다. 사실, 만약 개발자가 GPL을 위반하는 방식으로 GPL과 독점 코드를 조합하고 나면, 결과는 GPL 위반이 된다 - 그 이상도 이 이하도 아니다. (그리고 만약 개발자가 제3자 GPL 코드를 제3자 독점 코드와 조합한다면, 아마도 인입되는 두 라이선스 모두 위반이 될 것이다.) 법률적으로 이것이 함의하는 바는 GPL 코드 저자는 GPL 위반에 대한 구제방법과 만약 만약 라이선스가 결과로 종료되면, GPL 소프트웨어에 대한 허가되지않은 라이선스 사용에 대한 구제방법이 있다. 본질적으로, 두가지 가능성 모두 저작권 위반 청구 대상이 된다. 저작권 위반 청구에 대한 구제방법은 손해 배상(돈)과 법원명령(GPL 코드 사용 중단)이 있다.

사실 단순하게 GPL이 다른 코드에 대한 라이선싱 조건을 변경하는 법적 매커니즘은 없다. 소프트웨어가 특정 조건아래 라이선스되기 위해서는 다음을 만족해야 한다.특정 조건아래 코드를 제공하기 위해서 저자는 일리있는 행동을 취해 라이선스 사용 허가를 받은 사람과 라이선스 부여하는 사람 사이 라이선스 체결이 되도록 이끌어야 한다. 그에 반해서 독점 코드와 GPL 코드를 단일 프로그램에서 GPL 위반되는 방식으로 조합하면 라이선스 비호환이 된다 - 두 조건이 충돌나서 동시에 만족될 수 없다. 이런 유형의 라이선싱 비환성에 대한 좀더 좋은 비유는 소프트웨어 바이러스가 아니라, 소프트웨어 버그다.  

### 조건부 라이선스는 무엇인가?

GPL과 거의 모든 오픈소스 라이선스는 동시에 저작권 라이선서를 해당 라이선스 조건으로 코드를 수취하려는 모든 사람에게 부여된다. 하지만, 해당 라이선스는 요구사항을 준수하는 조건으로 한다. 이런 요구사항 범위는 (방임 라이선스에 대해서) 라이선스 고지부터 (카피레프트 라이선스에 대해서) 카피레프트 조건(소스코드 공개)까지 아우른다. 만약 이런 조건이 위반되면, 라이선스는 종료된다.

이런 아이디어에 고생하는 한가지 이유는 오픈소스 영역을 외에는 그다지 일반적이지 않기 때문이다. 변호사에게 가장 친숙한 비유는 아마도 편무계약(unilateral contract)일 것이다. 모든 로스쿨(law school) 계약법 수업은 다음 가상적인 사례로 시작된다: "만약 당신이 다리를 건넌다면, 나는 당신에게 $10 달러를 줄 것이다." 당신이 다리를 건널 때, $10 달러를 지불 의무가 있다. 하지만, 오픈소스 라이선싱은 정반대다. "이 작업을 수행하면 내가 당신을 보상해줄께" 라고 말하는 대신에, 오픈소스 라이선싱은 "이 요긴한 것을 못된 짓을 할 때까지 즐거라"라고 말하고 있따. 법적으로 다르다.

### 라이선스 혹은 계약?


오픈소스 추종하시는 분이 오픈소소 라이선스는 "계약이 아님"이라고 말하는 것을 들을 수 있다. 좀더 좋은 분석은 오픈소스 라이선스는 반듯이 계약이 아니라는 것이지만, 이것이 오픈소스 라이선스가 결코 계약이 될 수 없다고 말하는 것과 같지 않다. 라이선스 혹은 계약? 이 문제를 제기하는 것은 쟁점을 너무 단순화한다. 하지만, 먼저 계약과 조건부 라이선스 사이 차이를 이해하자.

*계약(contract)*은 전제(premise)의 집합이다. 법률에 따르면, 제안(offer), 승인(acceptance), 보답(consideration)이 있을 때 계약이 구성된다. 보답은 약속에 대해 교환되는 가치있는 무엇이다. 각 당사자가 무언가를 약속하지 않았다면 법은 계약을 인식하고 집행하지 않는다. (그렇지 않다면, 이런 합의를 *증여(gift)*라고 부른다.) 법에서 이런 합의가 공평 혹은 균등함이 요구하지 않고,[^2] 당사자가 의도한 것만 따진다. 보답에 대한 한가지 형태가 관용(forbearance)이다 - 당사자가 권리를 갖고 무언가 할 수 있음.[^3]

[^2]: 법에서 보답을 "말린 후추열매(peppercorn)"로 종종 불린다 - 다른 말로, 주어진 것이 가치가 있는지 그다지 중요하지 않는다. 그래서 후추면 충분할 것이다. 많은 법률 용어처럼, *말린후추열매*는 최초 의미보다도 더 오래 지속되었다. 용어가 처음 만들어질 당시, 후추는 값비싼 수입 사치재였다. Restatement (Second) Contracts 79절 참조.

[^3]: 예시로 협연을 하지 않은 것에 대해서 돈을 지불하는 것. Restatement (Second) Contracts 71절 참조.

따라서 항상 라이선스 계약은 관용을 수반하는데 이유는 라이선스가 지적재산 침해에 대해서 소송하지 않겠다는 약속이기 때문이다. 라이선스 허여자는 소송하지 않겠다고 약속하고, 라이선스를 부여받은 자는 라이선스 비용처럼 그 댓가로 지불을 약속한다. 대부분의 지식재산 변호사는 이런 모형에 익숙하다. 하지만, 오픈소스 라이선스는 미묘하게 다르다.

오픈소스 라이선스에서 라이선스를 사용하는 사람에게 그 자체로 부과된 보답은 없다. 대신에 라이선스 행사에 대한 조건이 있다. 라이선스를 사용하는 사람이 이런 조건을 지키기만 하면, 라이선스 사용을 부여받은 사람을 라이선스를 계속해서 행사할 수 있다. 만약 라이선스를 사용하는 사람이 조건을 위반하면, 라이선스는 사라지고, 라이선스 허여자는 위반에 대해서 자유로이 소송할 수 있다.

조건부 라이선스와 계약 사이 차이는 미묘하지만 중요하다. 계약에서 각 당사자는 약속을 한다. 만약 한 당사자가 약속을 어기면, 법원은 약속을 이행하도록 명령한다. 실은, 법원이 실제로 약속을 이행하도록 거의 명령하지 않는다. 만약 누군가 계약을 위반하면, 법원이 위반한 당사자에게 피해보상금을 지불하도록 명령한다. 사실, 법이 그밖의 어떤 것도 거의 지원하지는 않는다. 해당 당사자가 실제로 이행하도록 하는 명령을 *특정 이행(specific performance)*이라고 부른다. 부동산 공매같은 제한된 상황에서만 지원되는 예외적인 구제방법이다. 대부분의 경우에, 계약 위반은 순수하게 상업적 손해로 간주되고, 따라서, 유일한 구제방법이 돈이다. 이 개념은 중요하고, 관습법 국가에서 기본적인 정치적 자유 전제를 언급하고 있다. (범죄와 대조적으로) 권리침해(civil wrong)에 대해서, 처벌은 금전 지불 혹은 중지명령이다. 법원이 예외적인 경우를 제외하고 확신하는 행동(positive action)을 명령할 수 없다는 것이 정치적 자유에 대한 미국의 중요한 원리다.[^4]

[^4]: 형법에서, 법원은 개인적 자유를 제한하는데 구금하거나 다른 조치를 취할 수 있다. 하지만, 형법은 개인보다는 사회에 대한 해악을 바로 잡으려고하기 때문에 다르다. 따라서, 민법에서는 가용하지 않는 구제방법을 갖추고 있다.

조건부 라이선스에서, 라이선스 사용자는 어떤 것을 수행하는데 약속을 하지 않는다. 사실, 오픈소스 라이선스는 행사할지 않을지에 대해 권리를 부여한다. 라이선스 허여자는 코드를 GPL 라이선스 아래 출시하는 순간, 저자, 독자, 그리고 그밖의 모든 이가 해당 라이선스 조건으로 사용허락된다. 하지만, 실제 라이선스 권리 행사는 조건이 있다: 라이선스 사용허락을 받은 자는 라이선스 조건을 준수해야 한다. 그렇지 않으면 라이선스는 상실된다. GPL 2 5절에 다음과 같이 언급하고 있다.

~~~ {.python}
You are not required to accept this License, since you have not signed it. However, nothing else grants you permission to modify or distribute the Program or its derivative works. These actions are prohibited by law if you do not accept this License. Therefore, by modifying or distributing the Program (or any work based on the Program), you indicate your acceptance of this License to do so, and all its terms and conditions for copying, distributing or modifying the Program or works based on it. 
~~~

하지만, 실제로 이것이 계약을 만들려는 시도라기 보다는 라이선스 사용자가 조건을 준수하거나 라이선스를 포기해야 되다는 것을 설명하고 있다.

만약 이런 관점이 고문처럼 괴로워 보인다면, 어쩐면 그럴 것이다. "계약되지 않는 라이선스(license not contract)" 입장에 대해서 1990년대 GPL 2와 나란히 선구적으로 탐구되었다. 90년대 초반에 온라인 계약구성에 관한 법은 여전히 해결되지 않았다. 전통적으로, 계약에 들어감은 서면으로된 서명(written signature)을 수반한다 - 이것이 계약 조건에 대한 동의를 표현하는 수단이다. 하지만, 소프트웨어 산업이 성장함에 따라, 소프트웨어 개발자는 종이 문서와 서명이 필요없는 라이선스 동의 조건을 확립하려는 방법을 모색했다. "소프트웨어 제품 동의(shrink-wrap)" 혹은 "마우스 클릭 동의(click-to-accpet)" 라이선스가 1990년대까지 일반적인 관행이였고, 계약을 구성하는데 있어 이런 방법의 효험은 아직 법원에서 공식화되지 않았다. 그리고 나서 1996년, 서명되지 않은 합의에 대한 시행가능성을 옹호하는 획기적인 의견이 발표됐다.[^5] 하지만, 이런 방식으로 계약을 구성하는 것은 여전히 라이선스 허여자가 장애물을 넘어야 되도록 요구하고 있다. 예를 들어, 라이선스 사용자로부터 "동의함(I agree)" 행위를 강제하는 설치자(installer) 혹은 다운로드 관리자(downloader) 구현이 요구된다. 오픈소스 소프트웨어는 이러한 기술적인 메커니즘 없이 한 수령자에게서 다른 수령자로 종종 전달된다. 그래서 라이선스 조건이 계약을 구성할 필요없이 법적 수용절차(legal traction)를 가질 필요가 있다. 이점에 대해 조건부 라이선스 모형은 잘 작동한다. 왜냐하면 라이선스 사용자를 언제, 어디서, 어떤 방식으로 사용하는지 관계없이 그리고 라이선스 사용자 신원과 소프트웨어를 받은 수단에 관계없이, 라이선스 허가자에게 소프트웨어의 특정한 사용을 배제하는 권한을 부여한 저작권법으로부터 권한을 가져왔기 때문이다.


[^5]: *ProCD v. Zeidenberg*, 86 F.3d 1447 (7th Cir. 1996).

### 조건부 라이선싱 모형의 함의

조건부 라이선싱 모형은 두가지 주요 함의를 갖는다. 첫째로, 이 모형은 계약 모형아래 가능한 것과 다른 구제방법을 제공한다. 둘째로, 조건부 라이선싱 모형은 재배포자와 수령자 사이 당사자 관계(privity)를 만들지 않는다. 따라서 소프트웨어 원저작자에 시행 권리와 의무를 부여한다. 

#### 구제방법

저작권 침해과 계약 위반에 구제방법은 매우 다르다. 미국에서 저작권 침해에 대한 손해배상은 "침해결과로 겪었던 실제 손해와 침해자의 이득"이 된다. 침해자 이득을 규명하는데 있어, 저작권 소유자는 침해자의 총수입만 증명하면 된다. 침해자는 공제비용과 저작물이 아닌 요인에 기인하는 이득 요소를 증명하도록 하고 있다. [^6] 저작권 원고는 대안으로 저작권으로 보호를 받는 작품마다 "법원이 공정하다고 판단으로" $750에서 $30,000까지 "법정손해배상(statutory damages)"을 선택할 수 있다. 만약 원고가 침해를 고의적으로 저질렀다는 점을 증명하면, 손해배상은 $150,000까지 상향될 수 있다. 저작물이 시기적절한 때에 저작권위원회(copyright office)에 등록될 때만 법정손해배상은 가능하다.

[^6]: 17 USC 504.

대조적으로, 계약법은 권리침해를 당한 당사자가 전보배상(compensatory damage)만 허용한다.[^7]
이들 손해배상은 경제적 손해에 집중하고, 감정적 손해, 육체적 정신적 고통에 대한 배상은 포함되지 않는다(불법행위법(tort law) 개념이다). 만약 계약을 위반하면, 예상 손해(또다른 상대방이 계약으로부터 받기 개대되는 수익), 간접손해(계약 위반으로 발생되는 사업 상실 혹은 평판 실추), 배상(계약위반 당사자의 부당이익을 방지하기 위한 공정한 계산)에 대한 지불이 예상된다.

또한 저작권은 구제방법으로 법원명령(injunction)도 제안한다. 법원명령은 법원이 침해를 중지시키는 명령이다. 법원명령이 가능할 때, 저작권법 아래 법원은 네가지 요인을 갖는 시험을 도입한다: (1) 본안 사건에 대한 원고의 승소 가능성; (2) 법원명령 부재에 회복할 수 없는 손해 (즉, 손해가 나중에 금전적 손해배상으로 적절히 상쇄될 수 없다); (3) 원고와 피고 사이 고난의 균형; (4) 공공의 이익.[^8] 계약 청구에서, 법원명령은 거의 이용되지 않는 이례적인 구제방법이다.

[^7]: 계약법에서 징벌적 손해배상(punitive damage)은 극도로 드물다.
[^8]:  Metro-Goldwyn Mayer, Inc. v. 007 Safety Products, Inc., 183 F.3d 10, 15 n.2 (1st Cir. 1999) 을 참조한다.

보시다시피, 저작권 위반에 대한 금전 손해 배상금은 적어도 계약 위반에 대한 것만큼 폭넓고, 저작권은 법정손해배상과 법원명령 가능성을 추가한다. 이것이 오픈소스 라이선싱에 중요하다. 오픈소스 라이선싱에서 경제적 손해는 증명하기 어려울 수 있다. 오픈소스 라이선스 허여자는 소프트웨어를 저작권 사용료(royalty) 없이 나눠줬다. 그래서 라이선스 허가자의 손해는 조건 위반으로부터 누적된다. 조건 위반은 주로 고지위반과 소스코드 공개 요건이다. 이런 조건을 만족시키지 못한 것에 대해 손해를 경제적인 가치로 산정하기는 어려울 수 있고 저작권법은 라이선스 허가자가 다른 구제방법을 선택할 수 있게 하고 있다. 따라서, 계약 손해배상금에 대한 가능성을 포기하는 것이 라이선스 허가자에게 있어 실질적인 손실은 아니다.

바이러스 모형은 특정이행(specific performance)이 계약 구제방법으로 이용가능하다는 가정에 기초하고 있다. 오픈소스 라이선스에 대해서 이일이 일어나기 위해서, 계약이 구성될 필요가 있을 것이다. 소스코드 전달 조건이 라이선스 피허가자의 계약의무로 해석될 필요도 있을 것이다. 가장 중요하게, 법원이 이런 의무에 대한 특정이행을 명령할 필요가 있을 것이다. 하지만, 상기 분석으로부터 볼 수 있듯이, 이것은 결코 발생되면 안된다. 카피레프트 라이선스 아래 어떤 라이선스 피허가자도 오픈소스 코드를 깔도록 명령받지 않은 것이다. 그리고 저작권은 절대로 그런 구제방법을 제시하지 않는다. 그래서, 오픈소스 라이선스 위반에 대해서 그런 구제방법으로는 가능성있는 근거가 못 된다.

#### 당사자 관계(privity)

조건부 라이선싱 모형에 두번째 필연적인 결과는 라이선스 허가자 혹은 저작권 소유자가 항상 라이선스를 집행하는 사람이 된다는 점이다. 이점이 다소 직관에 어긋하는 패러다임을 이끌게 된다. 만약 누군가 GPL 코드를 갖고, 변형하고 나서, 변형된 코드 제공을 거절한다면, 수령자는 어떤 법적청구권도 없다. 대신에 청구권을 계속 추구할 권리를 갖는 사람은 GPL 코드 라이선스 허가자다.

미국에서, 저작권 소유자 혹은 독점적인 라이선스 피허가자만이 저작권 침해에 대한 소송을 주장할 수 있다.[^9] 조건부 라이선싱 패러다임은 라이선스 허가자가 미리 라이선스 피허가자 신원을 식별하지 않고 집행을 추구할 수 있도록 한다. 만약 오픈소스 라이선스가 계약으로 집행되면, 저작권자는 집행하려면 배포 채널부터 협업이 필요할 수 있다. 어떤 계약도 라이선스 원허가자가 아닌 수용자와 배포자 사이 구성될 수 있을 것이다. 재배포자가 라이선스 조건을 집행할 유인책(incentive)은 거의 없거나, 선택적으로 상업적 이득을 위해서 할 수도 있다. 그래서 조건부 라이선싱 모형이 계약모형보다 더 많이 오픈소스 저자에게 힘을 실어주게 된다.

[^9]: 17 USC Section 501(b) says, “The legal or beneficial owner of an exclusive right under a copyright is entitled … to institute an action for any infringement of that particular right committed while he or she is the owner of it.” Courts have held this statement to be exclusive under the doctrine of expressio unius est exclusio alterius. 예를 들어 *Silvers v. Sony Pictures Entertainment, Inc.*, 402 F.3d 881 (9th Cir. 2005) (en banc)를 참조한다.

상기 분석이 바이러스 오류와 조건부 라이선싱에 관해서 알 필요가 있는 것에 대한 이해을 충분히 줘서 도움이 되었을 것이다. 이번 장의 나머지는 이 쟁점을 둘러싼 법적인 상세한 점에 관심있는 독자를 위해서, 좀더 자세한 법적 분석을 담고 있다. 

### 계약의 성립 (contact formation)

앞에서 대략 제시되었듯이, 대부분 GPL 라이선스 허가자는 위반을 계약위반보다는 저작권 침해로 제시할 것이다. 하지만, 오픈소스 라이선스는 절대적으로 "계약이 아님"이라고 말하는 사람은 아마도 틀렸다. 많은 경우에 정반대로, 계약이 성립되었다는 것을 증명하기는 쉬울 수 있지만, 누구와 어떤 방식으로 성립되었는지 증명하기는 매우 복잡하다.

만약 누군가 계약이 성립됐음을 규정하려고 한다면, 그런 견해를 지지하는 것은 많다. 대부분의 오픈소스 라이선스의 명시조건은 문서가 계약임을 제시한다. 오픈소스 라이선스 대부분은 UCC 제2조에서 통계하는 물품매매계약에만 적용되는 UCC 품질보증 권리포기각서 (warranty disclaimers)[^10]를 담고 있다. 만약 참이면, GPL2 5절 "이 라이선스 수락을 표시한다(You indicate your acceptance of this License)" 문장이 계약을 성립한다. 가정하는 것은 제안이 있었고, 보답이 이미 존재했음이다. 하지만, 가장 중요하게는 조건의 수락을 둘러싼 상황이 계약의 성립을 지지하는데 충분할 수도 있다는 것이다.[^11] 만약 소프트웨어를 다운로드할 수 있다면 제안이 있었다는 것은 명확하다. 보답도 충분하다 - 라이선스 허가자는 침해소송 포기를 제안했고, 라이선스 피허가자도 조건을 준수해야만 한다. 계약성립의 가장 도전이 되는 항목이 승인이다. "그런 계약의 존재를 인식한 쌍방에 의한 행위를 포함"함으로써 승인이 나타날 수 있다고 UCC는 규정하고 있다. 또한 그런 행위는 증명하기 쉬울 것도 같다.

[^10]: 예를 들어 GPL2 11절.
[^11]: UCC 제2절, 1-204절.


#### 성립 논쟁에 대한 유인책

그리고 나면, 확실한 질문이 만약 행위를 경유한 승인을 보여주는 것이 그렇게 쉽다면, *Pro*CD 사례까지 이르게 되는 질풍노도(Strum und Drang)가 왜 그렇게 많느냐는 점이다. 오픈소스 라이선스 범위와 EULA 범위가 매우 다름을 명심하는 것이 중요하다. 따라서, 독점적 소프트웨어와 오픈소스 소프트웨어 수용자는 라이선스 조건을 회피하는데 매우 다른 유인책을 갖는다. 

합법적으로 소프트웨어 사본을 소지한 사람은 백업 사본(17 USC Section 1117(a)(2))과,소프트웨어를 실행하는데 필요한 일시적 사본(under 17 USC 1117(a)(1))을 생성할 권리를 갖는다. 부가적으로, 배경법(background law) 아래서 소프트웨어 사본을 구매한 사람은 [최초판매의 원칙](http://terms.naver.com/entry.nhn?docId=638931&cid=42143&categoryId=42143)(the first sale doctrine, 17 USC Section 109) 적용할 수 있고, (공정한 사용인 제한된 일부 상황에서) 소프트웨어를 역공학하는데 필요한 사본을 만들 수 있고, UCC 2-316절 아래 [묵시담보](http://terms.naver.com/entry.nhn?docId=1227658&cid=40942&categoryId=31831)(implied warranty)를 향유할 수 있다.

만약 전형적인 최종 사용자 라이선스를 읽어보면, 이런 행동 대부분이 "허락"됨을 알게 된다. 물론, 이런 행동이 허락될 필요는 없는데 이유는 우선 저작권 위반이 아니라고 저작권법에서 언급하고 있기 때문이다. 라이선스는 지적재산 침해에 대해 소송하기 않겠다는 단지 약속일 뿐이라는 것을 기억하라. 대부분 최종 사용자 라이선스는 역공학을 금지하고, 라이선스 허가자에 대한 법적책임을 부인하고, 라이선스 피허가자가 누리는 품질보증을 제한한다. 따라서, 최종사용자는 계약을 승인하면 더 좋지 못한 위치에 서게 된다.

하지만, 단순한 사용을 넘어서는 권리를 행사하려는 사람은 다른 입장에 위치하게 된다. 소프트웨어를 변경하거나 배포할 어떤 배경 권리(background right)도 없다. 그래서, 만약 소프트웨어 수령자가 이러한 권리를 향유하려면, 라이선스를 받아야만 된다. 이것이  왜 계약성립 전쟁이 1990년대 EULA에 대해서 했던 방식으로, 오픈소스에 대해서 구체화되지 못한 이유다. 살펴봤듯이, 라이선스 허가자는 계약 클레임에 대한 필요가 거의 없고, 라이선스 피허가자는 라이선스를 필요로 한다.

하지만, 계약 구제방법이 오픈소스 라이선스 피허가자에게 절대로 가능하지 않다고 가정하는 것은 현명하지 않을 것이다. 사실, 오픈소스 라이선스 위반에 대한 소송은 옳건 그르건 계약 클레임으로 종종 제기된다. [^13]

 [^13]:  Progress Software Corp. v. MySQL AB, 195 F. Supp. 2d 328 (D. Mass. 2002); MontaVista Software, Inc. v. Lineo, Inc., No. 2:02 CV-0309J (D. Utah filed July 23, 2002)를 참조한다.

물론, GPL이 라이선스 혹은 계약인지 묻는 것은 GPL이 라이선스이거나 계약이 되어야 된다는 가정이 있다. 분명히, GPL은 라이선스이지만 계약일수도 계약이 아닐 수도 있다. 문서가 그 자체로 계약은 아니다; 문서는 계약 조건을 담을 수 있지만, 계약은 행위로 성립된다. 점선 위에 서명을 하건, "동의함(I accept)"을 클릭하건, 소프트웨어를 다운로드하건, 계약은 제안, 승인, 보답으로 구성된다 - 그리고 오픈소스 라이선싱이 이것을 바꾸지는 않는다.

### 바이러스 박멸

저자는 바이러스 모형에 대한 어떤 형식적 법적 기반을 찾으려고 방심하지 않고 주의를 기울여 왔다. 저자가 찾은 유일한 사례는 Pickett v. Prince, 207 F. 3d 402 (7th Cir. 2000) 그리고 Anderson v. Stallone, 11 USPQ2D 1161 (C.D. Cal. 1989)이다. 두가지 사례 모두 인가받지 못한 파생저작물이 저작권 보호을 받을 자격이 있는가에 대한 원칙을 논의하다.

하지만 이들 사례 모두 전형적인 GPL 준수 문제와는 매우 다른 사실과 연관된다. 먼저, 각 사례의 경우 침해하는 파생 저작물이 아마도 법적 보호를 위해 필요한 창의성 임계수준을 아마도 만족시키지 못했다. 법률은 이 임계수준을 매우 낮게 설정하고 있다. 임의 상업적 가치를 갖는 어떤 독점 코드도 쉽게 임계치를 만족한다. 둘째, 각 사례의 경우 침해하는 파생저작물의 소유자로 추정되는 인물이 침해된 기반 저작물의 저자를 고소하려 시도했다 - 구식이지만 상당히 훌륭한 당돌함을 요구하는 무언가. 
GPL과 적절하게 조합될 수 없었던 독점적 소프트웨어 모듈 개발자가 제3자를 상대로 분리된 독점 코드에 권리를 집행하려는 상황에 대해서 이러한 사실로부터 합리적 추론을 할 수 없다.
독점적 소프트웨어 개발자가 GPL 코드 일부를 끄집어 내고, 한 줄 변경하고 나서, 저작권 침해로 GPL 저자를 고소하는 경우에 비유될 수 있다 - 물론 말도 안되는 소리다.

마지막으로, 설사 승인되지 않은 파생저작물이 저작권 보호를 받을 자격이 없다는 원칙을 지지하고 있을지라도 이런 사례를 통해서 독점적 저작물은 GPL 대상이라기 보다는 공공영역(public domain)에 있음을 나타내고 있다. 사실 이것은 매우 무서운 결과다 - 다행히 법적으로 단순히 옹호되지는 않고 있다.
