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
## ArrayList.add()
#### ArrayList의 add() 메소드는 인자로 전달된 객체를 리스트에 추가하는 역할
<사용 방법>
```
  ArrayList<String>  fruits = new ArrayList<String> ();
  fruits.add("apple");
  System.out.println(fruits.toString());
```
------------
## for(Object : List)
#### List에서 차례대로 꺼내서 A에다 넣는 역할
------------
## append()메소드
#### 인수로 전달된 값을 문자열로 변환 후, 해당 문자열의 마지막에 추가해주는 역할
<사용 방법>
```
StringBuffer str = new StringBuffer("Java");
System.out.println(str.append("왕이 되고 싶어요!"));
System.out.println("append() 메소드 이후 문자열 : " + str);
```
// <출력> Java왕이 되고 싶어요 (\n) Java왕이 되고 싶어요
--------------
##문자열로 받아서 소문자들 대문자로 만들기
```
import java.io.*;

public class Hiru {
    public static void main(String[] args) throws IOException{

    	BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
		String a = br.readLine();
		a = a.toUpperCase(); 
		System.out.print(a);
    }
}
```
### BufferedReader를 활용하여, 배열을 입력하기
#### int[] a = new int[8];
#### a[i] = Integer.parseInt(st.nextToken());  //Int로 입력하는 경우

## 두 배열을 비교하여 값이 같은지 비교하는 함수
#### Arrays.equals(a, b)

## Math함수
### Math.min(a, b)
#### a와 b 사이의 값이 짧은 것을 출력
-------------------------------------
## boolean
#### true나 false로만 나타낼 수 있다.
#### ex) boolean chk = true;
---------
## 팰린드롬수
1. str.charAt(i) != str.charAt(str.length() -1  - i))
#### 입력받은 변수(str)의 첫번째 수와 변수의 길이 -1 -i를 하면 마지막수를 비교해서 boolean으로 비교하는 방법
-----------
## 입력 받는 문자들 길이순으로 배열
```
Arrays.sort(word, new Comparator<String>() {
            @Override
            public int compare(String o1, String o2) {
                if(o1.length() > o2.length()) return 1;
                else if(o1.length() == o2.length()) return 0;
                else return -1;
            }
        });
```
#### word라는 배열에 입력 받은 값들을 비교하여 순서대로 값 저장
---------------
## 길이가 같은 문자들을 사전 순으로 정렬하는 방법
```
for (int i = 0; i < n; i++) {
            int j;
            for (j = i+1; j < n; j++) {
                if(word[i].length() != word[j].length()) break;
            }
            Arrays.sort(word, i,j);
            i = j-1;
        }
```
-------------------
## 우선 순위 큐
#### 일반 큐는 들어간 순서대로 나오는 (일방통행)자료구조라면 우선 순위 큐는 들어간 순서에 상관없이 일정한 규칙에 따라 우선 순위를 선정하고, 우선순위가 가장 높은 데이터가 가장 먼저 나온다.
### add(); peek(); poll(); 등의 메소드 사용
#### Integer와 같은 숫자는 Collections.reversOrder()를 사용
#### ex) PriorityQueue<Integer> priorityQueue = new PriorityQueue<>();
--------------------
## ArrayList
'''
ArrayList<String> list=new ArrayList<>(); //ArraryList 생성
list.add("철수"); // 리스트에 "철수"추가
```
#### 변수명.remove(위치 or "문자");
