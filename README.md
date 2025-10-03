# Project GGG   
⚠️ Disclaimer  
이 저장소는 제가 **Project GGG 개발에 참여했던 경험**을 기반으로 작성한 **포트폴리오 용도 문서**입니다.  

본 프로젝트는 2023년 12월 액션스퀘어가 개최한 **ActionSquare Steam Festival**을 통해 글로벌 유저 대상 플레이 테스트가 공식 진행된 바 있습니다.  
단, 이 저장소에는 원본 소스 코드나 회사의 미공개 자산은 일절 포함되어 있지 않으며, 이미지는 유튜브에 공개된 영상 중 일부를 캡처한 자료입니다.  
순수하게 개인 경험 정리와 포트폴리오 목적의 문서만 담고 있습니다.

## Quick Summary
- Unreal Engine 5 기반 PC Extraction Shooter 개발 참여
- 역할: 클라이언트 프로그래머 (인게임/아웃게임 콘텐츠, UI, 네트워크, DB, 빌드)
- 성과: 2023년 12월 **ActionSquare Steam Festival** 글로벌 테스트에서 7일간 약 4,000명의 유저 참여, 안정성 확보(크래시 0건)
  
**PC PVPVE 탑다운 루터 슈팅 익스트랙션 게임**

<img src="https://github.com/user-attachments/assets/38020595-f3c4-49cd-8ba7-6da9f2ef0a02" width="400" height="225"/> &nbsp;
<img src="https://github.com/user-attachments/assets/f3787a20-c5ab-43bd-9d01-f0415e583891" width="400" height="225"/>

---

### 1. 프로젝트 개요 (Project Overview)

*   **회사명**: Action Square Co., Ltd. (액션스퀘어(주))
*   **프로젝트명**: Project GGG
*   **개발 기간**: 2022년 10월 ~ 2024년 2월 (약 1년 4개월)
*   **플랫폼**: PC (Dedicated Server 기반 멀티플레이어)
*   **장르**: PVPVE 탑다운 루터 슈팅 익스트랙션 (Quarter-view Looter Shooter Extraction)
*   **주요 성과**:
    *   2023년 12월, 스팀(Steam) 플랫폼에서 **글로벌 플레이 테스트**를 성공적으로 진행
    *   총 **7일간 약 4,000명의 유저**가 테스트에 참여하여 게임의 핵심 재미와 안정성 검증

### 2. 개발 배경 및 본인 역할 (Development Background & My Role)

본 프로젝트는 스팀 글로벌 서비스를 목표로 한 멀티플레이어 탑다운 루터 슈팅 게임 개발 프로젝트였습니다.  
저는 클라이언트 프로그래머로서 게임의 핵심 인/아웃게임 플레이의 컨텐츠 구현 및 UI/UX 시스템 개발에 참여하였으며,
Dedicated Server 및 DB 관리, 빌드/크래시 분석 대응 등 다양한 영역에 걸쳐 프로젝트의 성공적인 글로벌 플레이 테스트에 기여하였습니다.

### 3. 기술 스택 및 개발 환경 (Tech Stack & Development Environment)

*   **게임 엔진**: Unreal Engine 5
*   **주요 언어**: C++, Go
*   **통합 개발 환경 (IDE)**: Visual Studio, VS Code
*   **데이터베이스 (DB)**: MongoDB
*   **버전 관리 시스템 (VCS)**: Git, SVN
*   **협업 툴**: Redmine (프로젝트 관리), Confluence (문서 협업), Jenkins Build (CI/CD)

### 4. 주요 구현 기능 및 기여 사항 (Key Implemented Features & Contributions)

