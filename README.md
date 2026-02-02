# 🤖 Daily AI Briefing Bot
> **Oracle Cloud와 n8n을 활용한 AI 뉴스 자동 수집 및 요약 시스템**

오라클 클라우드(OCI) 프리 티어 환경에서 n8n을 구축하고, Gemini AI를 연동하여 최신 IT/AI 트렌드를 수집해 텔레그램으로 전송하는 자동화 프로젝트입니다.

---

## 🛠 Tech Stack
| Category | Technology |
| :--- | :--- |
| **Infrastructure** | Oracle Cloud Infrastructure (Always Free) |
| **Automation** | n8n (Self-hosted via Docker) |
| **AI Model** | Google Gemini 1.5 Flash |
| **Notification** | Telegram Bot API |
| **OS** | Ubuntu 22.04 LTS (ARM) |

---

## 📋 주요 기능
- [x] **뉴스 수집**: Google News RSS 및 주요 IT 뉴스 피드 모니터링
- [ ] **AI 요약**: Gemini API를 활용한 한국어 3줄 요약 및 인사이트 추출
- [ ] **자동 알림**: 매일 정해진 시간에 텔레그램 메시지 발송
- [ ] **중복 방지**: 동일한 기사가 중복으로 오지 않도록 필터링 로직 적용

---

## 🚀 프로젝트 아키텍처
1. **Trigger**: n8n Cron 노드가 매일 정해진 시간에 작동
2. **Fetch**: HTTP Request 노드로 뉴스 소스 API/RSS 호출
3. **Analyze**: 수집된 데이터를 Gemini API로 전달하여 분석 및 요약
4. **Notify**: 최종 결과물을 텔레그램 봇을 통해 사용자에게 전송

---

## 📖 학습 및 기록 (Dev Log)
프로젝트를 진행하며 학습한 내용을 기록합니다.

### 1. 인프라 구축
- [ ] 오라클 클라우드 인스턴스 생성 및 보안 리스트(포트 5678) 설정
- [ ] Docker 및 Docker-compose 설치
- [ ] n8n 컨테이너 실행 및 환경 설정

### 2. 워크플로우 설계
- [ ] RSS 피드 데이터 파싱 방법 학습
- [ ] n8n에서 Gemini API 노드 연동 및 프롬프트 엔지니어링
- [ ] 텔레그램 봇 생성 및 API 연동

---

## 💡 Troubleshooting
- **Issue**: 오라클 클라우드 ARM 인스턴스 자원 부족 현상
- **Solution**: (해결 방법 기록 예정)

---

## 🔗 Reference
- [n8n 공식 문서](https://docs.n8n.io/)
- [Oracle Cloud Always Free 정보](https://www.oracle.com/cloud/free/)
