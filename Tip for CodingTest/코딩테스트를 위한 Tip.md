# 코딩테스트를 위한 팁

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