본 프로젝트에서 클라이언트 프로그래머로서 제가 담당하거나 기여한 핵심 기능들은 다음과 같습니다.
　  
#### 4.1. 핵심 게임플레이 흐름 구축
*   **[Owner / 전담 담당]** 사용자의 매칭 대기부터 인게임 진입, 플레이, 그리고 게임 종료까지의 **전반적인 인/아웃게임 플레이 흐름 구축**
<img width=30% height=30% alt="게임플레이_흐름_구축_1" src="https://github.com/user-attachments/assets/f3e112f0-c742-4f6d-8e2c-e4b37354df4f" />
<img width=30% height=30% alt="게임플레이_흐름_구축_3" src="https://github.com/user-attachments/assets/551d03ec-d26f-4394-876e-d591103a9137" />
<img width=30% height=30% alt="게임플레이_흐름_구축_4" src="https://github.com/user-attachments/assets/aa1f73d0-4ce5-4d41-b0d4-10eaa76c58fa" />
<img width=30% height=30% alt="게임플레이_흐름_구축_5" src="https://github.com/user-attachments/assets/11fdeff8-54e4-472d-bde7-71a0fbf66e31" />
<img width=30% height=30% alt="게임플레이_흐름_구축_6" src="https://github.com/user-attachments/assets/f1e1c516-b27a-4acf-a58a-55a2ab63d0ba" />
<img width=30% height=30% alt="게임플레이_흐름_구축_7" src="https://github.com/user-attachments/assets/f271e9d2-4ac9-4357-97b0-bcb63b6ef62a" />

　  
#### 4.2. 인게임 컨텐츠 개발
*  **[Maintainer]** **인게임 상호작용 및 인벤토리 시스템** 및
*  **[Owner / 전담 담당]** **아이템 상자 및 탈출포드 시스템, 인벤토리 UI/UX**를 담당하여 유저의 액션에 따른 보상 획득 로직 처리
<img width=30% height=30% alt="인게임_컨텐츠_개발_아이템상자_1" src="https://github.com/user-attachments/assets/e60b3801-4b18-48d8-8dcd-7013ca29f228" />
<img width=30% height=30% alt="인게임_컨텐츠_개발_아이템상자_2" src="https://github.com/user-attachments/assets/ac44a0a1-5ade-45b0-9265-6965494ab490" />
<img width=30% height=30% alt="인게임_컨텐츠_개발_아이템상자_3" src="https://github.com/user-attachments/assets/c97ae170-b42f-45a0-bcfa-6456a80c2f74" />
<img width=30% height=30% alt="인게임_컨텐츠_개발_아이템상자_탈출포드" src="https://github.com/user-attachments/assets/1c08e197-9e7b-4e54-a09a-8c5abb313ff7" />

　  
*   **[Maintainer]** **인게임 맵/미니맵 기능**을 담당하여 플레이어의 현재 위치 및 주변 환경 정보를 시각적으로 제공하고, 전략적인 플레이 지원
<img width=19.5% height=19.5% alt="인게임_컨텐츠_맵_미니맵_1" src="https://github.com/user-attachments/assets/3ae23ced-3479-4914-8bf1-033b645a5e26" />
<img width=30% height=30% alt="인게임_컨텐츠_맵_미니맵_2" src="https://github.com/user-attachments/assets/1d4835a3-f3e3-4c55-89d6-32ecd7f30cee" />

　  
#### 4.3. 커뮤니티 및 상점 시스템 클라이언트 개발
*   **[Owner / 전담 담당]** 멀티플레이어 환경에서의 **파티 시스템 클라이언트 로직**을 구현하여 유저 간의 협동 플레이 지원
<img width=30% height=30% alt="파티시스템_1" src="https://github.com/user-attachments/assets/7c0eed9d-dd9e-460b-b3d4-57b6dd00af1a" />
<img width=30% height=30% alt="파티시스템_2" src="https://github.com/user-attachments/assets/717df594-45ce-4ae6-875f-42736e97a642" />

　  
*   **[Owner / 전담 담당]** 게임 내 **상점 클라이언트**를 개발하여 아이템 구매 및 판매 기능을 직관적인 UI로 제공
<img width=30% height=30% alt="아웃게임_컨텐츠_상점_1" src="https://github.com/user-attachments/assets/aa056e52-758e-4cac-991d-33958d428c9a" />
<img width=30% height=30% alt="아웃게임_컨텐츠_상점_2" src="https://github.com/user-attachments/assets/541faf22-755f-40f4-84ca-9089ac3ceb7a" />
<img width=30% height=30% alt="아웃게임_컨텐츠_상점_3" src="https://github.com/user-attachments/assets/e7feb8a6-226b-4942-889b-c8b1c7709b55" />
<img width=30% height=30% alt="아웃게임_컨텐츠_상점_4" src="https://github.com/user-attachments/assets/47a2c7a9-41cb-4a94-85a9-829731e822fe" />

　  
#### 4.4. 데이터 연동 및 UI 처리
*   **[Maintainer]** **Json을 활용하여 웹 서버 DB와의 Read/Write 통신 로직**을 통한 게임 내 동적 데이터 관리 및 연동 경험
*   **[Owner / 전담 담당]** **UMG(Unreal Motion Graphics)를 활용한 UI 프로그래밍**에 전반적으로 대응하여 다양한 인게임 및 아웃게임 UI를 적용하고 사용자 경험 최적화

#### 4.5. 툴 제작 경험 – 로비/인게임 테스트 보조용 디버깅 기능 [Owner / 전담 담당]

