
# SoundBunker(팀명: BPM )
![image](https://github.com/KyoJin-Hwang/SoundBunker/assets/84490050/f8ba9ebf-971e-4e0f-8023-6492f39e011b)


## 1. 프로젝트명
* 움직임과 사물 감지를 통한 상황 맞춤 음악 스트리밍 서비스
* 서비스설명: 미디어파이프의 포즈랜드마크 모델을 통해 움직임을 분석하고 YOLOv5로 객체를 탐지하여 종합된 결과로 상황을 분석하여, 이에 맞는 음악을 자동으로 재생시켜 사용자의 홈라이프를 보조해주는 서비스입니다.

## 2. 주요기능
* 미디어파이프의 포즈랜드마크 모델을 통한 사용자 움직임 분석
* YOLOv5모델을 학습시켜 객체 탐지
* 카테고리모드의 아이콘을 통해 특정 카테고리에 맞는 음악 재생
* 노래분류용 DNN모델을 사용해 장르 및 분위기, 빠르기 등 세분화를 통한 음악 분류
* 스크린세이버

## 3. 개발환경
|구분|내용|
|------|---|
|사용언어|Java, HTML, CSS, JavaScript, Python|
|사용한 라이브러리| Bootstrap / Kakao Map /  jQuery / MyBatis etc...|
|개발도구|Spring Framework /  VisualStudioCode  / Jupyter etc...|
|서버환경|tomcat 9.0 , Flask |
|데이터베이스| MySQL / etc..|

## 4. 아키텍처(구조)
![서비스 아키텍처](서비스유스케이스.png)


## 5. 기능 흐름도
### 서비스 흐름도(유스케이스)
#### SW 유스케이스
![image](유스케이스.png)
#### 서비스 흐름도(웹 화면설계서)
![image](웹화면설계서.png)
#### ER 다이어그램
![image](ER다이어그램.png)

## 6 SW 동작 화면

### 메인페이지
![image](타이틀메인.png)

### 캠모드
![image](캠모드화면단.png)

### 카테고리모드
![image](카테고리모드화면단.png)

## 7 제작 일정
![image](일정.png)

## 8 트러블슈팅

### python에서 ajax로 결과값을 받아온 후 다른 JS 파일에 결과값 전송이슈
* 파이썬 플라스크 서버에서 모션인식 및 사물인식에서 나온 결과값을 Ajax로 받았지만
Ajax 를 사용했던 js 파일에서 다른 js 파일로 결과값을 보내는데 이슈가 생겼다. 
구글검색 및 책으로 이슈를 해결 할 수 있었다. 
그방법은 결과 값을 받은 ajax 안에 sessionStorage(localStorage).setItem('키', '값'));
을 사용하여 다른 js 파일에서 sessionStorage(localStorage).getItem('키', '값')); 으로 결과값을 받아올 수 있게 되었다.
 
* 문제2<br>


