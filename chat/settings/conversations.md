# 상담 설정

## 답변 추천 {#recommended-answer}

{% hint style="danger" %}
\*\*\*\*[**마스터**](../overview.md#undefined-1)만 설정할 수 있습니다.
{% endhint %}

{% hint style="info" %}
프로필 별로 각각 설정할 수 있습니다
{% endhint %}

![&#xB2F5;&#xBCC0; &#xCD94;&#xCC9C; &#xC124;&#xC815; &#xD654;&#xBA74; &#xC608;&#xC2DC;](../../.gitbook/assets/undefined%20%2818%29.png)

상담원들의 답변의 정확도를 높이기 위해 고객이 자주 묻는 질문과 답변들을 Microsoft의 QnA Maker나 IBM의 Watson에서 설정하여 연동할 수 있습니다.  
답변 추천을 설정하면 채팅창에서 고객이 질의한 내용을 선택하면 그에 알맞은 답변을 상담원이 확인하여 활용할 수 있습니다.

### Microsoft QnA Maker



![Microsoft QnA Maker &#xC124;&#xC815; &#xD654;&#xBA74; &#xC608;&#xC2DC;](../../.gitbook/assets/qna.png)

* Microsoft QnA Maker에서 질문 답변을 설정하고 QnA Maker에서 제공하는 정보를 입력합니다

### IBM Watson

![IBM Watson &#xC124;&#xC815; &#xD654;&#xBA74; &#xC608;&#xC2DC;](../../.gitbook/assets/watson.png)

* IBM Watson에서 질문과 답변을 설정하고 Wastson에서 제공하는 정보를 입력합니

## 커스텀 웹 패널 {#custom-web-panel}

{% hint style="danger" %}
\*\*\*\*[**마스터**](../overview.md#undefined-1)만 설정할 수 있습니다.
{% endhint %}

{% hint style="info" %}
프로필 별로 각각 설정할 수 있습니다
{% endhint %}

![&#xCEE4;&#xC2A4;&#xD140; &#xC6F9; &#xD328;&#xB110; &#xC124;&#xC815; &#xD654;&#xBA74; &#xC608;&#xC2DC;](../../.gitbook/assets/undefined%20%281%29.png)

상담에 필요한 도구가 추가적으로 필요한 경우, 고객님께서 작성하신 웹 앱을 커스텀 패널로 설정할 수 있습니다. 예를 들어, 기존 고객관리 페이지를 커스텀 패널로 설정하시면 상담원이 상담 화면을 벗어나지 않고도 고객정보를 확인할 수 있게 됩니다.

{% hint style="info" %}
Custom panel은 sandboxed iframe 으로 구현되어 있으며,   
보안상의 이유로 HTTP Cookie나 CORS가 설정된 https 리소스 등은 사용할 수 없습니다.

iframe sandbox attribute에는 다음 네 가지 옵션만 활성화되어 있습니다.

* **allow-scripts**: javascript 활성화
* **allow-popups**: window.open \(target=\_blank\) 활성화 
* **allow-modals**: window.alert, window.confirm, window.prompt, window.print 활성화
* **allow-forms**: form submit 활성화

이에 대한 자세한 내용은 다음 문서를 참고해 주세요.

* [https://html.spec.whatwg.org/multipage/origin.html\#sandboxing-flag-set](https://html.spec.whatwg.org/multipage/origin.html#sandboxing-flag-set)
* [https://developer.mozilla.org/ko/docs/Web/HTML/Element/iframe](https://developer.mozilla.org/ko/docs/Web/HTML/Element/iframe) 
{% endhint %}

## 상담 완료 설정 {#completed-call}

{% hint style="danger" %}
\*\*\*\*[**마스터**](../overview.md#undefined-1)만 설정할 수 있습니다.
{% endhint %}

{% hint style="info" %}
프로필에만 설정할 수 있습니다.
{% endhint %}

![&#xC0C1;&#xB2F4; &#xC644;&#xB8CC; &#xC124;&#xC815; &#xD654;&#xBA74; &#xC608;&#xC2DC;](../../.gitbook/assets/undefined%20%283%29.png)

상담 완료 설정 화면에서는 상담원이 상담을 완료했을 때의 동작을 설정할 수 있습니다.   
만일 미리 **만족도 조사 플로우**를 작성해 놓은 상태라면 상담원이 상담을 완료했을 때 챗봇에게 사용자의 만족도를 물어보도록 해당 플로우로 전환시키는 기능입니다.

만일 상담 완료 시 플로우 변경 기능을 **사용하지 않음**으로 설정하신다면 상담 완료 시의 동작은 다음과 같습니다.

* 상담원 호출 노드를 통해 상담이 시작된 경우: 상담원 호출 노드에서 재시작
* 상담원의 개입을 통해 상담이 시작된 경우: 처음부터 재시작
* 상담원이 상담 도중 챗봇으로 전환하고 상담을 완료한 경우: 해당 플로우에서 계속 진행

## 상담 운영 시간 {#operating-hour}

{% hint style="danger" %}
\*\*\*\*[**마스터**](../overview.md#undefined-1)만 설정할 수 있습니다.
{% endhint %}

{% hint style="info" %}
팀 설정을 하면 모든 프로필에서 사용할 수 있고 프로필 별로 각각 설정할 수도 있습니다.
{% endhint %}

![&#xC0C1;&#xB2F4; &#xC6B4;&#xC601; &#xC2DC;&#xAC04; &#xC124;&#xC815; &#xD654;&#xBA74; &#xC608;&#xC2DC;](../../.gitbook/assets/undefined%20%286%29.png)

상담 운영 시간을 설정할 수 있습니다. 기본 설정은 오전 9시 ~ 오후 6시\(KST\) 입니다.  
운영시간이 아닐 때 고객이 상담을 요청하는 경우의 메시지나 요청을 어떻게 처리할지 등을 설정할 수 있습니다.

![&#xC0C1;&#xB2F4; &#xC6B4;&#xC601; &#xC2DC;&#xAC04; &#xC124;&#xC815; \(&#xD504;&#xB85C;&#xD544;\) &#xC608;&#xC2DC;](../../.gitbook/assets/undefined%20%282%29.png)

### 운영시간 사용 / 항시 운영 {#operating-hour-enable}

* 프로필\(챗봇\) 이름 오른쪽의 스위치를 켜면 운영시간 설정을 사용하고, 끄면 운영시간 설정을 사용하지 않고 항시 운영으로 설정됩니다.

### 운영 스케쥴 {#schedule}

* 팀 설정을 선택하면 위의 팀 설정이 적용되고 개별 설정을 선택하면 해당 프로필\(챗봇\)만 별도로 운영시간을 설정합니다.

### 미운영 시간 안내 메시지 {#non-operating-hour-message}

* 상담 운영시간 외 시간에 고객이 상담원을 호출한 경우에 노출할 메시지를 설정합니다.
* 팀 설정에서는 메시지만 설정할 수 있고,  프로필\(챗봇\) 개별 설정에서는 상담 미운영시간에 특정 플로우로 이동하도록 설정할 수 있습니다.

### 미운영 시간 상담 요청 접수 {#non-operating-hour-agent-call}

* 상담 운영시간 외 시간에 고객이 상담원을 호출한 경우에 해당 상담을 접수할지 설정합니다.
* 미운영 시간에 들어온 상담을 별도로 확인하려면 접수함으로 설정하세요.

### 미운영 시간 자동 응답 전환 {#non-operating-hour-auto-reply}

* 미운영 시간에 봇이 자동으로 응답하게 할지 설정합니다.
* 미운영 시간에 상담 요청을 접수하고 운영시간에 상담을 모아서 대응해야 한다면 미사용으로 설정하세요.

## 상담 자동 배정 {#automatic-assignment}

{% hint style="danger" %}
\*\*\*\*[**마스터**](../overview.md#undefined-1)만 설정할 수 있습니다.
{% endhint %}

{% hint style="info" %}
팀 설정을 하면 모든 프로필에서 사용할 수 있고 프로필 별로 각각 설정할 수도 있습니다.
{% endhint %}

![&#xC0C1;&#xB2F4; &#xC790;&#xB3D9; &#xBC30;&#xC815; &#xC124;&#xC815; &#xD654;&#xBA74; &#xC608;&#xC2DC;](../../.gitbook/assets/undefined%20%284%29.png)

상담원 연결 요청 시 담당 상담원을 자동으로 배정하는 규칙을 설정합니다.

![&#xC0C1;&#xB2F4; &#xC790;&#xB3D9; &#xBC30;&#xC815; &#xC124;&#xC815; \(&#xD504;&#xB85C;&#xD544;\) &#xD654;&#xBA74; &#xC608;&#xC2DC;](../../.gitbook/assets/undefined%20%2817%29.png)

### 자동 배정 / 수동 배정 {#automatic-assignment-enable}

* 자동 배정 설정을 사용하지 않는 경우, 수동 배정으로 설정됩니다

### 배정 규칙 {#assignment-rule}

* 배정 규칙에서 아무것도 선택하지 않으면 랜덤하게 배정 됩니다.
* 상담원이 담당 고객을 관리해야 한다면 기존 상담원에게 배정되도록 설정하세요.
* 기존 상담원에게 배정되도록 설정했으나 기존 상담원이 부재중인 경우 다른 상담원에게 배정되도록 설정할 수 있습니다.

### 상담 배정 {#assignment-rule-2}

* 상담원이 한 명이 처리해야할 상담의 갯수를 설정할 수 있습니다.
* 여기서 설정한 배정받는 최대 상담 수는 상담을 요청한 상태\(대기\)와 상담이 진행중인 상태를 포함합니다.
* 상담 운영시간을 설정했고 미운영 시간에 들어온 상담을 접수하도록 설정했다면 상담 운영시간이 되었을 때, 운영시간에 요청한 상담을 먼저 처리할 지, 미운영 시간에 들어온 상담을 먼저 처리할 지 설정할 수 있습니다.

### 일반 상담원 설정 {#general-agent}

* 상담 요청이 들어왔을 때 배정받을 일반 상담원을 설정합니다.
* 여기서 설정한 상담원들에게 위에서 설정한 배정 규칙에 따라 자동 배정이 이루어집니다.

### 전문 상담원 설정 {#professional-agent}

> 대분류 chat:category:0 
>
> 중분류 chat:category:1
>
> 소분류 chat:category:2

* 대분류, 중분류, 소분류의 카테고리를 봇 빌더의 파라미터로 설정할 수 있습니다.
* 고객이 챗봇에서 선택한 대분류 / 중분류 / 소분류에 따라 전문 상담원에게 상담이 자동으로 배정되도록 설정할 수 있습니다.
* 예\) 대분류 - 회원 / 비회원, 중분류 - 결제 / 회원탈퇴 / 회원가입 등등
* 전문 상담원의 전문성이 보장되어야 한다면 전문 상담원으로 설정된 상담원 외의  상담원에게 배정되지 않도록 설정할 수 있습니다.

## 알림 {#notification}

{% hint style="info" %}
여러 팀에 속해있다면 각 팀별로 설정을 다르게 할 수 있습니다.
{% endhint %}

![&#xC54C;&#xB9BC; &#xC124;&#xC815; &#xD654;&#xBA74; &#xC608;&#xC2DC;](../../.gitbook/assets/undefined%20%2823%29.png)

고객이 상담원을 호출한 경우, 상담이 나에게 배정된 경우, 고객이 메시지를 보낸 경우에 브라우저 알림\(소리\)를 전송합니다. 브라우저에서 알림 차단/허용 선택창이 뜨는경우 ‘허용'을 선택하셔야 알림을 받을 수 있습니다.  
브라우저에서 알림을 받도록 허용한 경우에 알림을 어떤 상황에서 받을 지 설정할 수 있습니다.



