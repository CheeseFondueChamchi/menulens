# Menu Lens 개인정보처리방침

> **초안 — 법률 전문가 검토 전**
> **DRAFT — pending legal review**
>
> 이 문서는 정식 법률 자문 없이 작성된 초안입니다. 서비스 출시 전 반드시 개인정보보호법 전문 변호사의 검토를 받아야 합니다.
> This document is a draft prepared without formal legal advice. It must be reviewed by a lawyer specializing in the Personal Information Protection Act (PIPA) before launch.

---

## 한국어 원문 (Korean — Governing Text)

[사업자명 — PLACEHOLDER]("회사")는 「개인정보보호법」 제30조 등 관계 법령에 따라 이용자의 개인정보를 보호하고 관련 고충을 신속하고 원활하게 처리할 수 있도록 다음과 같이 개인정보처리방침을 수립·공개합니다.

### 제1조 (수집하는 개인정보 항목 및 수집 방법)

회사는 다음과 같은 개인정보를 수집합니다.

| 구분 | 수집 항목 | 수집 방법 | 수집 시점 |
|---|---|---|---|
| 필수 (익명 이용) | 기기 식별자(익명 디바이스 토큰), 접속 로그(타임스탬프) | 앱 설치·이용 시 자동 생성 | 앱 최초 실행 시 |
| 선택 (로그인 이용 시) | 로그인 제공자(Apple/Google/Kakao)가 발급하는 고유 식별자(subject identifier), 이메일 주소(제공자가 제공하는 경우) | 이용자가 로그인 기능을 선택하여 이용할 때 | 로그인 시 |
| 서비스 이용 과정 | 메뉴판 이미지에서 추출된 텍스트(운영 로그), 요청 타임스탬프, 기기 식별자 | 서비스 이용(메뉴 분석) 시 자동 생성 | 분석 요청 시 |
| 결제 관련 | 구매 영수증/거래 식별자(Apple/Google이 제공하는 범위 내) | 인앱결제 진행 시 | 결제 시 |

**중요 — 이미지 미저장**: 이용자가 촬영·업로드한 **메뉴판 원본 이미지는 서버에 저장되지 않습니다.** 이미지는 분석(텍스트 인식 및 번역) 처리 후 즉시 폐기되며, 서버에는 이미지로부터 추출된 **텍스트만** 운영 로그 형태로 남습니다.

### 제2조 (개인정보의 수집·이용 목적)

1. 익명 디바이스 토큰: 무료 체험(매일 5회) 소진 여부 판단, 7일 패스 유효기간 관리, 부정 이용(우회) 방지
2. 로그인 시 수집 정보(제공자 식별자, 이메일): 구매 복원, 기기 간 서비스 연동, 계정 기반 고객 지원
3. 운영 로그(추출 텍스트, 타임스탬프, 기기 식별자): 서비스 품질 개선, 오류 진단, 이상 이용 탐지, 법령상 분쟁 대응
4. 결제 정보: 결제 확인, 환불 처리, 관계 법령(전자상거래법 등)에 따른 거래 기록 보관

### 제3조 (개인정보의 보유 및 이용 기간)

1. **운영 로그(추출 텍스트, 타임스탬프, 기기 식별자)**: 수집일로부터 **90일간** 보관 후 자동 파기됩니다. (내부 설정값 `OPS_RETENTION_DAYS`, 기본 90일)
2. **계정 정보(로그인 시 수집한 제공자 식별자, 이메일)**: 이용자가 계정을 유지하는 동안 보관하며, **계정 삭제(탈퇴) 요청 시 지체 없이 파기**합니다.
3. **익명 디바이스 토큰**: 앱 삭제 또는 별도 삭제 요청 전까지 보관되며, 무료 체험/패스 유효기간 관리 목적이 소멸하면 파기합니다.
4. **결제 관련 기록**: 「전자상거래 등에서의 소비자보호에 관한 법률」 등 관계 법령이 정하는 경우 해당 법정 보관기간(예: 대금결제 및 재화 등의 공급에 관한 기록 5년, 소비자 불만 또는 분쟁처리에 관한 기록 3년 — 시행령 기준, 최신 법령 재확인 필요) 동안 별도 보관 후 파기합니다.
5. 관계 법령에 특별한 규정이 있는 경우 회사는 해당 법령에서 정한 기간 동안 개인정보를 보관합니다.

