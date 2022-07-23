---
layout: default
title: "HTTP 코드"
date: 2022-06-29
last_modified_date: 2022-06-29
---

# HTTP 코드

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

## HTTP 코드 순서도

HTTP 코드의 종류와 순서를 정리한 자료를 찾았는데 공부할 때 참고하기 좋을 것 같다.

<p>
  <strong>
    This infographic was created by <a href="https://www.loggly.com/blog/http-status-code-diagram/">Loggly</a>.
    아래의 순서도는 <a href="https://www.loggly.com/blog/http-status-code-diagram/">Loggly</a>가 제작한 자료입니다.
  </strong>
</p>
<p>
  <a href='https://www.loggly.com/blog/http-status-code-diagram/'>
    <img 
      src='https://www.loggly.com/wp-content/uploads/2015/06/http-decision-diagram.png' 
      alt='HTTP Status Code Diagram' 
      width='600px' 
      border='0'
    />
  </a>
</p>

## 401과 403

이 자료는 401과 403의 차이에 관해 얘기하다가 찾게 됐는데, 대화를 요약하면 결론은 이렇다.

| HTTP 코드 | 문제                                                                                    | 해결                                   |
| :-------- | :-------------------------------------------------------------------------------------- | :------------------------------------- |
| 401       | 당신이 누구인지 프로그램이 알지 못함 (unauthenticated)                                  | 계정을 확인하고 다시 시도해 보세요     |
| 403       | 프로그램은 당신이 누구인지 알지만, 당신에게 이 데이터를 가질 권한이 없음 (unauthorized) | 다시 시도하지 말고 관리자와 얘기하세요 |

나도 401과 403의 차이를 구체적으로는 잘 몰랐는데 이번 기회에 배우게 됐다. 실용적인 부분은

- 뭐가 문제인가
- 언제 다시 request 보내기를 시도해도 되는가

이 정도인 것 같다.
