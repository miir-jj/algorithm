# BOJ 1793번 [타일링](https://www.acmicpc.net/problem/1793)

## 🌈 풀이 후기
- 개근상 문제를 풀고나서 푼 문제라 아이디어를 생각하는 것은 어렵지 않았습니다.
- 하지만 엄청 큰 수에 대한 표현에서 막혀 블로그 도움을 받았습니다..
- BigInteger에 대해 처음 알게 되었습니다.

## 👩‍🏫 문제 풀이
- n번째에 타일을 채울 수 있는 경우의 수는 
  - n-1번째 경우에 2x1 타일을 세로로 하나 채우는 경우
  - n-2번째 경우에 2x1 타일을 가로로 두개, 2x1타일을 세로로 두개(위위 경우와 겹침), 2x2타일을 하나 채우는 경우
- dp[n]=dp[n-1]+dp[n-2]*2
- biginteger 연산은 일반연산이 안되므로 함수 이용