
````markdown
<!--타이틀 부분-->
<img src="https://capsule-render.vercel.app/api?type=blur&color=gradient&height=300&section=header&text=Jobis&fontSize=80" />

# 👀 Jobis
AI 기반 맞춤형 **면접 준비 플랫폼**  
이력서와 공고 URL을 기반으로 면접 질문을 생성하고, 실시간 피드백과 관련 학습 영상을 제공하여 사용자가 효과적으로 면접을 준비할 수 있도록 돕습니다.

---

## 🍎 소개
![1](https://github.com/user-attachments/assets/67379bb3-8184-472c-9a80-1787732c4445)

Jobis는 단순한 채용/이력서 관리 서비스가 아닌 **개인화된 AI 면접 준비 서비스**를 목표로 합니다.  
사용자의 이력서와 지원 직무 정보를 바탕으로 맞춤형 질문과 피드백을 제공하며, 부족한 부분은 영상 자료를 통해 보완할 수 있습니다.

**주요 기능**
- 📝 **맞춤형 면접 질문 생성** (LLM + RAG 기반)
- 💬 **실시간 피드백 및 개선 포인트 제시**
- 🎥 **이력서 맞춤 영상 추천**
- 📊 **피드백 히스토리 관리**

---

## 🍎 팀원
![9](https://github.com/user-attachments/assets/ada8b4f0-507d-410d-9b0f-41d3db558373)

---

## 🍎 배경
![4](https://github.com/user-attachments/assets/f3b25bd3-3504-46da-9ffd-f5a27ad24dae)

### 기존 서비스의 문제
1. 면접 보조가 아닌 **채용 중심** 서비스
2. **정형화된 질문**만 제공 → 다양성/적합성 부족
3. **개인화 수준 낮음**
4. **실시간 피드백 기능 부재**

➡️ Jobis는 이를 개선하여 **개인화 + 피드백 중심**의 차별화된 면접 준비 솔루션을 제공합니다.

---

## 🍎 기술 스택
<h4>Frontend</h4>
<div>
  <img src="https://img.shields.io/badge/react-20232a.svg?style=for-the-badge&logo=react&logoColor=61DAFB" />&nbsp
  <img src="https://img.shields.io/badge/javascript-F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=20232a" />&nbsp
  <img src="https://img.shields.io/badge/html5-E34F26.svg?style=for-the-badge&logo=html5&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/styled--components-DB7093?style=for-the-badge&logo=styled-components&logoColor=ffd35b" />&nbsp
  <img src="https://img.shields.io/badge/tailwindcss-1daabb.svg?style=for-the-badge&logo=tailwind-css&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/css3-1572B6.svg?style=for-the-badge&logo=css3&logoColor=white" />&nbsp
</div>

<h4>Backend</h4>
<div>
  <img src="https://img.shields.io/badge/Fastapi-009688.svg?style=for-the-badge&logo=Fastapi&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=Docker&logoColor=white"/>&nbsp
</div>

<h4>AI</h4>
<div>
  <img src="https://img.shields.io/badge/openai-412991?style=for-the-badge&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/faiss-E34F26?style=for-the-badge&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/yt_dlp-009688?style=for-the-badge&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/selenium-1572B6?style=for-the-badge&logo=openai&logoColor=white"/>
</div>

---

## 🍎 아키텍처
```mermaid
flowchart TD
    A[사용자 이력서 + 공고 URL] -->|입력| B[LLM + RAG 처리]
    B --> C[맞춤형 면접 질문 생성]
    C --> D[실시간 피드백 제공]
    D --> E[관련 영상 추천 시스템]
    E --> F[UI/UX 프론트엔드]
````

---

## 🍎 UI/UX

![38](https://github.com/user-attachments/assets/bdd8b5f2-f375-417b-83f5-4cf1e4e7a61f)
![39](https://github.com/user-attachments/assets/40c2564b-0a0b-4647-9934-371f94dc76c2)
![40](https://github.com/user-attachments/assets/786c8f87-9fb7-4000-9bc5-20800cdea3de)
![42](https://github.com/user-attachments/assets/15cc7623-9451-4042-ab81-a6f25777c8ad)

---

## 🍎 주요 기능 설명

### 추천 시스템

* 지원 직무와 이력서 기반으로 영상 자료를 자동 추천
* Faiss 기반 벡터 검색으로 개인화 강화
* YouTube 크롤링(`yt_dlp` + `selenium`)을 통해 최신 자료 확보

### 챗봇

* 면접관 역할 수행 (질문 생성)
* 답변에 대한 **실시간 피드백** 제공
* 답변 기록 저장 및 개선 히스토리 관리 가능

---

## 🍎 설치 및 실행 방법

```bash
# Clone repository
git clone https://github.com/your-repo/jobis.git
cd jobis

# Backend 실행
cd backend
docker-compose up --build

# Frontend 실행
cd frontend
npm install
npm run dev
```

---

## 🍎 향후 발전 방향

* 음성 인식 기반 실시간 피드백 (Speech-to-Text + Sentiment Analysis)
* 기업별/직무별 맞춤 데이터셋 확대
* 사용자 데이터 기반 **개인화 강화**
* 면접 모드(실제 화상 면접 시뮬레이션) 제공

```

