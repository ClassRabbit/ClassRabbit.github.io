---
layout: post
title:  "Vambrace: Cold Soul"
date:   2019-05-28 00:00:00 +0530
term:   2017.08 ~ 2019.05
categories: Game Unity DevespressoGames
---
  

<center><a href="https://ironkim.github.io/assets/image/project/vambrace/logo.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/vambrace/logo.png"></a></center>
  

---
### 설명
Devespresso Games에서 개발한 2D 횡스크롤 어드벤쳐 게임 **"Vambrace: Cold Soul"** 입니다.  
기본적인 RPG 기능을 토대로 **"Darkest Dungeon"**과 유사한 캐릭터 고용 방식 및 턴제 전투 시스템을 가진 로그라이크 게임입니다.  
얼어붙은 지하 도시에서 시작되는 주인공의 모험 이야기를 담은 게임으로 비주얼 노벨 방식의 시스템을 통해 진행되는 스토리와 선택지를 통해 3개의 엔딩을 경험할 수 있습니다.

---
### 관련 페이지
[Steam Store][url-steam]{: target="_blank"}  
[GOG Store][url-gog]{: target="_blank"}  
[Origin Store][url-origin]{: target="_blank"}  
[트레일러 영상][url-trailer]{: target="_blank"}  
[특징 영상][url-feature]{: target="_blank"}  
[마을 영상][url-town]{: target="_blank"}  
[전투 영상][url-combat]{: target="_blank"}  
[플래이 영상][url-play]{: target="_blank"}  

---
### 개발 기간
2017.08 ~ 2019.05

---
### 개발 인원
**총 4명**  
* 프로그래머(본인)
* 아트 디자이너
* 오디오
* 스토리 작가

---
### 개발 스팩
**엔진**  
* Unity 5.6.6f2

**플러그인**  
* Spine
* TextMesh Pro
* InControl
* AtlasGenerator  
* SQLite.net

**DB**
* SQLite  

**버전 관리**  
* Git
* Bitbucket

---
### 개발 역할
프로그래밍 전반

---
### 개발 요약
**게임 요소**
* 턴제 전투 시스템
* 10개의 캐릭터와 30개 이상의 몬스터, 각각의 스킬 구성
* 장비 아이템, 소모 아이템 구현
* 버프, 디버프 구현
* 퀘스트 시스템 구현
* 인벤토리 시스템 구현
* 비쥬얼 노벨 스타일의 대화 시스템 구현
* 분기를 통한 3가지 엔딩
* UGUI를 이용한 다양한 UI 구현
* 원근감을 위한 Parallax 맵 구현
* 게임 내 탐험마다 새로운 경험을 위한 랜덤 맵 생성  
  (오브젝트 풀 사용을 이용해서 맵 오브젝트 재사용)
* 다양한 컨트롤러 지원
    * 키보드
    * PS 컨트롤러
    * Xbox 컨트롤러
* 설정 기능
    * SFX, BGM 볼륨
    * 창 모드
    * 해상도
    * 8개 언어

**협업 툴** 
* 디자이너가 쉽게 레벨을 생성할 수 있도록 UnityEditor를 통한 맵 생성 툴 개발  
  (맵, 이벤트 설치)

**최적화**
* Sprite Atlas를 통해서 드로우콜 최소화
* 가능한 영역에서 Static Batching 사용
* 플래이어가 존재하는 구역 외 맵은 Active를 Off해서 불필요한 비용 감소

**기타**
* Git-flow 전략을 통한 브랜치 관리
* Steam, GOG, Origin SDK를 이용한 업적 시스템

---
### 경험 및 이슈
**PlayStation4 포팅**  
2018년 제 5회 PlayStation Arena 참가를 목적으로 PlayStation 포팅을 진행하며 다음과 같은 이슈를 경험하였습니다.

* 프래임 문제  
당시 타겟 기기의 사양으로 인한 프래임률의 차이를 고려하지 않고 개발된 부분이 존재하였습니다.  
프래임 차이로 발생할 수 있는 문제에 대하여 알 수 있었던 이슈였으며 FixedUpdate나 DeltaTime을 이용하는 방식으로 해결하였습니다. 

* 모듈 교체 이슈  
컨트롤 입력, 세이브, 동영상 재생 등 몇가지 모듈이 PlayStation에서 사용되는 방식으로 변경이 필요하였습니다.  
이를 위해 Git의 기존의 PC로만 진행해오던 Develop 브랜치를 Develop_PC 브랜치와 Develop_PS 브랜치로 나누웠습니다.  
이후 PlayStation 관련한 모듈은 Develop_PS 브랜치에서 개발하였으며 공통적인 Feature는 Develop_PC 브랜치에서 개발 후 Develop_PS 브랜치에 병합하는 방식으로 진행하였습니다.  

* PlayStation 기술지원팀과의 커뮤니케이션  
PlayStation 개발에 관련하여 접근이 제한적인 부분이 있기 때문에 개발 정보를 Google 검색을 통해서 얻기 어려웠습니다. 이 점을 극복하기 위해서 PS4 DevNet 사이트를 이용하여 능동적으로 현재 이슈를 작성하고 Unity PlayStation 개발지원팀의 응답에 맞춰 개발을 진행하였습니다.
  

---
### 이미지
* 메인 메뉴
<center><a href="https://ironkim.github.io/assets/image/project/vambrace/mainmenu.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/vambrace/mainmenu.png"></a></center>

* 마을 내부
<center><a href="https://ironkim.github.io/assets/image/project/vambrace/town0.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/vambrace/town0.png"></a></center>

* 마을 외부
<center><a href="https://ironkim.github.io/assets/image/project/vambrace/town1.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/vambrace/town1.png"></a></center>

* 전투
<center><a href="https://ironkim.github.io/assets/image/project/vambrace/combat.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/vambrace/combat.png"></a></center>

* 대화
<center><a href="https://ironkim.github.io/assets/image/project/vambrace/dialogue.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/vambrace/dialogue.png"></a></center>

* 고용
<center><a href="https://ironkim.github.io/assets/image/project/vambrace/employ.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/vambrace/employ.png"></a></center>

* 캐릭터 정보
<center><a href="https://ironkim.github.io/assets/image/project/vambrace/bio.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/vambrace/bio.png"></a></center>

* 인벤토리
<center><a href="https://ironkim.github.io/assets/image/project/vambrace/inventory.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/vambrace/inventory.png"></a></center>

* 노트
<center><a href="https://ironkim.github.io/assets/image/project/vambrace/note.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/vambrace/note.png"></a></center>

* 옵션
<center><a href="https://ironkim.github.io/assets/image/project/vambrace/option.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/vambrace/option.png"></a></center>

* 업적
<center><a href="https://ironkim.github.io/assets/image/project/vambrace/achievement.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/vambrace/achievement.png"></a></center>

[url-steam]: https://store.steampowered.com/app/904380/Vambrace_Cold_Soul
[url-gog]: https://www.gog.com/game/vambrace_cold_soul
[url-origin]: https://www.origin.com/kor/ko-kr/store/vambrace-cold-soul/vambrace-cold-soul
[url-trailer]: https://www.youtube.com/watch?v=iAbsjz1AMB8
[url-feature]: https://youtu.be/VH2GtnaYft8
[url-town]: https://www.youtube.com/watch?v=y2HeLfAQrYk
[url-combat]: https://www.youtube.com/watch?v=C1fLBnosflY
[url-play]: https://www.youtube.com/watch?v=aVg0BLUnitw
