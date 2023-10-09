# Process Writeup

## Name: Wilson Huang
## Course: APSCA
## Period: 7
## Concept: Objects

### Introduction
In APCSA (Advanced Placement Computer Science A), we are learning about Java. Learning Java is somewhat similar to Javascript; so learning Java has so far been easier due to my background knowledge in JavaScript. But I have faced challenges throughout my learning experience. For the past 2 weeks we have been learning about unit 2 (objects) in a website called ProjecStem. Learning unit 2 has been challenging for me and was much harder than unit 1 (primitives). After learning unit 2 we had to do an assignment to test our knowledge about unit 2 and an exam. In the text below I will explain some of my challenges when learning about objects.

### Challenge 1
One challenge I had is understanding what `.compareTo` does. I thought that when it compares to a word it would either put -1, 0, or 1. Negative one would mean that it is not the same and zero would mean the same. I later learned that I was incorrect it compares the letters if the first string had a higher letter than the second it will input how big the letter is than the other, vise versa if the letter is smaller. It is hard to explain but I will show you.
```java
String a = "java";
String b = "guava";
System.out.println(a.compareTo(b)); // This would output 3 because a is bigger than b by 3 letters

String a = "java";
String b = "guava";
System.out.println(b.compareTo(a)); // If ot was switched it would output -3 because b is smaller than a by 3 letters
```

### Challenge 2
After finishing unit 2 we had an assignment that would use all of the components in unit 2. In that assignment we would be simulating an Air Traffic Control tower. This program uses data of the Airplane class type. I was stuck on doing the math for the intial height distance between two airplanes. I foregot to use `Math.abs` to round the number; I instead used `(int)`. This is wrong because it wont round corectly.
#### Incorrect
``` java
System.out.println("The difference in height between Airplane 2 and Airplane 3 is " + (int)(two.getAlt()-three.getAlt())+ " feet.");
```
#### Correct
```java
System.out.println("The difference in height between Airplane 2 and Airplane 3 is " + (int)Math.abs(two.getAlt()-three.getAlt())+ " feet.");
```
### Challenge 3
After finishing the unit 2 and the assignment we had to take a unit 2 exam. I did bad on this exam because I didn't do enough to prepare myself. In this challenge I will show you one of the questions I had trouble with.
#### Question
``` java
int y = 15;
int x = 5;
System.out.println("Answer: " + (x + 10) + y);
```
In this question I thought that the answer would be 30 because I just did basic math to get the answer ((5+10)+15). This was not the case because "Answer: " is a string and 15 would go inside of it. So after (5+10) it would go inside the string "Answer: 15" then it would +15 inside the string so the output would be "Answer: 1515. However if the question was `System.out.println((x + 10) + y);`, it would equal to 30.
### Takeaways
* Always read the instructions in projectstem because in assignment 2 I was really confused in the beginning and I didn't know how to start but as I read the instructions it became a alot easier.
* You should experiment in the playground because when I got the question above wrong I was confused on what I did wrong so I went to a java playground to see the output and it made sense.
* I did bad in the exam but I learned how to better prepare for the next exam. I should do the pracrtices in AP classroom and not do everything last minute because it takes a while to sink it. Therefore it is important to manage my time. 
