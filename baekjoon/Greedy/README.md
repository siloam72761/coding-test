\# 📌 백준 1931 - 회의실 배정



\## 🔗 링크

\[문제 링크](https://www.acmicpc.net/problem/1931)



---



\## 📋 문제 설명

* 회의를 겹치지 않게 하면서 사용할 수 있는 회의의 최대 개수를 구하는 문제입니다.
* 회의는 시작 시간과 종료 시간이 주어진다.



---



\## 🧠 알고리즘 분류

* 그리디 알고리즘
* 매 순간마다 최적이라고 생각되는 것을 선택해 나가는 방식



---



\## ✅ 핵심 포인트 정리

* 핵심은 \*\*정렬 기준\*\*입니다.
* 'lambda x: (x\[1], x\[0])'을 이용해 1순위로 종료 시간으로 먼저 정렬한다.
* 2순위로 종료 시간이 같을 경우 시작 시간이 먼저 기준으로 정렬한다.



---





\## 🗒️ 배운 점 \& 느낀 점

* lambda를 활용해 정렬 기준을 다중으로 줄 수 있다는 점을 새로 알게 되었습니다.
* range 대신 enumerate를 사용하면 인덱스를 이용하지 않아 코드 가독성이 높아집니다.



---



\## ⏱️ 시간복잡도 분석

* 회의 탐색 = O(N)
* 정렬 = O(N log N)
* 정렬이 가장 오래 걸리므로 \*\*O(N log N)\*\* 입니다.
