# BOJ 14719번 [빗물](https://www.acmicpc.net/problem/14719)

## 🌈 풀이 후기
골드 문제치고 비교적 수월하게 풀렸던 문제였던 것 같습니다!


## 👩‍🏫 문제 풀이
 처음에는 순서대로 높이를 비교하며 최댓값만 저장했었는데 양옆을 다 검사해줘야한다는 것을 깨닫고 처음부터 다시 작성했습니다.
 현재 위치를 제외한 양옆에서 각각 최댓값을 구해준 후 그 중 작은 값에서 현재 높이를 빼줍니다.
 처음에는 조건문을 복잡하게 작성했었으나 결국에는 결과에 더해줄 값이 0보다 커야 빗물이 저장된 것이므로 조건문을 수정했습니다.
 ```java
 tmp=(Math.min(h1,h2)-height[i]); //양 옆 높이 중 최솟값에서 현재 높이 빼줌
 if(tmp>0)	////빗물이 저장 될 경우
    result+=tmp;
```