- **디자이너 협업 사례**  
  UI 디자이너가 멀티플레이 UI 테스트 과정에서 겪는 불편함을 해소하기 위해,  
  **로비에서는 싱글 상태에서도 멀티플레이 UI를 확인할 수 있는 디버그 위젯**,  
  **인게임에서는 실시간 파티 Join/Leave가 가능한 Cheat 기능**을 직접 구현하고 제공했습니다.

- **기능 구분**  
  - **로비 디버그 위젯**  
    - 버튼/파라미터 조작만으로 2인/3인 파티 상태 구성 가능
    - 더미 플레이어 정보 출력, Leader/Member/Ready 상태 시뮬레이션
    - 파티 상태에서만 활성화되는 UI 기능 테스트 지원 
  - **인게임 Cheat 기능**  
    - RPC 기반 실시간 파티 Join/Leave 조작  
    - 파티원 HUD 동기화 상태 확인 가능

- **성과 및 효과**  
  UI 디자이너가 클라이언트 다중 실행 없이도 반복 테스트를 빠르게 진행할 수 있게 되었고,  
  **UI 피드백 주기 단축**, **수정 사이클 가속화**, **협업 효율 향상**에 실질적으로 기여했습니다.

#### 4.6. 운영 및 안정성 강화 
*   **[협업 지원]** **SteamFest JP / US Region의 Dedicated Server 및 MongoDB DB 관리**를 담당하여 글로벌 테스트 환경의 안정성 확보
*   **[협업 지원]** **서버 머신/DB 관리 및 빌드 대응** 업무를 수행하며 배포 및 운영 전반에 기여
*   **[협업 지원]** 발생하는 **크래시(Crash) 분석 및 수정, 버그(Bug Fix)** 에 적극 대응하여 게임의 안정성과 완성도 향상에 기여
<!--
### 5. 기술적 도전과 해결 과정 (Technical Challenges & Solutions)

#### 5.1. [구체적인 문제점 작성 예: Dedicated Server 환경에서의 클라이언트와 서버 간 데이터 동기화 최적화]
*   **문제 상황**: [...]
*   **분석 과정**: [...]
*   **해결 방안 및 구현**: [...]
    ![도전 1 해결](https://raw.githubusercontent.com/your-username/your-repo/main/images/challenge1_solution.png)
    *(선택: 문제 상황을 보여주는 스크린샷 또는 해결 방안의 핵심이 되는 아키텍처 다이어그램/코드 스니펫)*

#### 5.2. [구체적인 문제점 작성 예: 복잡한 인게임 UI의 성능 최적화 및 확장성 확보]
*   **문제 상황**: [...]
*   **분석 과정**: [...]
*   **해결 방안 및 구현**: [...]
    ![도전 2 해결](https://raw.githubusercontent.com/your-username/your-repo/main/images/challenge2_solution.png)
    *(선택: 최적화 전/후 UI 프레임 비교 스크린샷 또는 UI 아키텍처 다이어그램)*

#### 5.3. [구체적인 문제점 작성 예: 퀘스트 시스템의 데이터 주도 설계 및 게임 데이터 연동]
*   **문제 상황**: [...]
*   **분석 과정**: [...]
*   **해결 방안 및 구현**: [...]
    ![도전 3 해결](https://raw.githubusercontent.com/your-username/your-repo/main/images/challenge3_solution.png)
    *(선택: 퀘스트 데이터 테이블 구조 또는 데이터 연동 흐름도)*
-->
### 5. 성과 및 배운 점 (Achievements & Lessons Learned)

*   본 프로젝트를 통해 Dedicated Server 환경에서의 **멀티플레이어 게임 클라이언트 개발 전반에 대한 깊이 있는 이해와 실전 경험**을 쌓았습니다.
*   글로벌 플레이 테스트를 성공적으로 진행하며, **실제 유저 피드백을 기반으로 게임을 개선하는 과정**을 경험하고, 안정적인 서비스 운영의 중요성을 깨달았습니다.
*   C++과 Go 언어, 그리고 MongoDB를 아우르는 다양한 기술 스택을 경험하며, **서로 다른 시스템 간의 연동 및 문제 해결 능력**을 한층 더 발전시킬 수 있었습니다.

### 6. 이미지 출처 및 참고 영상 링크 (Video Links)
*   **[프로젝트 플레이 참고영상_솔로 (YouTube)](https://www.youtube.com/watch?v=YABNqBDIPUo)**
*   **[프로젝트 플레이 참고영상_파티 (YouTube)](https://www.youtube.com/watch?v=TTiAwMBl4nw)**
*   위 링크는 사용자 플레이 영상(UGC)로, 당사/개발사의 공식 자료가 아닙니다.   
    링크 만료/삭제가 발생할 수 있으며, 영상의 저작권은 각 업로더 또는 권리자에게 있습니다.
