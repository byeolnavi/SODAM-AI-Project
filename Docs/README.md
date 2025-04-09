# SODAM-AI-Project

소담(小譚) - 작고 편안한 시니어를 위한 말동무 AI 로봇 프로젝트  
사용자의 **음성 감정 인식 및 반응**을 통해 시니어의 **정서적 교감**을 유도하는 **AI 음성비서 시스템**

---

### 📁 프로젝트 폴더 구조 (Project Folder Structure)

```text
Sodam-AI-Project/
├── Hardware/ (하드웨어, ESP32, 회로도 등)
├── RaspberryPi/ (라즈베리파이 코드 전체)
├── AI/ (음성, 감정분석, 비전 관련 코드)
├── App/ (Flutter 앱 코드 전체)
├── Docs/ (모든 문서, README, 발표자료)
└── .gitignore
```

---

### 📂 브랜치 구조 (Branch Structure)

소담 프로젝트는 팀원 역할에 따라 아래와 같은 브랜치 구조를 사용합니다.

| 브랜치 이름 | 설명 |
|-------------|------|
| `main` | 최종 배포용 메인 브랜치 |
| `dev` | 기능 개발 통합 브랜치 |

| 역할             | 이름     | 브랜치 이름                     | 설명                         |
|------------------|----------|----------------------------------|------------------------------|
| 🧑‍💼 팀장           | 고한별   | `feature/team-leader-kohanbyeol`      | 팀장 작업용 브랜치     |
| 🧠 AI & S/W 파트장 | 김병훈   | `feature/ai-leader-kimbyeonghun`| AI 및 소프트웨어 파트 총괄 작업용 |
| 🧠 AI & S/W 팀원  | 노종환   | `feature/ai-nojonghwan`         | AI 및 소프트웨어 팀원 작업용   |
| 🔧 H/W 파트장     | 고연우   | `feature/hw-leader-koyeonwoo`   | 하드웨어 파트 총괄 작업용      |
| 🔧 H/W 팀원       | 김민     | `feature/hw-kimmin`             | 하드웨어 파트 팀원 작업용      |


> ✅ **규칙**: 각 팀원은 본인 전용 브랜치에서 작업하고, 완료 후 `dev` 브랜치로 Pull Request를 보냅니다.
---
### 📝 커밋 메시지 작성 팁

| 태그          | 사용 예시                             | 설명                                    |
|---------------|---------------------------------------|-----------------------------------------|
| `[feat]`      | `[feat] 음성 감정 인식 기능 추가`         | 새로운 기능 추가                         |
| `[fix]`       | `[fix] MQTT 연결 오류 수정`             | 버그 또는 오류 수정                      |
| `[docs]`      | `[docs] 프로젝트 README 업데이트`       | 문서 작성, 수정                          |
| `[init]`      | `[init] 프로젝트 기본 폴더 구조 설정`      | 프로젝트 초기 설정 및 초기화 작업        |
| `[refactor]`  | `[refactor] AI 코드 구조 개선`          | 기능 변화 없이 코드 구조 개선 및 리팩토링 |
| `[style]`     | `[style] 코드 주석 및 포맷 정리`         | 코드 스타일 변경 (형식, 주석, 띄어쓰기 등)|

---

### 💡 브랜치 이름 작성 규칙

- `feature/역할-이름` 형식 사용
  - 예시: `feature/hw-kimmin`, `feature/ai-leader-kimbyeonghun`
- 브랜치 이름은 영어 소문자로 작성
- 이름은 구분이 쉽게 "영문 이름 또는 한글 이름 로마자 표기" 사용

---

### 🛠️ 사용 기술

- **Raspberry Pi 5 + MicroPython + MQTT**
  - 라즈베리파이 및 ESP32 장비와 무선 통신 (MQTT)

- **Whisper + GPT (OpenAI API)**
  - 음성 인식(Whisper) 및 감정 분석, 대화 생성(GPT)

- **Flutter (Caregiver App)**
  - 보호자와 사용자를 위한 모바일 앱 개발 프레임워크

- **Firebase**
  - 데이터베이스, 사용자 인증 및 실시간 데이터 관리

- **GitHub + GitHub Actions**
  - 코드 협업 및 자동화 배포 관리
