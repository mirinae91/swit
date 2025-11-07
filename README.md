# Study App

> 10대 학생 둘이서 서로의 **공부 기록을 공유하며** 함께 **동기부여를 받을 수 있는 스터디 앱**

---

## 아키텍처 개요

### 🧩 Clean Architecture 기반 구조
- **Presentation / Domain / Data** 계층 분리
- **Freezed**를 활용한 불변(Immutable) 데이터 모델링  

### ☁️ Supabase 서버리스 아키텍처
- **Supabase RPC (Remote Procedure Call)** 로 서버–클라이언트 간 데이터 처리 최적화  
- **SQL Function** 기반 로직 처리 (예: 공부 기록 저장, 그룹 활동 집계)
- **Edge Functions (Deno 기반)** 을 이용한 **Firebase Cloud Messaging(FCM)** 알림 구현

---

## 주요 기능

| 기능 | 설명 |
|------|------|
| 📈 **공부 기록 히트맵** | 날짜별 집중 시간 시각화 |
| 🔔 **FCM 푸시 알림** | 스터디 초대, 리마인더, 팔로우 알림 |
| 👥 **스터디 그룹 생성** | 그룹 만들기 및 참여 기능 |
| 📅 **공유 캘린더 연동** | 스터디 일정 관리 및 공유 |

---

## 기술 스택
- **Flutter (Dart)**  
- **State Management:** GetX   
- **Supabase:** Auth, Database(PostgreSQL), RPC, Edge Functions  
- **Firebase Cloud Messaging:** 푸시 알림  
- **Clean Architecture:** 유지보수성과 확장성 향상

