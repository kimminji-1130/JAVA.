# JAVA
---------
## StringBuilder
#### String객체와 String객체를 더하는 행위는 메모리 할당과 메모리 해제를 발생시켜, 성능(시간초과)이 좋지 않기 때문에 사용하는 문법(String 과 문자열 더할 때 사용)
<사용 예시>
```
StringBuilder sb = new StringBuilder();
sb.append("더할 문자열");
System.out.println(sb.toString());
```
-----------
## 정렬해주는 문법
### Array.sort (오름차순)
### Collections.sort(내림차순)
-----------
## rrayList.add()
#### ArrayList의 add() 메소드는 인자로 전달된 객체를 리스트에 추가하는 역할
<사용 방법>
''' 
  ArrayList<String>  fruits = new ArrayList<String> ();
  fruits.add("apple");
  System.out.println(fruits.toString());
  '''
