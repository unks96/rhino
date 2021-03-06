# Visualization 담당 : 서경덕, 정권상

Our goal is to make a interactive plot dashboard using shinydashboard in R.

-Reference
1) interactive maps 관련 자료
leaflet + shiny

https://medium.com/@joyplumeri/how-to-make-interactive-maps-in-r-shiny-brief-tutorial-c2e1ef0447da <br>
https://hansenjohnson.org/post/interactive-maps-in-r/ <br>
https://geocompr.robinlovelace.net/adv-map.html <br>
https://kuduz.tistory.com/1196 <br>
https://m.blog.naver.com/PostView.nhn?blogId=hsj2864&logNo=220909725602&targetKeyword=&targetRecommendationCode=1 - 한글자료 <br>
http://blog.naver.com/PostView.nhn?blogId=hsj2864&logNo=221004882027 - 레이아웃조정 <br>
https://rstudio.github.io/shinydashboard/structure.html - layout 설정에 대한 코드(infobox등 여러가지 box를 넣는 법} <br>
https://stackoverflow.com/questions/50245925/tabitem-cannot-show-the-content-when-more-functions-in-menuitem-using-shiny-and - body의 menuitem menu별로 input type 조정하는법 <br>
https://github.com/rstudio/shinydashboard/issues/25 - select input을 tab에 넣었을 때 뜨는 에러 해결(시도결과 에러 해결 X) <br>
https://stackoverflow.com/questions/50245925/tabitem-cannot-show-the-content-when-more-functions-in-menuitem-using-shiny-and - several input types을 tab에 넣어을 때 근래 발생하는 문제 해결법 (찐문제해결) <br>
https://stackoverflow.com/questions/21465411/r-shiny-passing-reactive-to-selectinput-choices
(Tab 1개에 selectinput을 여러개 넣어서 reactive input을 받는 법) <br>
https://github.com/rstudio/shiny/issues/650 (플랏 사이즈 조정 -> body에 조정하고 server에도 조정해야함! 총 두번) <br>

2) Shiny dashboard 호스팅 방법

https://wikidocs.net/66610 -> ui, server R파일 따로 만들어서 시도하였으나 에러발생 <br>
http://blog.naver.com/PostView.nhn?blogId=hsj2864&logNo=220915578619&redirect=Dlog&widgetTypeCall=true <br>
https://m.blog.naver.com/PostView.nhn?blogId=hsj2864&logNo=220892395419&proxyReferer=https:%2F%2Fwww.google.com%2F <br>

# Timeline
## 2020.05.13
- 샤이니대시보드 자료조사 시작
 
## 2020.05.24
- 데이터캠프 샤이니 대시보드 코드 트레이닝
- Leaflet 활용 및 구별 단계구분도 표시
- 대시보드 프로토 타입 제작

## 2020.06.01 
 ### Visualization 팀 회의(대쉬보드 레이아웃 구조)
- Tab1) Data table1 -> 소수점 정리하기 -> Feature table
- Tab2) Feature별 barplot구하기 
- Tab3) Interactive map1 (색깔의 진하기로 값 표시) (권상이형) -> Sidebar에 feature 선택
- Tab4) Data table2 -> 수소차대수 table -> Check box(단일선택)로 updating
- Tab5) Interactive map2 -> 수소 충전소 입지 선정 -> Check box(단일선택)로 updating
 
필요사항 : 
Tab1) 소수점 정리
Tab2) 레이아웃(특히 사이즈)조정
Tab3) 레이아웃 조정
-> animation

## 2020.06.12~14 Visualization 팀 주요 변동 사항
- Tab5) 수소 충전소 입지 선정 구현 완료.(구, 동 2가지의 drop-down menu를 이용하여 업데이트)
- Tab4)와 Tab5) 통합 및 테이블과 지도를 박스에 넣어서 레이아웃을 새롭게 배치.

2020.06.16
select input 초기에 잠깐 미선택 오류발생 -> 어느정도 해결
------------------------------------------------------------------------------
# D.A.S.H B.O.A.R.D 완성 
<br>https://ysuks.shinyapps.io/dashboard/

<br>Tab1) 구별 특성 그래프(ggplotly)
<br>Tab2) 구별 특성 테이블(table)
<br>Tab3) 구별 특성 지도(leaflet)
<br>Tab4) 수소차 충전소 지도(leaflet)
