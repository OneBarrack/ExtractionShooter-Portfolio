# Project GGG: PC PVPVE 쿼터뷰 루터 슈팅 익스트랙션 게임 개발

![Project GGG 대표 이미지](https://raw.githubusercontent.com/your-username/your-repo/main/images/main_gameplay.png)

---

### 1. 프로젝트 개요 (Project Overview)

*   **프로젝트명**: Project GGG
*   **개발 기간**: 2022년 10월 ~ 2024년 2월 (약 1년 4개월)
*   **플랫폼**: PC (Dedicated Server 기반 멀티플레이어)
*   **장르**: PVPVE 쿼터뷰 루터 슈팅 익스트랙션 (Quarter-view Looter Shooter Extraction)
*   **주요 성과**:
    *   2023년 12월, 스팀(Steam) 플랫폼에서 **글로벌 플레이 테스트**를 성공적으로 진행하였습니다.
    *   총 **7일간 약 4,000명의 유저**가 테스트에 참여하여 게임의 핵심 재미와 안정성을 검증받았습니다.

### 2. 개발 배경 및 본인 역할 (Development Background & My Role)

본 프로젝트는 스팀 글로벌 서비스를 목표로 한 멀티플레이어 쿼터뷰 루터 슈팅 게임 개발 프로젝트였습니다.  
저는 클라이언트 프로그래머로서 게임의 핵심 인/아웃게임 플레이 흐름 구현 및 UI/UX 시스템 개발을 주도하였으며,   
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
*   사용자의 매칭 대기부터 인게임 진입, 플레이, 그리고 게임 종료까지의 **전반적인 인/아웃게임 플레이 흐름을 C++과 블루프린트를 활용하여 구축**하였습니다. (State Machine 및 GameState/PlayerState 기반)
    ![게임 시작 화면](https://raw.githubusercontent.com/your-username/your-repo/main/images/game_start.png)
    *(게임 시작 화면 (로그인/메인 메뉴) 또는 인게임 진입 직후의 장면)*

#### 4.2. 인게임 컨텐츠 개발
*   **인게임 상호작용 보상 상자 시스템**을 구현하여 유저의 액션에 따른 보상 획득 로직을 처리하였습니다.
    ![보상 상자 UI](https://raw.githubusercontent.com/your-username/your-repo/main/images/loot_box_ui.png)
    *(보상 상자 오픈 또는 루팅 인터페이스 UI 스크린샷)*
*   **인게임 맵/미니맵 기능**을 개발하여 플레이어의 현재 위치 및 주변 환경 정보를 시각적으로 제공하고, 전략적인 플레이를 지원했습니다.
    ![맵/미니맵](https://raw.githubusercontent.com/your-repo/main/images/map_minimap.png)
    *(인게임 맵 또는 미니맵이 표시된 UI 스크린샷)*

#### 4.3. 커뮤니티 및 상점 시스템 클라이언트 개발
*   멀티플레이어 환경에서의 **파티 시스템 클라이언트 로직**을 구현하여 유저 간의 협동 플레이를 지원했습니다.
    ![파티 UI](https://raw.githubusercontent.com/your-username/your-repo/main/images/party_ui.png)
    *(파티 UI 또는 파티원 정보 UI 스크린샷)*
*   게임 내 **상점 클라이언트**를 개발하여 아이템 구매 및 판매 기능을 직관적인 UI로 제공했습니다.
    ![상점 UI](https://raw.githubusercontent.com/your-username/your-repo/main/images/shop_ui.png)
    *(상점 UI 스크린샷)*

#### 4.4. 퀘스트 시스템 개발
*   유저에게 목표를 부여하고 진행 상황을 추적, 보상을 지급하는 **퀘스트 시스템의 클라이언트 전반**을 구현했습니다. (데이터 기반의 확장성 고려)
    ![퀘스트 UI](https://raw.githubusercontent.com/your-username/your-repo/main/images/quest_ui.png)
    *(퀘스트 목록 UI 또는 퀘스트 진행 상황 표시 UI 스크린샷)*

#### 4.5. 데이터 연동 및 UI 처리
*   **Json을 활용하여 웹 서버 DB와의 Read/Write 통신 로직**을 개발, 게임 내 동적 데이터 관리 및 연동 경험을 쌓았습니다.
*   **UMG(Unreal Motion Graphics)를 활용한 UI 프로그래밍**에 전반적으로 대응하여 다양한 인게임 및 아웃게임 UI를 구현하고 사용자 경험을 최적화했습니다.
    ![다양한 UI 요소](https://raw.githubusercontent.com/your-username/your-repo/main/images/various_ui.png)
    *(여러 UI 요소 (HUD, 메뉴, 팝업 등)가 복합적으로 보여지는 인게임 스크린샷 (UMG 강조))*

#### 4.6. 운영 및 안정성 강화
*   **SteamFest JP / US Region의 Dedicated Server 및 MongoDB DB 관리**를 담당하여 글로벌 테스트 환경의 안정성을 확보했습니다.
*   **서버 머신/DB 관리 및 빌드 대응** 업무를 수행하며 배포 및 운영 전반에 기여했습니다.
*   발생하는 **크래시(Crash) 분석 및 수정, 버그(Bug Fix)** 에 적극 대응하여 게임의 안정성과 완성도 향상에 기여했습니다.
    ![안정적인 플레이](https://raw.githubusercontent.com/your-username/your-repo/main/images/stable_gameplay.png)
    *(선택: 게임이 안정적으로 구동되는 인게임 플레이 장면 또는 버그/크래시 수정 전후를 간접적으로 보여주는 스크린샷)*

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

### 6. 성과 및 배운 점 (Achievements & Lessons Learned)

*   본 프로젝트를 통해 Dedicated Server 환경에서의 **멀티플레이어 게임 클라이언트 개발 전반에 대한 깊이 있는 이해와 실전 경험**을 쌓았습니다.
*   글로벌 플레이 테스트를 성공적으로 진행하며, **실제 유저 피드백을 기반으로 게임을 개선하는 과정**을 경험하고, 안정적인 서비스 운영의 중요성을 깨달았습니다.
*   C++과 Go 언어, 그리고 MongoDB를 아우르는 다양한 기술 스택을 활용하며, **서로 다른 시스템 간의 연동 및 문제 해결 능력**을 한층 더 발전시킬 수 있었습니다.
    ![프로젝트 성과](https://raw.githubusercontent.com/your-username/your-repo/main/images/achievements.png)
    *(프로젝트의 성공을 보여주는 상징적인 이미지 (예: 스팀 플레이 테스트 결과 요약 화면, 핵심 플레이 장면 중 하나))*

### 8. 시각 자료 및 링크 (Visuals & Links)

*   **[프로젝트 플레이 영상 (YouTube)](https://www.youtube.com/watch?v=YABNqBDIPUo)**
