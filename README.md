# 리틀파이터2 모작

## 시연 영상 및 게임 소개
<!--[![LittleFighter2 Demo](https://img.youtube.com/vi/2OhpsBg-Lko/0.jpg)](https://youtu.be/2OhpsBg-Lko)-->
[![LittleFighter2 Demo](https://img.shields.io/badge/YouTube-Video-red?logo=youtube)](https://youtu.be/2OhpsBg-Lko)  
<img width="240" alt="image" src="docs/images/overview_001.png" />
<img width="240" alt="image" src="docs/images/overview_002.png" />
<img width="240" alt="image" src="docs/images/overview_003.png" />

WinAPI 활용한 벨트스크롤 2D 액션 게임

- 비트 연산 활용한 커맨드 기능 구현
- 싱글톤 패턴을 이용한 매니저 기반 프레임워크 구현

## 핵심 기술

### 비트 연산 활용한 커맨드 기능 구현
[D 방어] ⇒ [→↑↓ 방향키] ⇒ [J or A 점프 혹은 공격]
원작의 커맨드 시스템이 반드시 위의 순서대로 입력해야 발동되도록 설계되어 있어 이를 구현하기 위해 비트 연산 활용  
<!--<img width="240" alt="image" src="https://github.com/user-attachments/assets/90266ac2-f8f6-430b-a35c-dfb2fe39d874" />-->
<img width="240" alt="image" src="docs/images/coretech_001.png" />
<img width="240" alt="image" src="docs/images/coretech_002.png" /><br>
가장 우선순위가 높은 [D 방어] 키가 입력됨에 따라 기존 커맨드 값이 초기화되는 모습

### 싱글톤 패턴을 이용한 매니저 기반 프레임워크 구현
<img width="500" alt="image" src="docs/images/coretech_003.png" /><br>
객체 생성을 1회로 제한하기 위한 DECLARE_SINGLETON 매크로와 외부에서의 생성을 막기 위한 private 생성자
