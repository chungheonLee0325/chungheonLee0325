<div align="center">

<h1>👋 안녕하세요, Unreal Client Engineer 이충헌입니다</h1>
<h3>게임플레이·UI의 상태 흐름을 설계하고, 반복 작업은 도구와 측정으로 개선합니다.</h3>

[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=20&pause=1000&color=F75C7E&center=true&vCenter=true&width=600&lines=C%2B%2B+%2B+Unreal+Engine+Developer;Gameplay+%26+Multiplayer+Systems;Unreal+Editor+Tooling)](https://git.io/typing-svg)

</div>

<p align="center">
Unreal Engine C++ 기반 클라이언트·게임플레이 개발을 중심으로 작업합니다.<br>
서버 상태 수신부터 클라이언트 데이터 처리와 UMG/Slate 반영까지 연결하고,<br>
객체 수명·UI 입력·성능 문제를 코드 구조와 실제 측정 결과로 검토합니다.
</p>

<div align="center">

[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=Gmail&logoColor=white)](mailto:fire6376@gmail.com)
[![Steam](https://img.shields.io/badge/Steam-000000?style=for-the-badge&logo=steam&logoColor=white)](https://steamcommunity.com/id/fire6376/)

</div>

---

## 대표 작업 — Gameplay / Editor Tooling

<table width="100%" border="0" style="border:none; border-collapse: collapse;">
<tr style="border-bottom: 1px solid #d0d7de;">
<!-- 왼쪽: 이미지 및 영상 링크 -->
<td width="45%" valign="top" style="padding:15px;">
<a href="https://www.youtube.com/watch?v=TDRRWp6M_9E" target="_blank">
<img src="https://github.com/chungheonLee0325/Sonheim/raw/main/Doc/Gifs/Project_Overview.gif" alt="Sonheim Demo Thumbnail" width="100%"/>
</a>
<p align="center" style="margin-top: 10px;">
<a href="https://www.youtube.com/watch?v=TDRRWp6M_9E" target="_blank"><b>🎥 시연 영상 보기</b></a>
</p>
<hr>
<p style="margin-bottom: 5px;">📅 <strong>기간:</strong> 25.03 ~ 25.09 / 26.09 ~ 현재</p>
<p style="margin-bottom: 5px;">👥 <strong>구성:</strong> 초기 2인 팀 → 개인 확장 개발</p>
<p style="margin-bottom: 5px;"><strong>🔧 주요 기술:</strong></p>
<div align="center">
<img src="https://img.shields.io/badge/Unreal_Engine-5.5-313131?style=for-the-badge&logo=unrealengine&logoColor=white"/>
<img src="https://img.shields.io/badge/Multiplayer-blue?style=for-the-badge"/>
</div>
</td>
<!-- 오른쪽: 상세 설명 -->
<td width="55%" valign="top" style="padding:15px;">
<h3 align="center">Sonheim — UE5.5 Multiplayer Gameplay & UI</h3>
<p align="center" style="color: #57606a;">서버 권위 게임플레이와 데이터 기반 콘텐츠, 클라이언트 화면 구조를 연결한 액션 어드벤처</p>

<p>초기 2인 팀에서 전투·인벤토리·제작·포획 시스템을 구현한 뒤, 개인 개발로 도감·퀘스트·분기 던전·보스·월드맵·UI 프레임워크를 확장했습니다.</p>

<p><strong>주요 구현:</strong></p>
<ul>
<li><b>게임플레이·네트워크</b>: Server RPC, OwnerOnly FastArray, 스킬 UObject 복제, GameState Snapshot으로 실행 권한과 복제 범위를 구분했습니다.</li>
<li><b>콘텐츠 확장</b>: 게임플레이 이벤트를 도감·퀘스트 기록과 연결하고, 던전 Event/Action/Transition 및 보스 PatternClock·Telegraph를 데이터로 관리했습니다.</li>
<li><b>UI 아키텍처</b>: 게임 상태 → Delegate/RepNotify → Presenter/ViewData → Widget 경로를 정리하고, <code>GameUIFramework</code>로 화면 레이어·입력 모드·팝업·재사용 정책을 분리했습니다.</li>
<li><b>월드맵</b>: 플레이어별 탐험 안개를 미니맵·전체 지도에서 공유하고, 퀘스트·도감 위치와 빠른 이동 표석을 연동했습니다.</li>
<li><b>성능 분석</b>: 1080p/RTX 2070 SUPER 환경에서 아이템 교환 이벤트 프레임 <b>32.6 → 17.1ms</b>, 인벤토리 열기 <b>57.5 → 22.1ms</b>를 측정했습니다. 수집 조건과 원인은 Wiki에 기록했습니다.</li>
</ul>

<p align="center" style="margin-top: 20px;">
<a href="https://github.com/chungheonLee0325/Sonheim"><b>Repository</b></a>
&nbsp;|&nbsp;
<a href="https://github.com/chungheonLee0325/Sonheim/blob/main/Doc/Wiki/Home.md"><b>Tech Docs (01–21)</b></a>
&nbsp;|&nbsp;
<a href="https://github.com/chungheonLee0325/Sonheim/blob/main/Doc/Wiki/20_UI_Performance_Profiling.md"><b>UI 성능 분석</b></a>
</p>
</td>
</tr>
</table>

---

## 🧰 Developer Tools & R&D

<table width="100%" border="0" style="border:none; border-collapse: collapse;">
<tr style="border-bottom: 1px solid #d0d7de;">
<td width="45%" valign="top" style="padding:15px;">

<a href="https://github.com/chungheonLee0325/AgentMcp" target="_blank">
<img src="https://github.com/chungheonLee0325/AgentMcp/raw/main/Docs/Images/dungeon_result.jpg" alt="AgentMcp Dungeon UI Case Study" width="100%"/>
</a>

</td>

<td width="55%" valign="top" style="padding:15px;">

<h3 align="center">AgentMcp — Unreal Editor MCP · Agent Skills</h3>

<p><strong>UE 5.5·5.7에서 사용하는 Unreal Editor 플러그인으로, Claude Code·Codex가 프로젝트를 조사·수정·실행·검증할 수 있도록 MCP 도구와 작업별 Skill을 제공합니다.</strong></p>

<p>UE 5.8의 실험적 MCP/Toolset 및 Agent Skill 개념을 참고해 기존 버전에서 별도로 구현했습니다. <code>SKILL.md</code> 작업 지침을 런타임에 읽고, 에디터 조사·수정·실행 도구와 함께 제공합니다.</p>

<ul>
<li><b>Dynamic Agent Skills</b> — 기본 Skill을 에디터에서 제공하고, 프로젝트별 <code>SKILL.md</code>를 런타임에 읽어 덮어쓰기. <code>umg-authoring</code>·<code>blueprint-graphs</code>·<code>perf-investigation</code> 등</li>
<li><b>UMG / Blueprint</b> — Widget Tree·C++ <code>BindWidget</code> 검증, Widget Blueprint 및 Blueprint 노드 편집, Compile → PIE → Viewport/Log 확인</li>
<li><b>UI Performance</b> — CSV·Unreal Insights Trace·<code>ProfileGPU</code>를 분석하고, 반복 실행 간 편차를 고려해 수정 전후 비교</li>
<li><b>Editor AI Chat</b> — 에디터 내 채팅에서 계정 기반 에이전트를 호출하고 읽기/에셋/코드 권한 및 변경 승인 카드로 작업 범위 제어</li>
</ul>

<p>실제 Sonheim UI에서 기존에 측정하지 않았던 화면을 조사해 보관함 재생성 비용, Delegate 중복 구독, 알림 오류를 확인·수정한 과정을 기록했습니다.</p>

<p align="center" style="margin-top: 20px;">
<a href="https://github.com/chungheonLee0325/AgentMcp"><b>Repository</b></a>
&nbsp;|&nbsp;
<a href="https://github.com/chungheonLee0325/AgentMcp/blob/main/Docs/Samples/SonheimUiPerf.ko.md"><b>성능 조사 기록</b></a>
&nbsp;|&nbsp;
<a href="https://github.com/chungheonLee0325/AgentMcp/blob/main/Docs/Samples/DungeonUi.ko.md"><b>UMG 제작 사례</b></a>
</p>
</td>
</tr>
</table>

---

## 🛠️ 기술 스택 (Tech Stack)

<div align="center">

| Languages | Engines | Game Development Specialties |
| :---: | :---: | :---: |
| ![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white) <br> ![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white) | ![Unreal Engine](https://img.shields.io/badge/Unreal_Engine-313131?style=for-the-badge&logo=unrealengine&logoColor=white) <br> ![Unity](https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white) | `Gameplay Systems` `Multiplayer / Replication` <br> `UMG / Slate UI` `Unreal Editor Tooling` <br> `Data-Driven Design` `Gameplay Ability System` |

</div>

---

## 🏢 업무 경력 (Work Experience)

| 회사 | 기간 | 직무 및 주요 업무 | 사용 기술 |
| :---: | :---: | :--- | :---: |
| **Unreal Engine 기반 크로스플랫폼 MMORPG(라이브 서비스)** | 2025.11 ~ 2026.09 | **UE5 MMORPG 클라이언트 콘텐츠/UI 개발** <br> • 공성전·길드 파티·복구 쿠폰 등 서버 연동 콘텐츠 구현 <br> • UMG/Slate UI 데이터 반영·입력 처리 정책 개선 <br> • Editor Tool 개발, UObject 수명·크래시 원인 분석 | <img src="https://img.shields.io/badge/Unreal_Engine-0E1128?style=flat-square&logo=unrealengine&logoColor=white" /> <br> <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" /> <br> <img src="https://img.shields.io/badge/Blueprint-1E90FF?style=flat-square" /> <br> <img src="https://img.shields.io/badge/Slate_UI-2F4F4F?style=flat-square" /> |
| **모바일 MMORPG 개발사** | 9개월 | **모바일 MMORPG 서버/클라이언트 개발** <br> • 레이드 보스 시스템 (페이즈, 패턴, 난이도) <br> • 영웅 성장 시스템 설계 <br> • 스킬 시스템 개선 (예약, 확장, 인디케이터) <br> • FSM 기반 몬스터 AI 구현 | <img src="https://img.shields.io/badge/Unity-000000?style=flat-square&logo=unity&logoColor=white" /> <br> <img src="https://img.shields.io/badge/C%23-239120?style=flat-square&logo=c-sharp&logoColor=white" /> |
| **차량용 SW/툴 개발사** | 2년 7개월 | **차량용 설계 도구 및 SW 개발** <br> • RapidAUTO Tool 연동 기능 개발 <br> • Windows 애플리케이션 기능 개발/유지보수 <br> • 전기차 BMS 시스템 코드 변환 컨설팅 | <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" /> <br> <img src="https://img.shields.io/badge/Windows_API-0078D6?style=flat-square&logo=windows&logoColor=white" /> |
---

### 프로젝트 문서 안내

이 페이지에서는 프로젝트별 핵심 구현을 소개합니다. 시연과 기능 구성은 **Repository README**, 구조·코드·기술 선택은 **Tech Docs**에서 확인할 수 있습니다.

---

## 📝 기술 아티클

<div>
  <h4>UE5 개발 중 마주친 문제들의 원인 분석과 해결 과정</h4>
  <p>구현 중 확인한 Unreal Engine 동작과 재현·수정 과정을 정리했습니다.</p>
</div>

| 아티클 | 내용 |
| :--- | :--- |
| [AnimNotifyState 인스턴스 공유 문제](https://github.com/chungheonLee0325/ue5-troubleshooting/blob/main/animnotifystate-instance-sharing.md) | 여러 캐릭터가 같은 NotifyState 인스턴스를 공유해서 생기는 문제와 해결 |
| [Fast Array로 인벤토리 동기화하기](https://github.com/chungheonLee0325/ue5-troubleshooting/blob/main/fast-array-inventory.md) | TMap 리플리케이션 불가 문제, FFastArraySerializer로 델타 동기화 구현 |
| [Listen Server에서 소켓 기반 공격이 실패하는 이유](https://github.com/chungheonLee0325/ue5-troubleshooting/blob/main/listen-server-lod-socket.md) | LOD가 소켓 위치 계산에 미치는 영향과 SetForcedLOD 해결책 |
| [BindWidget vs GetWidgetFromName](https://github.com/chungheonLee0325/ue5-troubleshooting/blob/main/bindwidget-vs-getwidgetfromname.md) | GetWidgetFromName의 O(N) 트리 순회 비용, BindWidget이 효율적인 이유 |
| [UScrollBox 버튼 드래그 스크롤 문제](https://github.com/chungheonLee0325/ue5-troubleshooting/blob/main/scrollbox-button-drag.md) | Slate 이벤트 버블링과 FReply, PreciseClick 원리<br><br>**심화:** [터치와 마우스의 엔진 레벨 동작 차이](https://github.com/chungheonLee0325/ue5-troubleshooting/blob/main/scrollbox-touch-vs-mouse.md) |

<p align="center">
  <a href="https://github.com/chungheonLee0325/ue5-troubleshooting" target="_blank"><b>📁 전체 보기</b></a>
</p>

---



## 그 외 프로젝트 (Other Projects)
<table width="100%" border="0" style="border:none; border-collapse: collapse;">
<!-- ================================================================================================================= -->
<!-- 프로젝트 1: VALORANT -->
<tr style="border-bottom: 1px solid #d0d7de;">
<!-- 왼쪽: 이미지 및 영상 링크 -->
<td width="45%" valign="top" style="padding:15px;">
<a href="https://www.youtube.com/watch?v=Ym0MJUSHHbc" target="_blank">
<img src="https://github.com/chungheonLee0325/VALORANT/raw/main/Doc/Gifs/VALORITH_Overview.gif" alt="VALORANT Gameplay GIF" width="100%"/>
</a>
<p align="center" style="margin-top: 10px;">
<a href="https://www.youtube.com/watch?v=Ym0MJUSHHbc" target="_blank"><b>🎥 시연 영상 보기</b></a>
</p>
<hr>
<p style="margin-bottom: 5px;">📅 <strong>기간:</strong> 25.05 ~ 25.06 (2M)</p>
<p style="margin-bottom: 5px;">👥 <strong>구성:</strong> 7인 팀 프로젝트</p>
<p style="margin-bottom: 5px;"><strong>🔧 주요 기술:</strong></p>
<div align="center">
<img src="https://img.shields.io/badge/Unreal_Engine-5.5-313131?style=for-the-badge&logo=unrealengine&logoColor=white"/>
<img src="https://img.shields.io/badge/GAS-F85A5A?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Multiplayer-blue?style=for-the-badge"/>
</div>
</td>
<!-- 오른쪽: 상세 설명 -->
<td width="55%" valign="top" style="padding:15px;">
<h3 align="center">VALORANT (Multiplay Hypher FPS 게임)</h3>
<p align="center" style="color: #57606a;">
GAS를 활용하여 주요 시스템을 구현한 멀티플레이 하이퍼 FPS
</p>
<p>
4종의 에이전트와 12개 스킬을 공통 Ability 구조로 구현했습니다. Spike 설치·해체 상태 머신과 라운드별 상점·경제 처리를 서버 판정 경로에 연결했습니다.
</p>
<div>
<p><strong>담당 개발 및 역할:</strong></p>
<ul>
<li><b>모듈화된 어빌리티 설계</b>: 준비→대기→실행 상태 흐름과 후속 입력·투사체·장판형 스킬의 공통 실행 경로를 구성했습니다.</li>
<li><b>다양한 스킬 메커니즘 구현</b>: 즉발형(Jett), 후속입력형(KAY/O) 등 여러 에이전트의 스킬을 공통 시스템 내에서 구현했습니다.</li>
<li><b>핵심 게임 루프 구축</b>: Spike 설치·해체 상태와 라운드 전환, 구매 가능 시점 및 재화 갱신을 연결했습니다.</li>
<li><b>서버 검증·입력 라우팅</b>: 서버에서 스킬 사용·구매 조건을 검사하고 GameplayTag로 입력을 분기했습니다.</li>
</ul>
</div>
<p align="center" style="margin-top: 20px;">
<a href="https://github.com/chungheonLee0325/VALORANT" target="_blank"><b>📁 Repository README</b></a>
&nbsp;|&nbsp;
<a href="https://github.com/chungheonLee0325/VALORANT/wiki" target="_blank"><b>🔗 Tech Docs</b></a>
</p>
</td>
</tr>
<!-- ================================================================================================================= -->
<!-- 프로젝트: Fishing Is Good -->
<tr style="border-bottom: 1px solid #d0d7de;">
<!-- 왼쪽: 이미지 및 영상 링크 -->
<td width="45%" valign="top" style="padding:15px;">
<a href="https://chungheonlee0325.github.io/FishingIsGood/Media/videos.html#unity" target="_blank">
<img src="https://github.com/chungheonLee0325/FishingIsGood/raw/main/Media/unity-gameplay-preview.gif" alt="Fishing Is Good Unity Gameplay" width="100%"/>
</a>

<p align="center" style="margin-top: 10px;">
<a href="https://chungheonlee0325.github.io/FishingIsGood/Media/videos.html#unity" target="_blank"><b>🎥 웹에서 영상 보기</b></a>
</p>

<hr>

<p style="margin-bottom: 5px;">📌 <strong>형태:</strong> 개인 프로토타입</p>
<p style="margin-bottom: 5px;">👤 <strong>구성:</strong> 개인 개발</p>
<p style="margin-bottom: 5px;"><strong>🔧 주요 기술:</strong></p>

<div align="center">
<img src="https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white"/>
<img src="https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white"/>
<img src="https://img.shields.io/badge/HTML%20Prototype-1E1E1E?style=for-the-badge&logo=html5&logoColor=E34F26"/>
</div>
</td>

<!-- 오른쪽: 상세 설명 -->
<td width="55%" valign="top" style="padding:15px;">
<h3 align="center">Fishing Is Good (HTML/Unity Prototype)</h3>

<p align="center" style="color: #57606a;">
전통적인 낚시 미니게임보다, 물고기를 지켜보는 재미와 최소한의 개입에 초점을 둔 탑다운 낚시 프로토타입
</p>

<p>
방치형 게임에 맞게 반복 입력이나 타이밍 조작을 줄이고, 물고기의 움직임을 지켜보다가 찌를 놓을 위치를 고르는 플레이를 만들었습니다.
이를 위해 물고기의 이동과 반응을 빠르게 반복 검증할 수 있는 HTML 프로토타입을 먼저 만들고, 직접 플레이하며 남길 규칙을 정한 뒤 Unity에서 게임플레이와 수중 연출로 구현했습니다.
</p>

<div>
<p><strong>주요 작업:</strong></p>
<ul>
<li><b>행동 검증</b>: HTML 프로토타입에서 이동, 선회, 회피, 접근, 먹이 반응과 찌 배치에 따른 반응을 빠르게 비교하며 조정했습니다.</li>
<li><b>낚시 흐름</b>: 찌 배치 → 관심·접근 → 입질 → 회수 → 낚시 가방 도착 → 점수·수량 집계까지 구현했습니다.</li>
<li><b>시각 표현</b>: 어종별 메시 생성과 움직임 셰이더를 구현하고, 수면 굴절·그림자·착수 파문·렌즈 물방울·수중 카메라 전환을 제작했습니다.</li>
<li><b>개발 방식</b>: AI를 구현 대안 탐색과 반복 작업에 활용하고, 실제 실행 결과를 보며 채택·수정·폐기할 요소를 결정했습니다.</li>
</ul>
</div>

<p align="center" style="margin-top: 20px;">
<a href="https://github.com/chungheonLee0325/FishingIsGood" target="_blank"><b>📁 Repository README</b></a>
&nbsp;|&nbsp;
<a href="https://chungheonlee0325.github.io/FishingIsGood/HTML/" target="_blank"><b>🌐 Browser Prototype</b></a>
</p>
</td>
</tr>
<!-- ================================================================================================================= -->
<!-- 프로젝트 3: Tazan -->
<tr>
<!-- 왼쪽: 이미지 및 영상 링크 -->
<td width="45%" valign="top" style="padding:15px;">
<a href="https://youtu.be/vQU0mdTJhvQ" target="_blank">
<img src="https://user-images.githubusercontent.com/83523295/233767521-17c37466-0752-411a-a312-b98e72b4f918.gif" alt="Tazan Gameplay GIF" width="100%"/>
</a>
<p align="center" style="margin-top: 10px;">
<a href="https://youtu.be/vQU0mdTJhvQ" target="_blank"><b>🎥 시연 영상 보기</b></a>
</p>
<hr>
<p style="margin-bottom: 5px;">📅 <strong>기간:</strong> 2025.02 ~ 2025.03 (1개월)</p>
<p style="margin-bottom: 5px;">👥 <strong>구성:</strong> 3인 팀 프로젝트</p>
<p style="margin-bottom: 5px;"><strong>🔧 주요 기술:</strong></p>
<div align="center">
<img src="https://img.shields.io/badge/Unreal_Engine-5.5-313131?style=for-the-badge&logo=unrealengine&logoColor=white"/>
</div>
</td>
<!-- 오른쪽: 상세 설명 -->
<td width="55%" valign="top" style="padding:15px;">
<h3 align="center">Tazan (소울라이크 게임)</h3>
<p align="center" style="color: #57606a;">
Poise 기반 경직 우선순위·패리·회피를 구현한 3인 팀 소울라이크 액션 게임
</p>
<p>
공격 강인도와 방어 강인도를 비교해 경직·Stagger를 판정하고, 행동 상태에 따라 패리·회피·차지 공격의 반응을 분기했습니다.
</p>
<div>
<p><strong>주요 구현 내용:</strong></p>
<ul>
<li><b>강인도 기반 경직 시스템</b>: 공격 강인도 vs 방어 강인도를 비교하고 경직 우선순위를 따져 상태를 갱신합니다.</li>
<li><b>Lock-on 타겟 선정</b>: 화면 중심과 대상 거리를 이용해 타겟을 선정하고, 타겟과의 거리에 따라 카메라를 조정합니다.</li>
<li><b>공격 충돌 판정</b>: 이전·현재 프레임 위치 사이를 보간해 히트 검사를 수행하고 여러 히트박스를 처리했습니다.</li>
<li><b>입력·애니메이션 연결</b>: Enhanced Input과 AnimNotifyState로 패리·회피·콤보 입력 가능 구간을 제어했습니다.</li>
</ul>
</div>
<p align="center" style="margin-top: 20px;">
<a href="https://github.com/chungheonLee0325/Tazan" target="_blank"><b>📁 Repository README</b></a>
&nbsp;|&nbsp;
<a href="https://www.notion.so/Tazan-Project-C-1ff6058f0c2e80c68b38efdf320946f1?pvs=21" target="_blank"><b>🔗 Tech Docs</b></a>
</p>
</td>
</tr>
<!-- ================================================================================================================= -->

<!-- 프로젝트 4: Dororong World (Voice Command) -->

<tr style="border-bottom: 1px solid #d0d7de;">
<!-- 왼쪽: 이미지 및 영상 링크 -->
<td width="45%" valign="top" style="padding:15px;">
<a href="https://youtu.be/cXoGXADRAa8" target="_blank">
<img src="https://github.com/chungheonLee0325/VoiceCommand/raw/main/Document/Dororong World_resize.gif" alt="Dororong Work Gameplay GIF" width="100%"/>
</a>
<p align="center" style="margin-top: 10px;">
<a href="https://youtu.be/cXoGXADRAa8" target="_blank"><b>🎥 시연 영상 보기</b></a>
</p>
<hr>
<p style="margin-bottom: 5px;">📅 <strong>기간:</strong> 25.08 (2D 게임잼)</p>
<p style="margin-bottom: 5px;">👥 <strong>구성:</strong> 7인 팀 프로젝트 (게임팀 3, AI팀 4)</p>
<p style="margin-bottom: 5px;"><strong>🔧 주요 기술:</strong></p>
<div align="center">
<img src="https://img.shields.io/badge/Unreal_Engine-5.5-313131?style=for-the-badge&logo=unrealengine&logoColor=white"/>
</div>
</td>
<!-- 오른쪽: 상세 설명 -->
<td width="55%" valign="top" style="padding:15px;">
<h3 align="center">Dororong World (Voice Command)</h3>
<p align="center" style="color: #57606a;">
"도로롱, 제발 내 말좀 들어!!" - 음성 명령으로 팰을 조종하는 3D 자원 수집 게임
</p>
<p>
'AI와의 융합'을 주제로 한 게임잼에서 <strong>우승한 프로젝트</strong>입니다. 플레이어의 자연어 음성 명령을 AI가 분석하여 게임 내 '팰'에게 작업을 지시하는 직관적인 플레이 방식을 구현했습니다.
</p>
<div>
<p><strong>담당 개발 및 역할:</strong></p>
<ul>
<li><b>AI-게임 통신 시스템</b>: FastAPI 서버와 Unreal Engine 클라이언트 간의 실시간 통신 파이프라인을 구축하고, 음성 데이터 전송 및 분석된 명령(JSON)을 수신하는 기능을 구현했습니다.</li>
<li><b>음성 명령 라우팅 시스템</b>: 수신된 JSON 데이터를 분석하여 '모두', '아무나', '개인(특정 대상)' 등 적절한 대상에게 명령을 전달하는 로직을 개발했습니다.</li>
<li><b>핵심 게임 루프 구현</b>: 플레이어 캐릭터의 움직임, 자원(나무, 돌, 광석) 시스템, 레벨업 및 엔딩으로 이어지는 전체 게임 사이클을 구현했습니다.</li>
</ul>
</div>
<p align="center" style="margin-top: 20px;">
<a href="https://github.com/chungheonLee0325/VoiceCommand" target="_blank"><b>📁 Repository README</b></a>
</p>
</td>
</tr>

<tr>
<td width="45%" valign="top" style="padding:15px;">
<a href="https://github.com/chungheonLee0325/LostGPU" target="_blank">
<img src="https://github.com/chungheonLee0325/LostGPU/blob/main/Docs/LostGPU.gif?raw=true" alt="LostGPU Gameplay GIF" width="100%"/>
</a>
<p align="center" style="margin-top: 10px;">
<a href="https://youtu.be/mgP-u5mvh1c" target="_blank"><b>🎥 시연 영상 보기</b></a>
</p>
<hr>
<p style="margin-bottom: 5px;">📅 <strong>기간:</strong> 24.12 (1M)</p>
<p style="margin-bottom: 5px;">👥 <strong>구성:</strong> 3인 팀 프로젝트</p>
<p style="margin-bottom: 5px;"><strong>🔧 주요 기술:</strong></p>
<div align="center">
<img src="https://img.shields.io/badge/Unreal_Engine-5.5-313131?style=for-the-badge&logo=unrealengine&logoColor=white"/>
<img src="https://img.shields.io/badge/Blueprint-100%25-0D90E1?style=for-the-badge&logo=unrealengine&logoColor=white"/>
</div>
</td>
<td width="55%" valign="top" style="padding:15px;">
<h3 align="center">LostGPU (100% Blueprint 액션 RPG)</h3>
<p align="center" style="color: #57606a;">
Blueprint FSM과 데이터 테이블을 이용해 전투·보스 패턴을 구현한 액션 RPG
</p>
<p>
Unreal Engine 학습 초기의 팀 프로젝트로, C++ 없이 Blueprint에서 플레이어 액션, 보스 전투 FSM, 상태이상 및 레이드 진행을 구현했습니다.
</p>
<div>
<p><strong>담당 개발 및 역할:</strong></p>
<ul>
<li><b>FSM 기반 전투 로직</b>: 플레이어의 스킬 시전 제약 및 대쉬 캔슬, 보스의 확률/사정거리 기반 '스킬 룰렛' 등 복잡한 전투 상호작용을 FSM으로 구현했습니다.</li>
<li><b>스킬 데이터 분리</b>: 공통 <code>Base Skill Class</code>와 DataTable에서 스킬 피해·쿨타임·상태이상을 조회하도록 구성했습니다.</li>
<li><b>레이드 진행</b>: 보스 선택 → Sequencer 컷신 → 갑옷·지형 파괴가 포함된 전투 → 승패 처리 흐름을 연결했습니다.</li>
</ul>
</div>
<p align="center" style="margin-top: 20px;">
<a href="https://github.com/chungheonLee0325/LostGPU" target="_blank"><b>📁 Repository README</b></a>
</p>
</td>
</tr>

</table>
---
<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=chungheonLee0325&color=brightgreen&style=flat-square)

</div>
