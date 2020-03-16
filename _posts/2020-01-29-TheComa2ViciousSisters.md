---
layout: post
title:  "The Coma2 Vicious Sisters"
date:   2020-01-29 00:00:00 +0530
term:   2018.10 ~ 2020.02
categories: Game Unity DevespressoGames
---
  

<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/logo.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/logo.png"></a></center>
  

---
### 설명
**OGN 2020 2월 G-RANK 챌린지 서울상 수상작**  
Devespresso Games에서 개발한 2D 횡스크롤 미스테리 공포 게임 **"The Coma2: Vicious Sisters"** 입니다.  
전작 **"The Coma: Cutting Class"**의 후속작으로, 쫒아오는 킬러를 피해 퍼즐과 QTE를 해결해 나가는 런앤하이드 게임입니다.  
갑작스럽게 코마 세계에 들어온 주인공 "미나"가 위기를 피해 현실 세계로 탈출하는 이야기를 담았습니다.

---
### 관련 페이지
[Steam Store][url-steam]{: target="_blank"}  
[GOG Store][url-gog]{: target="_blank"}  
[트레일러 영상][url-trailer]{: target="_blank"}  
[플래이 영상1][url-play-0]{: target="_blank"}  
[플래이 영상2][url-play-1]{: target="_blank"}  

---
### 개발 기간
2018.10 ~ 2020.02

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
* Unity 2018.3.3f1

**플러그인**  
* UniRx
* Spine
* TextMesh Pro
* InControl
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
1. 스테이트 패턴을 이용한 AI 구성
2. QTE 시스템
3. 소모 아이템 구현
4. 버프, 디버프 구현
5. 퀘스트 시스템 구현
6. 비쥬얼 노벨 스타일의 대화 시스템과 분기를 통한 엔딩 결정
7. UGUI를 이용한 다양한 UI
8. 웹툰 스타일의 컷씬
9. 쉐이더를 사용한 화면 효과
10. 현재 위치에 맞춰 업데이트 되는 지도
11. 원근감을 위한 Parallax 맵 구현
12. AssetBundle을 이용한 플래이어 DLC 코스튬
13. 다양한 컨트롤러 지원
    * 키보드
    * PS 컨트롤러
    * Xbox 컨트롤러
14. 설정 기능
    * SFX, BGM, Movie 볼륨
    * 창 모드
    * 해상도
    * 9개 언어
    * 컨트롤러 확인 키 변경
    * 화면 밝기

**협업 툴** 
1. 디자이너가 쉽게 레벨을 생성할 수 있도록 UnityEditor를 통한 맵 생성 툴 개발 (맵, 이벤트 설치)
2. 인게임 애니메이션 씬을 인스팩터를 통해 만들 수 있는 툴 개발

**최적화**
1. Sprite Atlas를 통해서 드로우콜 최소화
2. 가능한 영역에서 Static Batch 사용
3. 플래이어가 존재하는 구역 외 맵은 Active를 Off해서 불필요한 비용 감소

**기타**
1. Git-flow 전략을 통한 브랜치 관리
2. Steam, GOG SDK를 이용한 업적 시스템, 클라우드 세이브
3. Unity Analytics을 이용한 활동 분석

**Vambrace: Cold Soul에서 개선점**
1. 기존 모듈을 상속 중심에서 컴포넌트 중심으로 리팩토링
2. 패치 및 메모리 관리의 편리함을 위해 Resources를 사용하지않고 AssetBundle을 사용
3. Atlas 생성을 플러그인 AtlasGenerator을 사용하지 않고 Unity2018부터 제공되는 Sprite Atlas를 사용
4. 시간 관리가 편리한 UniRx를 실험적으로 사용
5. 퀘스트 시스템이 씬 로딩 과정에서 해당 씬의 퀘스트만 캐시해 연산을 준비하게 하는 과정 추가하여 플래이중 실행 속도를 개선
6. 대화 시스템에 스킵, 강제 종료 등 기능을 추가하여 개선
7. 인게임 애니메이션 씬을 스크립트 없이 인스팩터 설정를 통해 제작할 수 있도록 변경
8. 게임패드 컨트롤러의 확인 키를 설정하여 선택할 수 있게 변경 

---
### 경험 및 이슈



---
### 이미지
* 메인 메뉴
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/mainmenu.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/mainmenu.png"></a></center>

* 탐험
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/play0.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/play0.png"></a></center>

* 숨기
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/play1.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/play1.png"></a></center>
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/play2.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/play2.png"></a></center>

* QTE
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/qte.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/qte.png"></a></center>
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/craft.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/craft.png"></a></center>

* 피격
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/attack0.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/attack0.png"></a></center>
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/attack1.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/attack1.png"></a></center>

* 잡기
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/catch.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/catch.png"></a></center>

* 대화
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/dialogue.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/dialogue.png"></a></center>

* 컷씬
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/cutscene.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/cutscene.png"></a></center>

* 인벤토리
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/inventory.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/inventory.png"></a></center>

* 자판기 상점
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/vending.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/vending.png"></a></center>

* 노트
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/note.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/note.png"></a></center>

* 옵션
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/option.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/option.png"></a></center>

* 업적
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/achievement.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/achievement.png"></a></center>

* DLC 코스튬
<center><a href="https://ironkim.github.io/assets/image/project/thecoma2/dlc.png" target="_blank"><img class="post-img" src="https://ironkim.github.io/assets/image/project/thecoma2/dlc.png"></a></center>

[url-steam]: https://store.steampowered.com/app/1045720/The_Coma_2_Vicious_Sisters
[url-gog]: https://www.gog.com/game/the_coma_2_vicious_sisters
[url-trailer]: https://youtu.be/FxuzlLULr18
[url-play-0]: https://youtu.be/F9pJZmC9nik
[url-play-1]: https://youtu.be/NQ-7fCQG1QM

