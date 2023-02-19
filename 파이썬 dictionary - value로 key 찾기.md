딕셔너리에서 value를 이용해 key를 찾는 방법은 쉽게 두 가지가 있다.<br>
1. 반복문을 사용하는 방법
```python
[k for k,v in dic.item()]
```
이 경우 매번 딕셔너리 전체를 순회하면서 값을 가져오기 때문에 비효율적이다.<br><br>

2. {key,value}를 뒤집는 방식
다른 방법으로는 {key,value}를 뒤집어 {value,key}로 저장해놓고 쓰는 방법이 있다.
```python
get_key={v:k for k,v in dic.items()}
```
이 경우 1의 방법보다 저장 공간을 크게 사용한다는 단점과 value에 중복이 있는 경우 1개만 저장된다는 단점이 있어서 주의해서 사용해야 한다.
<br><br><br>
[참고](https://blog.naver.com/wideeyed/222007663089)
