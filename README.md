### tool usage error (line 126)

다음과 같이 고쳤다.
```
if not result 
=> if result is None or (isinsance(result, str) and str=="")
```
에러의 원인은 result가 str일 수도 있고 None일 수도 있기 때문이다.
result의 타입은 (None|str), 따라서 result가 빈문자열인지만 검사할 것이 아니라.
result가 None인지도 검사를 해야 한다.
