# JAVA_TypeCasting  


## ✅ 형변환이란?  하나의 자료형을 다른 자료형으로 바꾸는 것  

int -> float, double
```
int score = 93;
System.out.println(score); //90
System.out.println((float) score); //93.0
System.out.println((double) score); //93.0
```

float, double -> int  
```
float score_f = 93.3F;
double score_d = 98.8;
System.out.println((int) score_f); //93
System.out.println((int) score_d); //98
```

정수 + 실수 연산
```
score = 93 + (int) 98.8; // 93 + 98
System.out.println(score); //191
```
98.8은 실수가 형변환으로 int가 되면서 소수점이 사라짐  
  
```
score_d = (double) 93 + 98.8; // 93.0 + 98.8
System.out.println(score_d); // 191.8
```
(double)93 생략 가능: 정수 + 실수 연산 시 정수가 자동으로 실수로 바뀜  



숫자 -> 문자열
```
String s1 = String.valueOf(93);
s1 = Integer.toString(93);
System.out.println(s1);
```
실수 -> 문자열
```
String s2 = String.valueOf(98.8);
s2 = Double.toString(98.8);
System.out.println(s2); //98.8
```
문자열 -> 숫자
```
int i = Integer.parseInt("93");
System.out.println(i); // 93
double d = Double.parseDouble("98.8");
System.out.println(d); //98.8
```
