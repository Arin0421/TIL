- bisect(arr,a)는 a가 arr에 들어갈 수 있는 가장 오른쪽 위치를 반환한다.<br>

```python
arr=[1,2,3,4,5]
a=3
print(bisect(arr,a))
```
결과로는 3이 출력된다.<br>
- 가능한 가장 왼쪽의 위치를 반환하려면 bisect_left(arr,a)를 사용하면 된다.