### 제4조 (개인정보의 국외 이전)

회사는 메뉴판 이미지에서 텍스트를 인식하고 번역하는 과정에서 **비전 언어모델(Vision LLM) 처리를 위해 OpenAI, Inc.(미국)의 API를 이용**하며, 이 과정에서 이미지 및/또는 추출된 텍스트가 국외로 이전될 수 있습니다. 「개인정보보호법」 제28조의8에 따라 다음과 같이 고지합니다.

| 항목 | 내용 |
|---|---|
| 이전받는 자 | OpenAI, Inc. (또는 그 계열사/서비스 제공 법인) |
| 이전되는 국가 | 미합중국(United States) |
| 이전 일시 및 방법 | 메뉴 분석 요청 시마다 API 호출을 통해 실시간 전송 |
| 이전 항목 | 메뉴판 이미지(처리 목적, 처리 후 즉시 폐기) 및/또는 추출된 텍스트 |
| 이전받는 자의 이용 목적 | 이미지 내 텍스트 인식 및 번역 처리 |
| 이전받는 자의 보유·이용 기간 | OpenAI의 API 데이터 처리 정책에 따름 [PLACEHOLDER — 변호사/운영자 검토: OpenAI API 데이터 보유·재사용 정책 최신 조건 확인 및 계약(DPA 등) 체결 여부 명시 필요] |

이용자는 국외 이전에 관한 동의를 거부할 권리가 있으나, 거부 시 비전 언어모델 기반 메뉴 분석 기능(서비스의 핵심 기능)을 이용할 수 없습니다.

### 제5조 (개인정보의 제3자 제공)

회사는 이용자의 개인정보를 원칙적으로 제3자에게 제공하지 않습니다. 다만 다음의 경우는 예외로 합니다.

1. 이용자가 사전에 동의한 경우
2. 법령의 규정에 의거하거나, 수사 목적으로 법령에 정해진 절차와 방법에 따라 수사기관의 요구가 있는 경우
3. 제4조에 따른 국외 이전(비전 언어모델 처리 위탁)은 서비스 제공을 위한 처리위탁이며, 별도의 영리 목적 판매·제공이 아닙니다.

**회사는 이용자의 개인정보를 판매하지 않습니다.**

### 제6조 (개인정보 처리 위탁)

| 수탁업체 | 위탁업무 내용 |
|---|---|
| OpenAI, Inc. | 메뉴판 이미지/텍스트 인식 및 번역을 위한 비전 언어모델 처리 |
| Apple Inc. / Google LLC | 인앱결제 처리, 로그인(Sign in with Apple / Google Sign-In) |
| 카카오 (주식회사 카카오) | 로그인(Kakao Login) |
| [PLACEHOLDER — 서버/클라우드 호스팅 업체명] | 서버 인프라 운영 (한국 내 서버 운영) |

### 제7조 (개인정보의 안전성 확보 조치)

회사는 다음과 같은 기술적·관리적 조치를 취하고 있습니다.

