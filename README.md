# Computer_Algorithm project_01
## Closest_pair_of_points
2차원 평면상에 n개의 점이 입력으로 주어질 때, 거리가 가장 가까운 한 쌍의 점을 찾는 문제
### Algorithm
___
 1. **S에 있는 점의 수가 3개 이하면 더이상 분할 x**
  
  
  -*2개일 경우 그대로 리턴*
  
  
  -*3개일 경우 최근접 점의 쌍을 리턴*
  
  
 2. **x좌표가 오름차순으로 정렬 된 배열 S를 같은 개수의 점을 갖는 왼쪽(Sl) 오른쪽(Sr)으로 분할한다.**
  
  
  -*점의 개수가 홀수 개일 경우 왼쪽(Sl)에 1개 더 많게 분할*
  
  
 3. **Sl과 Sr에 대해 재귀적으로 분할해 최근접 점의 쌍을 CPl과 CPr이라 놓는다.**
 
 
 -*CPl과 CPr의 더 짧은 거리를 d로 정의*
  
  
 4. **d를 이용해 분할전 S에 중간 영역(Sc)에 속하는 점들을 찾고, 이 중에서 최근접 점의 쌍을 CPc라 놓는다.**
  
  
  -*Sl의 최우단점의 x좌표-d 보다 크고 Sr의 최좌단점의 x좌표+d 보다 작은 점을 middlepoints 배열에 저장해 최근접 점의 쌍을 찾는다.*
  
  
 5. **CPl CPr CPc 중에서 가장 짧은 거리를 가진 쌍을 해를 리턴한다.**
 
 
 ####coding histories
 -1단계
 배열 S를 재귀적으로 분할해 Sl과 Sr로 분할
 
 2개의 점이 남았을때 그대로 리턴
 
 -2단계
 3개의 점이 남았을때 최근접 점의 쌍을 리턴
 
 
 Sl과 Sr을 이용해 Sc를 정의하고 배열(middle points)에 저장
 
 
 CPl과 CPr를 이용해 d를 구하고 CPc를 구함
 
 
 closest point를 해로 리턴
 
 
 -3단계
 배열 middle points를 오름 차순으로 정렬한 뒤 d를 이용해 계산 횟수를 줄임
 
 


 
 
 
