---
layout: post
title:  "The Coma2: Vicious Sisters"
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
* 스테이트 패턴을 이용한 AI 구성
* QTE 시스템
* 소모 아이템 구현
* 버프, 디버프 구현
* 퀘스트 시스템 구현
* 비쥬얼 노벨 스타일의 대화 시스템과 분기를 통한 엔딩 결정
* UGUI를 이용한 다양한 UI
* 웹툰 스타일의 컷씬
* 쉐이더를 사용한 화면 효과
* 현재 위치에 맞춰 업데이트 되는 지도
* 원근감을 위한 Parallax 맵 구현
* AssetBundle을 이용한 플래이어 DLC 코스튬
* 다양한 컨트롤러 지원
    * 키보드
    * PS 컨트롤러
    * Xbox 컨트롤러
* 설정 기능
    * SFX, BGM, Movie 볼륨
    * 창 모드
    * 해상도
    * 9개 언어
    * 컨트롤러 확인 키 변경
    * 화면 밝기

**협업 툴** 
* 디자이너가 쉽게 레벨을 생성할 수 있도록 UnityEditor를 통한 맵 생성 툴 개발 (맵, 이벤트 설치)
* 인게임 애니메이션 씬을 인스팩터를 통해 만들 수 있는 툴 개발
* Google2U를 이용한 DB 내용 모듈 테스트

**최적화**
* Sprite Atlas를 통해서 드로우콜 최소화
* 가능한 영역에서 Static Batch 사용
* 플래이어가 존재하는 구역 외 맵은 Active를 Off해서 불필요한 비용 감소

**기타**
* Git-flow 전략을 통한 브랜치 관리
* Steam, GOG SDK를 이용한 업적 시스템, 클라우드 세이브
* Unity Analytics을 이용한 활동 분석

**Vambrace: Cold Soul에서 개선점**
* 기존 모듈을 상속 중심에서 컴포넌트 중심으로 리팩토링
* 패치 및 메모리 관리의 편리함을 위해 Resources를 사용하지않고 AssetBundle을 사용
* Atlas 생성을 플러그인 AtlasGenerator을 사용하지 않고 Unity2018부터 제공되는 Sprite Atlas를 사용
* 시간 관리가 편리한 UniRx를 실험적으로 사용
* 퀘스트 시스템이 씬 로딩 과정에서 해당 씬의 퀘스트만 캐시해 연산을 준비하게 하는 과정 추가하여 플래이중 실행 속도를 개선
* 대화 시스템에 스킵, 강제 종료 등 기능을 추가하여 개선
* 인게임 애니메이션 씬을 스크립트 없이 인스팩터 설정를 통해 제작할 수 있도록 변경
* 게임패드 컨트롤러의 확인 키를 설정하여 선택할 수 있게 변경 

---
### 경험 및 이슈
**Google2U를 이용한 테스트**  
Vambrace:Cold Soul 개발 당시 팀원들이 협업과정에서 Google Spreadsheet를 이용해서 Database 내용을 작성해 왔으며 이 결과물을 csv 파일로 다운로드하여 SQLite에 임포트해오는 과정으로 개발을 진행해왔습니다.  
하지만 한 번의 Spreadsheat 수정이 필요할 경우 위의 과정을 매번 반복한다는 점이 상당히 불편하였으며 진행 속도를 뎌디게 만들어 왔습니다.  
이 문제를 해결하기 위해 Unity에서 Google SpreadSheet에 접근해 다양한 포멧으로 다운로드 해주는 **Google2U**을 이용하여 Unity에서 Google SpreadSheet를 JSON으로 다운로드할 수 있도록 세팅한 뒤 이 JSON을 파싱해서 테스트를 진행할 수 있도록 계획하였습니다.  
이를 위해 Database 조회 클래스의 동일한 함수를 Scripting define symbols을 이용하여 Json, SQLite로 각각 구현하였습니다.  
그 결과 SpreadSheat 구성 내용을 테스트하는 과정에서는 JSON을 이용하는 상태로 보다 빠르게 수정 및 다운로드하여 진행하였으며 SpreadSheat 구성 내용이 결정되면 SQLite로 임포트하여 기존 과정을 1회로 축소할 수 있었습니다. 또한 Scripting define symbols로 JSON 기능을 실제 라이브용 빌드 시 포함되지 않도록 할 수 있었습니다.


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

