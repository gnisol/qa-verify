<div align="center">

<img src="gni_logo.png" alt="GNI Solution" width="140">

# 증명서 진위확인 · Certificate Verification

**지엔아이솔루션(주) 품질보증부**가 발급한 증명서의 **발급 사실**을 확인하는 공개 페이지입니다.<br>
Public verification service for certificates issued by **GNI Solution Co., Ltd. — Quality Assurance Dept.**

[![진위확인 바로가기](https://img.shields.io/badge/진위확인-바로가기-D97757?style=for-the-badge)](https://gnisol.github.io/qa-verify/)
[![GitHub Pages](https://img.shields.io/badge/hosted%20on-GitHub%20Pages-1E2630?style=for-the-badge&logo=github)](https://gnisol.github.io/qa-verify/)

</div>

---

## 확인 방법 · How to verify

증명서를 받으신 발주처·기관에서는 아래 두 가지 방법 중 하나로 확인하실 수 있습니다.

| 방법 | 절차 |
|------|------|
| **① QR 스캔** | 증명서에 인쇄된 QR 코드를 휴대폰 카메라로 스캔 → 결과 즉시 표시 |
| **② 직접 입력** | 아래 조회 페이지 접속 → 증명서에 기재된 **발급번호(Certificate No.)** 와 **조회코드(Code, 8자리)** 입력 |

> Scan the QR code printed on the certificate, or enter the **Certificate No.** and the 8-digit **Code** on the verification page below.

### 조회 주소 · Verification URLs

| 대상 | 주소 |
|------|------|
| 진위확인 포털 · Portal | <https://gnisol.github.io/qa-verify/> |
| 경력증명서 · Certificate of Career | <https://gnisol.github.io/qa-verify/career_verify.html> |

한국어 / English 표시를 지원합니다. · Available in Korean and English.

### 조회 결과 · Result

조회 결과에는 **발급 여부 · 발급일 · 증명서 유형 · 마스킹 성명 · 총 경력일수 · 경력 기재건수**가 표시됩니다.

| 결과 | 의미 |
|------|------|
| **VERIFIED** | 당사가 발급한 증명서가 맞습니다. |
| **CODE MISMATCH** | 발급번호는 존재하나 조회코드가 일치하지 않습니다. 입력값을 확인해 주십시오. |
| **NOT FOUND** | 해당 발급번호의 기록이 없습니다. |

`CODE MISMATCH` 또는 `NOT FOUND`가 반복되거나 조회 결과가 증명서 내용과 다를 경우,
해당 증명서는 당사가 발급한 것이 아닐 수 있으므로 **품질보증부로 문의**하여 주시기 바랍니다.

---

## 개인정보 보호 · Privacy

본 서비스는 진위확인에 **필요한 최소한의 정보만** 공개하도록 설계되었습니다.

**공개 항목**

- 발급번호 · 발급일 · 증명서 유형
- **마스킹된 성명** (예: `Kim, K***`)
- 총 경력일수 · 경력 기재건수

**비공개 항목**

- 주민등록번호 · 생년월일
- 성명 전체
- 프로젝트 상세내역 · 발주처 · 근무지
- 주소 · 연락처 · 제출처

**무단 조회 방지**

- 발급번호만으로는 조회할 수 없으며, 증명서에만 기재된 **8자리 조회코드**가 일치해야 합니다.
- 공개 데이터에는 조회코드 원본 대신 **단방향 해시(SHA-256, 반복 적용)** 값만 저장되어 있어, 공개 파일로부터 코드를 역산할 수 없습니다.
- 성명은 조회코드로 **암호화**되어 저장되며, 코드를 모르면 복호화되지 않습니다. 복호화에 성공하더라도 화면에는 마스킹된 형태로만 표시됩니다.
- 전체 발급내역은 사내에서만 관리하며 외부에 공개하지 않습니다.

---

## 저장소 구성 · Repository contents

| 파일 | 설명 |
|------|------|
| `index.html` | 진위확인 포털 (증명서 유형 선택) |
| `career_verify.html` | 경력증명서 조회 페이지 (KO / EN) |
| `gni_career_db.json` | 발급기록 (공개용 · 최소 항목만 포함) |
| `gni_logo.png` | 회사 로고 |

정적 파일만으로 구성되어 있으며 서버·데이터베이스를 사용하지 않습니다.<br>
Fully static site — no server-side code, no database.

---

<div align="center">

**지엔아이솔루션(주)** · 품질보증부<br>
GNI Solution Co., Ltd. — Quality Assurance Dept.<br>
Tel. 070-7575-2463

</div>
