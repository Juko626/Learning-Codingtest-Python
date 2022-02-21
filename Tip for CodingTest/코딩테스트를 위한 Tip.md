# 코딩테스트를 위한 팁

## 코딩테스트에 쓰이는 라이브러리나 알게 된 것 들을 추가하는 공간입니다.
<br>
<br>
<br>

### remove 와 discard의 차이점

- Remove()는 지워야 할 원소가 없으면  error 발생

```python
number={1,2,3,4,5,6}
number.remove(7)              #없는 7을 제거할 때

#에러 발생
```

```python
number={1,2,3,4,5,6}
number.discard(7)              #없는 7을 제거할 때

#에러 없이 종료
```

- Remove는 list 에서도 사용 가능 , discard 는 list 에서 사용 불가

```python
list_number=[1,2,3,4,5,6]
list_number.discard(x) #오류남, discard는 리스트에서 사용 불가
```

<br>
<br>
<br>

### 이진탐색에는 from bisect import bisect_right, bisect_left
```python
from bisect import bisect_right, bisect_left

bisect_left(a, x)
#정렬된 a에 x를 삽입할 위치를 리턴해준다. x가 a에 이미 있으면 기존 항목의 앞 (왼쪽)의 위치를 반환한다.

bisect_right(a, x)
#bisect_left와 거의 같은 함수인데, 이번에는 x가 a에 이미 있으면 기존 항목 뒤 (오른쪽)의 위치를 반환한다.
```

