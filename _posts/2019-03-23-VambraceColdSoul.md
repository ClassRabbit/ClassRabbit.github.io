---
layout: post
title:  "Vambrace Cold Soul"
date:   2019-05-28
categories: Unity DevespressoGames
---

<img src="https://IronKim.github.io/assets/image/project/VambraceColdSoul/logo.jpg"> 

---
### 게임 설명
Devespresso Games에서 개발한 2D 횡스크롤 어드벤쳐 게임 **"Vambrace : Cold Soul"** 입니다.  
기본적인 RPG 기능을 토대로 **"Darkest Dungeon"**과 유사한 캐릭터 고용 방식 및 턴제 전투 시스템을 가진 로그라이크 게임입니다.  
얼어붙은 지하 도시에서 시작되는 주인공의 모험 이야기를 담은 게임으로 비주얼 노벨 방식의 시스템을 통해 진행되는 스토리와 선택지를 통해 3개의 엔딩을 경험할 수 있습니다.

---
### 관련 페이지
[Steam Store][steam-url]{: target="_blank"}  
[GOG Store][gog-url]{: target="_blank"}  
[트레일러 영상][trailer-url]{: target="_blank"}  
[마을 영상][town-url]{: target="_blank"}  
[전투 영상][combat-url]{: target="_blank"}  

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
* SpriteGenerator  
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
1. 턴제 전투 시스템
2. 10개의 캐릭터와 30개 이상의 몬스터, 각각의 스킬 구성
3. 장비 아이템, 소모 아이템 구현
4. 버프, 디버프 구현
5. 퀘스트 시스템
6. 비쥬얼 노벨 스타일의 대화 시스템과 분기를 통한 엔딩 결정
7. UGUI를 이용한 다양한 UI
8. 게임 내 탐험마다 새로운 경험을 위한 랜덤 맵 생성 (오브젝트 풀 사용을 이용해서 맵 오브젝트 재사용)
9.  다양한 컨트롤러 지원
    * 키보드
    * PS 컨트롤러
    * Xbox 컨트롤러
10. 설정 기능
    * SFX, BGM 볼륨 설정
    * 창 모드
    * 해상도
    * 8개 언어

**협업 툴** 
1. 디자이너가 쉽게 레벨을 생성할 수 있도록 UnityEditor를 통한 맵 생성 툴 개발 (맵, 이벤트 설치)

**최적화**
1. 스프라이트 아틀라스를 통해서 드로우콜 최소화
2. 가능한 영역에서 Static Batch 사용
3. 플래이어가 존재하는 구역 외 맵은 Active를 Off해서 불필요한 비용 감소

**기타**
1. Git-flow 전략을 통한 브랜치 관리
2. Steam, GOG SDK를 이용한 업적 시스템



[steam-url]: https://store.steampowered.com/app/904380/Vambrace_Cold_Soul/
[gog-url]: https://www.gog.com/game/vambrace_cold_soul
[trailer-url]: https://www.youtube.com/watch?v=iAbsjz1AMB8
[town-url]: https://www.youtube.com/watch?v=y2HeLfAQrYk
[combat-url]: https://www.youtube.com/watch?v=C1fLBnosflY
