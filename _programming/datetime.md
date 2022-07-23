---
layout: default
title: "시간과 시간대"
date: 2022-01-28
last_modified_date: 2022-07-22
---

# 시간과 시간대

[The Problem with Time & Timezones - Computerphile][datetime-video]의 내용에 교차검증과 개인적인 감상을 붙인 글

[datetime-video]: https://youtu.be/-5wpm-gesOY

<iframe width="560" height="315" src="https://www.youtube.com/embed/-5wpm-gesOY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---

{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

---

## 각국의 timezone offset

시차의 최소단위가 1시간이 아닌 건 이미 알고 있었지만, [15분 단위로 차이가 나는 경우도 있다][list-of-utc-offsets]는 건 이번에 처음 알았다.

[list-of-utc-offsets]: https://en.wikipedia.org/wiki/List_of_UTC_offsets

- Australian Central Daylight Time (ACDT): UTC+10:30
- Australian Central Western Standard Time: UTC+08:45
- Nepal Standard Time (NPT): UTC+05:45

## Daylight savings time

영국은 daylight savings time의 시작이 1주 빠르다고 한다. 그런데 무엇보다 1주 빠르다는 건지 찾아보다가 알아낸 것:

- [2차 세계대전 당시 영국은 서머타임을 두 배로 만들었다.][whatever-happened-to-double-summer-time] 그래서 영국의 시간이 그리니치 표준시보다 2시간 빨라졌었는데, 정작 그리니치 표준시의 기준이 되는 그리니치 천문대는 영국에 있다.
- 영국은 서머타임을 daylight savings time이 아니라 [British Summer Time][gov-uk-when-do-the-clocks-change]이라 부른다.
  - 서머타임 적용 중일 때: British Summer Time (BST)
  - 서머타임이 아닐 때: Greenwich Mean Time (GMT)
- 위키피디아에는 [daylight saving time by country 항목][daylight_saving_time_by_country]이 따로 있는데 문서의 길이가 상당하다.
- 남반구는 북반구와 계절이 반대니까 daylight savings time을 계산할 때 한 시간을 더할지 뺄지를 북반구와 반대로 계산해야 한다.

[gov-uk-when-do-the-clocks-change]: https://www.gov.uk/when-do-the-clocks-change
[daylight_saving_time_by_country]: https://en.wikipedia.org/wiki/Daylight_saving_time_by_country
[whatever-happened-to-double-summer-time]: https://www.theguardian.com/commentisfree/2006/jun/24/comment.mainsection2

## 날짜변경선을 변경하는 경우

날짜변경선을 바꾸며 날짜를 하루씩 건너뛰는 일도 있다. 예를 들어 [Samoa와 Tokelau는 2011년에 날짜를 하루 건너뛰었다.][samoa-tokelau-article] 12월 29일에서 31일로 이어졌다고.

[samoa-tokelau-article]: https://www.bbc.com/news/world-asia-16351377

국가들이 시간을 바꾸는 일이 내가 생각했던 것보다 더 많이 있었던 모양인데 나오는 예시들이 흥미롭다. Samoa와 Tokelau의 경우에는 호주 & 뉴질랜드와의 교류와 사업을 편리하게 하려고 내린 결정이었다고 한다.

## 같은 지리적 위치 != 같은 시간대

[이스라엘과 팔레스타인의 경우][palestinians-to-observe-two-different-local-times]처럼 한 지역에서 다른 시간대를 사용하기도 한다. 지리적으로 같은 위치에 있더라도 정치적 문제로 다른 시간대를 쓸 수 있다고 한다.

[palestinians-to-observe-two-different-local-times]: https://www.timeanddate.com/news/time/gaza-dst-2011.html

## 율리우스력과 그레고리력

18세기부터 지금까지의 시간을 계산하려면 역법이 율리우스력에서 그레고리력으로 바뀐 걸 고려해야 한다.

- 율리우스력의 1년: 365.25일
- 그레고리력의 1년: 365.2425일

그런데 [스웨덴이 그레고리력을 _점차적으로_ 도입했다는 댓글][youtube-sweden-calendar-comment]이 있어서 [찾아보니까 스웨덴은 정말로][sweden-article]

- 1700년 3월 1일부터 1712년 2월 30일까지 그레고리력도 율리우스력도 아닌 달력을 썼고
- 1712년 3월 1일부터 1753년까지는 율리우스력을 사용했다.

[youtube-sweden-calendar-comment]: https://www.youtube.com/watch?v=-5wpm-gesOY&lc=Ugj3g0tOMpeutHgCoAEC
[sweden-article]: https://articles.adsabs.harvard.edu//full/1920PA.....28...18L/0000025.000.html

그리고 러시아는 무려 [20세기에 들어서야 그레고리력을 도입했다고 한다.][soviet-calendar]

[soviet-calendar]: https://en.wikipedia.org/wiki/Soviet_calendar

## 한 해의 시작 != 1월 1일

[율리우스력은 16세기까지 1년의 시작일이 다양했다고 한다.][older-julian-calendar-new-years-day]

[older-julian-calendar-new-years-day]: https://en.wikipedia.org/wiki/New_Year%27s_Day#New_Year's_Day_in_the_older_Julian_calendar

- 3월 1일: 구 로마
- 3월 25일: 기독교의 주님 탄생 예고 대축일
- 8월 29일: 이집트의 알렉산드리아력
- 9월 23일: 아우구스투스 황제의 생일
- 9월 1일: 비잔틴
- 12월 25일: 중세 기독교 유럽

그러니까 예를 들면 이렇게 계산하는 것이다.

- 924년 3월 24일의 다음 날 == 925년 3월 25일
- 924년 12월 31일의 다음 날 == 924년 1월 1일

## 윤초

[윤초란 천문 시각과 맞추기 위해 더해진 1초다.][leap-seconds-faqs] 1분에 61초가 있을 수 있다는 뜻이다.

[leap-seconds-faqs]: https://www.nist.gov/pml/time-and-frequency-division/leap-seconds-faqs

그런데 프로그래머에게 익숙한 시간 표기법인 [Unix time][unix-time-wikipedia]는 윤초를 포함하지 않는다. 이 때문에 unix time은 정말로 정밀한 UTC 표기법은 아니라고 한다.

[unix-time-wikipedia]: https://en.wikipedia.org/wiki/Unix_time

실제 시각을 초 단위로 맞추는 것보다는 사건들이 일어난 순서대로 배열되도록 하는 게 더 중요할 때도 있는데, 이런 경우에는 구글에서 공개한 [Leap Smear][leap-smear]와 같은 방법을 사용할 수 있다.

[leap-smear]: https://developers.google.com/time/smear

## 마치며

결론: 이 무시무시한 문제를 나보다 먼저 해결한 사람들에게 감사하며 기존의 라이브러리를 가져다 쓰기

직접 만들지 않는 게 답이긴 한 거 같은데 ㅋㅋㅋ 으악 이걸 언제 다 만들어 기존의 라이브러리 개발자분들께 감사합니다 하고 큰절을 올려야 할 거 같지

재미있었다… 가져다 쓸 수 있는 기존 라이브러리 만세 🙌 끝!
