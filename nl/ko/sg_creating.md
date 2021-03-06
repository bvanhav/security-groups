---



저작권:
  연도: 2017년
마지막 업데이트 날짜: "2017-04-27"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# 보안 그룹 및 규칙 작성(베타)
{: #creating-security-groups}

보안 그룹 및 이와 연관된 규칙을 작성한 후 하나 이상의 가상 서버 인스턴스 인터페이스에 지정하여 가상 방화벽을 사용으로 설정할 수 있습니다.
{:shortdesc}

## 보안 그룹 작성

보안 그룹을 작성하려면 다음 단계를 완료하십시오.
{:shortdesc}
 
1. [고객 포털 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://control.softlayer.com/) 탐색에서 **보안 -> 네트워크 보안 -> 보안 그룹**을 선택하십시오.
2. 보안 그룹 페이지에서 **그룹 작성**을 클릭하십시오.
3. 보안 그룹의 이름 및 설명을 입력하고 **그룹 작성**을 다시 클릭하십시오.

**참고:** 기본적으로 "모든 아웃바운드 트래픽을 허용하는 기본 규칙으로 그룹 작성"이 선택됩니다. 이 필드를 선택 취소하여 규칙이 없는 보안 그룹을 작성할 수 있습니다. 규칙이 없는 보안 그룹은 모든 트래픽(인바운드 및 아웃바운드 모두)을 차단합니다.

## 보안 그룹 규칙 작성

보안 그룹 규칙을 작성하려면 다음 단계를 완료하십시오.
{:shortdesc}

1. [고객 포털 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://control.softlayer.com/) 탐색에서 **보안 -> 네트워크 보안 -> 보안 그룹**을 선택하십시오.
2. 보안 그룹 페이지에서 보안 그룹 이름을 클릭하여 세부사항 페이지를 여십시오.
3. 보안 그룹 세부사항 페이지에서 해당 조치(예: 방향, IP 유형, 프로토콜 및 소스/대상 정보)를 모두 입력하십시오. 완료되면 **규칙 작성**을 클릭하십시오.

**참고**: 소스 및 대상 필드에는 CIDR(Classless Inter-Domain Routing) 블록 또는 보안 그룹을 지정할 수 있습니다. 

CIDR 블록은 IP 주소 블록의 라우팅을 용이하게 합니다. CIDR을 유형으로 선택하는 경우 IP 주소 범위를 지정해야 합니다. 

보안 그룹을 유형으로 선택하는 경우 기존 보안 그룹 목록에서 선택해야 합니다. 이 경우 선택한 보안 그룹에 연결된 디바이스의 IP 주소를 선택할 수 있습니다. 가상 서버가 여러 IP 주소를 보유하도록 구성된 경우 기본 IPv4 및 IPv6 주소만 이러한 원격 보안 그룹 규칙에서 사용됩니다.
