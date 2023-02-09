[11725:트리의 부모 찾기](https://www.acmicpc.net/problem/11725) 문제를 풀다 런타임 에러(RecursionError)가 발생했다.<br>
파이썬에서는 재귀의 한도가 시스템의 안정을 위해 정해져있기 때문에 발생하는 에러이다. <br>
해결 방법은 의외로 간단하다. 재귀 한도를 늘려주면 된다. <br>
그 방법은 아래와 같다.
<br>

```python
import sys
sys.setrecursionlimit(10**6)
```