1. **토큰 해시 저장**: 기기 식별자 등 인증 관련 토큰은 원문이 아닌 해시(hash) 값으로 저장하여, 데이터베이스가 유출되더라도 원본 토큰이 노출되지 않도록 합니다.
2. **관리 페이지 접근 제한**: 내부 운영(관리자) 페이지는 외부 인터넷에 노출되지 않고, 서버 자체(loopback, 127.0.0.1)에서만 접근 가능하도록 제한되어 있습니다.
3. **이미지 비저장**: 앞서 밝힌 바와 같이 메뉴판 원본 이미지는 서버에 저장되지 않고 처리 후 즉시 폐기됩니다.
4. **접근 권한 관리**: 개인정보 처리 시스템에 대한 접근 권한을 최소한의 인원(운영자 본인)으로 제한합니다.
5. 그 밖에 관계 법령이 요구하는 수준의 기술적·관리적 보호조치를 적용합니다. [PLACEHOLDER — 변호사 검토: 개인정보보호법 시행령상 안전성 확보조치 세부 고시 기준(암호화, 접근통제, 접속기록 보관 등) 충족 여부 상세 점검 필요]

### 제8조 (개인정보 보호책임자)

회사는 개인정보 처리에 관한 업무를 총괄해서 책임지고, 개인정보 처리와 관련한 정보주체의 불만처리 및 피해구제 등을 위하여 아래와 같이 개인정보 보호책임자를 지정하고 있습니다.

- **개인정보 보호책임자**: [PLACEHOLDER — 성명] (운영자 본인 겸임)
- **연락처(이메일)**: [PLACEHOLDER — 이메일 주소]
- **연락처(전화)**: [PLACEHOLDER — 전화번호]

정보주체는 회사의 서비스를 이용하며 발생한 모든 개인정보 보호 관련 문의, 불만처리, 피해구제 등에 관한 사항을 개인정보 보호책임자에게 문의할 수 있습니다.

### 제9조 (정보주체의 권리·의무 및 행사방법)

1. 이용자는 회사에 대해 언제든지 다음 각 호의 개인정보 보호 관련 권리를 행사할 수 있습니다.
   - 개인정보 열람 요구
   - 오류 등이 있을 경우 정정 요구
   - 삭제 요구
   - 처리정지 요구
2. 제1항에 따른 권리 행사는 회사에 대해 이메일([PLACEHOLDER — 이메일])을 통하여 하실 수 있으며, 회사는 이에 대해 지체 없이 조치하겠습니다.
3. **계정(로그인 정보) 삭제**: 앱 내 설정 메뉴의 "계정 삭제" 기능 또는 위 이메일을 통해 요청할 수 있습니다. 요청 접수 후 [PLACEHOLDER — 처리 기한, 예: 7일] 이내에 처리됩니다.
4. 정보주체는 개인정보 침해로 인한 신고나 상담이 필요한 경우 개인정보침해신고센터(privacy.go.kr / 국번없이 182), 대검찰청, 경찰청 등에 문의할 수 있습니다.

### 제10조 (개인정보의 파기)

1. 회사는 개인정보 보유기간의 경과, 처리목적 달성 등 개인정보가 불필요하게 되었을 때에는 지체 없이 해당 개인정보를 파기합니다.
2. 전자적 파일 형태의 정보는 기술적 방법을 사용하여 복구·재생이 불가능하도록 영구 삭제합니다.

### 제11조 (개인정보 유출 등에 대한 통지·신고)

회사는 개인정보 유출 등 사고가 발생한 경우, 관계 법령(개인정보보호법 제34조 등)에 따라 지체 없이(정당한 사유가 없는 한 72시간 이내) 정보주체에게 관련 사실을 통지하고, 일정 규모 이상의 피해(1천 명 이상의 정보주체에 관한 개인정보 유출 등 법령이 정한 기준에 해당하는 경우)에 대해서는 개인정보보호위원회 또는 한국인터넷진흥원(KISA)에 신고합니다.

### 제12조 (쿠키 등 자동 수집 장치)

[PLACEHOLDER — 변호사 검토: 앱에서 쿠키/유사 기술(모바일 광고 식별자 등)을 실제로 사용하는지 기술팀 확인 후 해당 여부에 따라 이 조항 작성/삭제. 현재 파악된 범위에서는 기기 식별자 외 별도 광고 추적 SDK 사용 계획 없음.]

### 제13조 (개인정보처리방침의 변경)

