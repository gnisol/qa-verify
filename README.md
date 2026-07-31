# GNI Solution — 증명서 진위확인
### Certificate Verification — GNI Solution Co., Ltd. (QA Department)

지엔아이솔루션(주) 품질보증부가 발급한 증명서의 **발급 사실**을 확인하는 공개 페이지입니다.

This site confirms **the fact of issuance** of certificates issued by the QA Department of
GNI Solution Co., Ltd. (Global Nondestructive Examination & Inspection Solution Co., Ltd.)

---

## 확인 방법 · How to verify

**1. QR 스캔** — 증명서 좌측 하단의 QR 코드를 스마트폰으로 촬영하면 결과가 바로 표시됩니다.

**2. 직접 입력** — QR을 쓸 수 없으면 아래 주소에서 증명서에 인쇄된 두 값을 입력하십시오.

| 입력값 | 증명서상 위치 |
|--------|--------------|
| 발급번호 (Certificate No.) | 좌측 상단 `Issued No.` 또는 QR 아래 `No.` |
| 조회코드 (Code) | QR 아래 `Code` — 8자리, 대소문자 무관 |

- 포털 · Portal : https://gnisol.github.io/qa-verify/
- 경력증명서 · Career Certificate : https://gnisol.github.io/qa-verify/career_verify.html

화면 우측 상단에서 **KR / EN** 을 전환할 수 있습니다.

---

## 판정 결과 · Results

| 표시 | 의미 |
|------|------|
| **VERIFIED** | 발급 기록과 일치합니다 · Matches our issuance record |
| **CODE MISMATCH** | 조회코드가 일치하지 않습니다 · The code does not match |
| **NOT FOUND** | 해당 발급번호의 기록이 없습니다 · No record for that number |

---

## 공개되는 정보 · What is disclosed

이 저장소의 `gni_career_db.json` 은 누구나 내려받을 수 있습니다. 그래서 아래만 담습니다.

**포함** — 발급번호 · 발급일 · 증명서 유형 · **마스킹 성명**(예: `Hong, G** D***`) · 총 경력일수 · 경력 기재건수 · 발급 기록시각

**미포함** — 주민등록번호 · 성명 전체 · 경력 상세(프로젝트·검사방법·부서) · 제출처 · 주소 · 연락처

### 조회코드는 저장되지 않습니다

공개 파일에는 조회코드 원본이 아니라 `SHA-256(발급번호:조회코드)` 의 앞 32자만 들어갑니다.
파일을 통째로 받아도 조회코드를 알아낼 수 없습니다 (8자리 · 약 1.1조 가지).

발급번호는 연번이므로 번호만으로는 타인의 기록을 열람할 수 없도록 조회코드 일치를 함께 요구합니다.

The public file stores only the first 32 characters of `SHA-256(certificate-no:code)` — never the code itself.

---

## 문의 · Contact

증명서 원본 대조나 발급 관련 문의는 **지엔아이솔루션(주) 품질보증부** 로 연락하십시오.
For verification against the original document, please contact the QA Department.

---

GNI Solution Co., Ltd. · 품질보증부 · Form GA-3