이 개인정보처리방침은 [PLACEHOLDER — 시행일자]부터 적용되며, 법령 및 방침에 따른 변경내용의 추가, 삭제 및 정정이 있는 경우에는 변경사항의 시행 최소 7일 전부터 서비스 내 공지사항을 통하여 고지할 것입니다.

---

## English Translation (Reference Only — Korean Text Governs)

*This is a courtesy translation. In case of any discrepancy, the Korean original text prevails.*

[Business name — PLACEHOLDER] ("Company") establishes and discloses this Privacy Policy in accordance with Article 30 of Korea's Personal Information Protection Act ("PIPA") and related regulations, to protect users' personal information and handle related grievances promptly.

### Article 1 (Items Collected and Method of Collection)

| Category | Items Collected | Method | When |
|---|---|---|---|
| Required (anonymous use) | Device identifier (anonymous device token), access logs (timestamps) | Auto-generated on install/use | First app launch |
| Optional (if logging in) | Unique subject identifier issued by the login provider (Apple/Google/Kakao); email address (if provided by the provider) | When the user chooses to log in | At login |
| During Service use | Text extracted from menu images (operational logs), request timestamps, device identifier | Auto-generated when using the Service (menu analysis) | At each analysis request |
| Payment-related | Purchase receipt / transaction identifier (within what Apple/Google provide) | During in-app purchase | At payment |

**Important — no image storage.** The **original menu image a user captures or uploads is never stored on our servers.** The image is discarded immediately after processing (text recognition and translation); only the **extracted text** is retained server-side, as part of operational logs.

### Article 2 (Purposes of Collection and Use)

1. Anonymous device token: tracking free-trial (5-use) consumption, managing 7-day pass validity, preventing abuse/circumvention.
2. Login-collected data (provider identifier, email): purchase restore, cross-device service linkage, account-based customer support.
3. Operational logs (extracted text, timestamps, device identifier): service quality improvement, error diagnosis, abuse detection, responding to legal disputes.
4. Payment information: payment verification, refund processing, transaction record-keeping required by law (e.g., the Act on Consumer Protection in Electronic Commerce).

### Article 3 (Retention Period)

1. **Operational logs** (extracted text, timestamps, device identifier): retained for **90 days** from collection, then automatically destroyed. (Internal configuration `OPS_RETENTION_DAYS`, default 90 days.)
2. **Account data** (provider identifier, email collected at login): retained while the account exists; **destroyed without delay upon account deletion.**
3. **Anonymous device token**: retained until app deletion or a separate deletion request; destroyed once its free-trial/pass-tracking purpose no longer applies.
4. **Payment records**: retained separately for the statutory period required by law (e.g., records of payment and supply of goods/services: 5 years; records of consumer complaint/dispute handling: 3 years — per Enforcement Decree of the e-commerce consumer protection law; reconfirm current figures), then destroyed.
5. Where other laws specifically require a different retention period, the Company retains data for that statutory period.

### Article 4 (Overseas Transfer of Personal Information)

To recognize and translate text from menu images, the Company uses the **API of OpenAI, Inc. (United States) for vision-language-model processing**, which may involve transferring images and/or extracted text abroad. Per PIPA Article 28-8, the Company discloses:

| Item | Detail |
|---|---|
| Recipient | OpenAI, Inc. (or its affiliated service-providing entity) |
| Destination country | United States |
| Timing and method | Real-time, via API call, for each menu-analysis request |
| Items transferred | Menu image (for processing only; discarded immediately after) and/or extracted text |
| Recipient's purpose of use | Text recognition and translation within images |
| Recipient's retention period | Per OpenAI's API data-handling policy. [PLACEHOLDER — lawyer/operator review: confirm OpenAI's current API data retention/reuse terms and whether a data processing agreement (DPA) has been executed.] |

Users may decline consent to this overseas transfer, but doing so means the vision-language-model-based menu analysis feature (the Service's core function) cannot be used.

### Article 5 (Provision to Third Parties)

The Company does not provide users' personal information to third parties, except:

1. Where the user has given prior consent;
2. Where required by law or requested by an investigative agency following legally prescribed procedures; or
3. The overseas transfer under Article 4 (vision-language-model processing) is a processing entrustment for Service delivery, not a for-profit sale or provision.

**The Company does not sell users' personal information.**

### Article 6 (Entrustment of Personal Information Processing)

| Processor | Entrusted Task |
|---|---|
| OpenAI, Inc. | Vision-language-model processing for menu image/text recognition and translation |
| Apple Inc. / Google LLC | In-app payment processing; login (Sign in with Apple / Google Sign-In) |
| Kakao Corp. | Login (Kakao Login) |
| [PLACEHOLDER — server/cloud hosting provider name] | Server infrastructure operation (servers operated in Korea) |

### Article 7 (Security Measures)

1. **Token hashing**: authentication-related tokens such as device identifiers are stored as hashes, not plaintext, so a database breach does not expose the original token.
2. **Restricted admin access**: the internal operations (admin) page is not exposed to the public internet and is reachable only from the server itself (loopback, 127.0.0.1).
3. **No image storage**: as noted above, original menu images are never stored server-side and are discarded immediately after processing.
4. **Access control**: access to personal-information-processing systems is limited to the minimum necessary personnel (the operator).
5. Other technical/administrative safeguards required by law are applied. [PLACEHOLDER — lawyer review: verify compliance with detailed security-measure standards under PIPA's Enforcement Decree and related notices (encryption, access control, access-log retention, etc.).]

### Article 8 (Privacy Officer)

- **Privacy Officer**: [PLACEHOLDER — name] (concurrently the Operator)
- **Email**: [PLACEHOLDER — email address]
- **Phone**: [PLACEHOLDER — phone number]

Users may direct all privacy-related inquiries, complaints, and requests for remedy to the Privacy Officer above.

### Article 9 (Data Subject Rights and How to Exercise Them)

1. Users may exercise the following rights regarding their personal information at any time:
   - Request access to their data
   - Request correction of errors
   - Request deletion
   - Request suspension of processing
2. These rights may be exercised by emailing [PLACEHOLDER — email]; the Company will act without undue delay.
3. **Account (login data) deletion**: available via the "Delete Account" feature in the app's settings menu, or by emailing the address above. Requests are processed within [PLACEHOLDER — processing timeframe, e.g., 7 days].
4. Users may also contact the Personal Information Infringement Report Center (privacy.go.kr / 182), the Supreme Prosecutors' Office, or the National Police Agency for complaints or reports related to personal information infringement.

### Article 10 (Destruction of Personal Information)

1. The Company destroys personal information without delay once its retention period expires or its processing purpose is achieved and it is no longer needed.
2. Electronic files are permanently deleted using methods that prevent recovery or reconstruction.

### Article 11 (Breach Notification)

If a personal information breach occurs, the Company will, per PIPA Article 34 and related law, notify affected users without delay (within 72 hours absent a valid reason) and, where the breach meets the statutory threshold (e.g., affecting 1,000 or more data subjects), report it to the Personal Information Protection Commission (PIPC) or the Korea Internet & Security Agency (KISA).

### Article 12 (Cookies and Similar Automated Collection)

[PLACEHOLDER — lawyer review: confirm with engineering whether cookies or similar tracking technologies (e.g., mobile ad identifiers) are actually used, and draft or remove this article accordingly. As currently understood, no separate ad-tracking SDK is planned beyond the device identifier.]

### Article 13 (Changes to This Policy)

This Privacy Policy takes effect on [PLACEHOLDER — effective date]. Any additions, deletions, or corrections required by law or policy changes will be announced via in-app notice at least 7 days before they take effect.

---

## 변경 이력 / Changelog

- v0.1 draft — 2026-08-19 — Initial draft for legal review.
