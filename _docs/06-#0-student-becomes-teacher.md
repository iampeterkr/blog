---
# layout : rchive
title: "Student becomes the teacher"
permalink: /student-becomes-teacher/
excerpt: "We learn about using the list, dictionary Syntax."
# last_modified_at: 2019-02-15T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---



<hr style="border: solid 1px #dddddd ;">    

LESSON    

Use what you've learned so far to manage your own class.    

**설명:** [ 학습방향 ]     
지금까지 배운 것을 반복 연습하여, 자신의 것으로 완전히 만들자.
{: .notice--info}     
     
     
    
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 1. Lesson Number One   

Welcome to this "Challenge Course". Until now we've been leading you by the hand and working on some short and relatively easy projects. This is a challenge so be ready. We have faith in you!

We’re going to switch it up a bit and allow you to be the teacher of your own class. Make a gradebook for all of your students.    

```python
animal = {
  "name": "Mr. Fluffles",
  "sounds": ["meow", "purr"]
}
print animal["name"]
```    

The example above is just to remind you how to create a dictionary and then to access the item stored by the "name" key.




**설명:** [ Learn ]      
• Ch13. Let's Check Out! 에서는 딕셔너리 개념을 정리한다.    
• 이 장은 딕셔너리를 생성하고, ky / value 를 읽고, 변경, 삭제 하는것을 학습한다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create three dictionaries: `lloyd`, `alice`, and `tyler`.

* Give each dictionary the keys "name", "homework", "quizzes", and "tests".

* Have the "name" key be the name of the student (that is, lloyd's name should be "Lloyd") and the other keys should be an empty list (We'll fill in these lists soon!)




**설명:** [ Instruction ]         
• 딕셔너리 lloyd, alice, tyler 를 생성하라.    
• 각 딕셔너리의 key 값으로 "name", "homework", "quizzes", "tests" 를 갖는다.    
• key "name" 에는 학생들의 이름이 values 로 매칭된다.    
• e.g. lloyd = {"name" : "Lloyd"}     
• 다른 key "homework", "quizzes", "tests" 의 values 는 리스트로 비워 둔다.    
• 추후에 채워 나갈 예정이다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Note, "homework", "quizzes", "tests" should be an empty list    
* key's name is not `name` but `"name"` 


**설명:** [ Hint ]          
• 주의) "homework", "quizzes", "tests" 는 빈 리스트 이다.     
• key 값은 name 이 아니고, 문자열 "name" 으로 만들어야 한다.    
• 그냥 name 은 변수이다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>

```python
lloyd = {
  "name" : "Lloyd",
  "homework" : [],
  "quizzes" : [],
  "tests" : []
}

alice = {
  "name" : "Alice",
  "homework" : [],
  "quizzes" : [],
  "tests" : []
}

tyler = {
  "name" : "Tyler",
  "homework" : [],
  "quizzes" : [],
  "tests" : []
}
```

**설명:** [ Solution ]          
• 각 사람의 이름으로 딕셔너리를 만들었다.     
• e.g. lloyd, alice, tyler    
• key 로 "name", "homework", "quizzes", "tests" 로 정의 하였다.     
• key 값 "name" 에만, 문자열 이름(e.g. "Lloyd", "Alice", "Tyler")을 쓴다.    
• key 값 "homework", "quizzes", "tests" 는 빈 리스트(e.g. [] ) 이다. 
{: .notice--info}


**결과** 
``` 
#skip
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 2.  What's the Score?    

Great work!



**설명:** [ Learn ]          
• Ch2.  What's the Score? 에서는 딕셔너리의 빈 value 에 값을 넣어보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Now fill out your `lloyd` dictionary with the appropriate scores. To save you some time, we've filled out the rest for you.

  * Homework: 90.0, 97.0, 75.0, 92.0

  * Quizzes: 88.0, 40.0, 94.0

  * Test Scores: 75.0, 90.0

* Make sure to include the decimal points so your grades are stored as floats! This will be important later.


**설명:** [ Instruction ]          
• 딕셔너리 lloyd 의 key "homework", "quizzes", "test" 아래 값을 넣어라.    
• 입력값을 넣을때, float 값으로 넣어라.
{: .notice--info}    

**아래:**    
• Homework: 90.0, 97.0, 75.0, 92.0    
• Quizzes: 88.0, 40.0, 94.0    
• Test Scores: 75.0, 90.0
{: .notice--info}    


<p style="page-break-before: always;"></p>
<br>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ Hint ]          
• skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
lloyd = {
  "name": "Lloyd",
  "homework": [90.0, 97.0, 75.0 ,92.0],
  "quizzes": [88.0, 40.0, 94.0],
  "tests": [75.0, 90.0]
}
alice = {
  "name": "Alice",
  "homework": [100.0, 92.0, 98.0, 100.0],
  "quizzes": [82.0, 83.0, 91.0],
  "tests": [89.0, 97.0]
}
tyler = {
  "name": "Tyler",
  "homework": [0.0, 87.0, 75.0, 22.0],
  "quizzes": [0.0, 75.0, 78.0],
  "tests": [100.0, 100.0]
}
```

**설명:** [ Solution ]          
• 딕셔너리 lloyd 의 key 인 "homework", "quizzes", "tests" 의 value 에 float 형식으로 값을 대입했다. 
{: .notice--info}


**결과** 
``` 
#skip
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 3. Put It Together    

Now lets put the three dictionaries in a list together.    

```python
my_list = [1, 2, 3]
```    

The above example is just a reminder on how to create a list. Afterwards, my_list contains 1, 2, and 3.

 



**설명:** [ Learn ]     
• Ch3. Put It Together 에서는 리스트에 항목값으로 딕셔너리를 넣는것을 학습한다.    
• 복습으로 리스트를 어떻게 만들고, 사용했는지를 다시 연습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Below your code, create a list called `students` that contains `lloyd`, `alice`, and `tyler`.


**설명:** [ Instruction ]          
• 리스트 studetns 를 만들어라.    
• 리스트 students 는 딕셔너리 이름이 lloyd, alice, tyler 를 항목으로 가진다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip
<p style="page-break-before: always;"></p>
<br>


**설명:** [ Hint ]          
• skip
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
lloyd = {
  "name": "Lloyd",
  "homework": [],
  "quizzes": [],
  "tests": []
}
alice = {
  "name": "Alice",
  "homework": [100.0, 92.0, 98.0, 100.0],
  "quizzes": [82.0, 83.0, 91.0],
  "tests": [89.0, 97.0]
}
tyler = {
  "name": "Tyler",
  "homework": [0.0, 87.0, 75.0, 22.0],
  "quizzes": [0.0, 75.0, 78.0],
  "tests": [100.0, 100.0]
}

students = [lloyd, alice, tyler]
```

**설명:** [ Solution ]          
• 리스트 students 의 항목으로 lloyd, alice, tyler 를 가진다.
{: .notice--info}



**결과** 
``` 
#skip
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 4. For the Record    

Excellent. Now you need a hard copy document with all of your students' grades.    

```python
animal_sounds = {
  "cat": ["meow", "purr"],
  "dog": ["woof", "bark"],
  "fox": [],
}
print animal_sounds["cat"]
```    

The example above is just to remind you how to create a dictionary and then to access the item stored by the "cat" key.



**설명:** [ Learn ]     
• Ch4. For the Record 에서는 딕셔너리의 특정 key / value 에 접근하는 방법을 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* for each student in your `students` list, print out that student's data, as follows:

* print the student's `name`
* print the student's `homework`
* print the student's `quizzes`
* print the student's `tests`


**설명:** [ Instruction ]          
• 리스트 students 의 각 학생들 name, homework, quizzes, tests 의 값을 출력하라.  
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the for loop with list `students`


**설명:** [ Hint ]          
• 리스트 students 를 for 문을 사용하여 각 key / value 값을 추출하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
lloyd = {
  "name": "Lloyd",
  "homework": [],
  "quizzes": [],
  "tests": []
}
alice = {
  "name": "Alice",
  "homework": [100.0, 92.0, 98.0, 100.0],
  "quizzes": [82.0, 83.0, 91.0],
  "tests": [89.0, 97.0]
}
tyler = {
  "name": "Tyler",
  "homework": [0.0, 87.0, 75.0, 22.0],
  "quizzes": [0.0, 75.0, 78.0],
  "tests": [100.0, 100.0]
}

students = [lloyd, alice, tyler]
for student in students:
  print student["name"]
  print student["homework"]
  print student["quizzes"]
  print student["tests"]
```

**설명:** [ Solution ]          
• 리스트 students 의 항목값은 각 딕셔너리 이름이다.     
• for 문을 사용하여 리스트 students 의 항목값 딕셔너리 이름을 하나씩 추출한다.    
• 해당 딕셔너리 이름의 key 값 "name" 을 지정하여 읽어서 출력한다.    
• 해당 딕셔너리 이름의 key 값 "homework" 을 지정하여 읽어서 출력한다.    
• 해당 딕셔너리 이름의 key 값 "quizzes" 을 지정하여 읽어서 출력한다.    
• 해당 딕셔너리 이름의 key 값 "test" 을 지정하여 읽어서 출력한다.    
• for 문에서 리스트 students 의 다음 딕셔너리 이름 하나를 추출한다.     
• 리스트 이름 3개가 다 출력될 때까지 반복하며, 출력한다.
{: .notice--info}



**결과** 
``` 
Lloyd
[]
[]
[]
Alice
[100.0, 92.0, 98.0, 100.0]
[82.0, 83.0, 91.0]
[89.0, 97.0]
Tyler
[0.0, 87.0, 75.0, 22.0]
[0.0, 75.0, 78.0]
[100.0, 100.0]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 5. It's Okay to be Average    

When teaching a class, it's important to take the students' averages in order to assign grades.

```python
5 / 2
# 2

5.0 / 2
# 2.5

float(5) / 2
# 2.5
```
The above example is a reminder of how division works in Python.

When you divide an integer by another integer, the result is always an integer (rounded down, if needed).
When you divide a float by an integer, the result is always a float.
To divide two integers and end up with a float, you must first use `float()` to convert one of the integers to a float.
 



**설명:** [ Learn ]          
• Ch5. It's Okay to be Average 에서는 float, integer 계산법을 학습한다.    
• python에서 정수를 정수로 나누면 정수가 반환된다.    
• 실수를 정수로 나누면 실수가 반환된다.    
• 실수를 실수로 나누면 실수가 반환된다.    
• 정수를 실수로 변환해주는 내장함수 float() 를 사용하여 정수로 나누면 실수가 반환된다.    
• 둘 중 하나가 실수이면 반환값도 실수이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    
<p style="page-break-before: always;"></p>
<br>

* Write a function average that takes a list of `numbers` and returns the `average`.

* Define a function called `average` that has one argument, `numbers`.
* Inside that function, call the built-in `sum()` function with the numbers list as a parameter. Store the result in a variable called `total`.
* Like the example above, use `float()` to convert `total` and store the result in `total`.
* Divide total by the length of the `numbers` list. Use the built-in `len()` function to calculate that.
* Return that result.


**설명:** [ Instruction ]          
• 리스트 studetns 의 값들을 가져와서, 평균값을 만들어 주고 반환하는 함수를 작성하라.     
• 평균값을 계산해주는 함수 average(numbers) 를 만들어라.    
• 함수 average(), 함수 sum() 을 사용하여 변수 total 에 결과 값을 저장하라.    
• 함수 float() 를 사용하여 예제(e.g. float(total) )와 같이 변경 후 저장하라.    
• 변수 total 을 리스트의 갯수만큼 나누어라.    
• 리스트의 갯수는 내장함수 len() 를 사용하라.    
• 평균값 average 을 반환하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Don't use `list` as a parameter name because it is a special function in Python. Many people also say you shouldn't use `l` because it looks too much like a `1`.


**설명:** [ Hint ]          
• list 는 Parameter 변수명으로 사용하지 못한다.    
• list 는 Python 에서 이미 특수 함수로 지정되어 있기 때문이다.    
• 변수 l 도 되도록 사용하지 말자. 숫자 1 과 혼동되기 때문이다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    
<p style="page-break-before: always;"></p>
<br>


```python
lloyd = {
  "name": "Lloyd",
  "homework": [90.0, 97.0, 75.0, 92.0],
  "quizzes": [88.0, 40.0, 94.0],
  "tests": [75.0, 90.0]
}
alice = {
  "name": "Alice",
  "homework": [100.0, 92.0, 98.0, 100.0],
  "quizzes": [82.0, 83.0, 91.0],
  "tests": [89.0, 97.0]
}
tyler = {
  "name": "Tyler",
  "homework": [0.0, 87.0, 75.0, 22.0],
  "quizzes": [0.0, 75.0, 78.0],
  "tests": [100.0, 100.0]
}

# Add your function below!
def average(numbers):
  total = sum(numbers)
  total = float(total)
  return total / len(numbers)
```

**설명:** [ Solution ]          
• 새로운 함수 average(numbers) 를 만들었다.    
• 이 함수는 입력값을 numbers 로 받았다.    
• 입력값 numbers 를 함수 sum(number) 으로 합을 구하였다.   
• 변수 total 변수에 sum(number) 값을 저장한다.    
• 변수 total 을 함수 float(total)를 사용하여 실수로 변환한다.    
• 실수로 변환한 값을 다시 변수 total 에 저장한다.     
• 변수 numbers 의 갯수를 내부함수 len(numbers) 를 사용하여 길이를 계산한다.    
• 평균값을 구하기 위하여 최종 total 값에 변수 numbers 갯수를 나눈다.    
• 그 결과값을 반환(return)한다.
{: .notice--info}



**결과** 
``` 
#skip
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 6. Just Weight and See    

Great! Now we need to compute a student’s average using weighted averages.
```python
cost = {
    "apples": [3.5, 2.4, 2.3],
    "bananas": [1.2, 1.8],
}

return 0.9 * average(cost["apples"]) + \
       0.1 * average(cost["bananas"])
```

In the above example, we create a dictionary called `cost` that contains the costs of some fruit.
Then, we calculate the average cost of apples and the average cost of bananas. Since we like apples much more than we like bananas, we weight the average cost of apples by 90% and the average cost of bananas by 10%.
The `\` character is a continuation character. The following line is considered a continuation of the current line.





**설명:** [ Learn ]    
• Ch6. Just Weight and See 에서는 함수에서 함수를 호출하는 방법을 학습한다.    
• 딕셔너리 cost 의 *apples* 와 *bananas* 의 평균값을 계산한다.    
• 최종 값을 반환하기 전에 *apples* 와 *bananas* 의 가중 평균값을 곱한 후 반환한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write a function called `get_average` that takes a student dictionary (like lloyd, alice, or tyler) as input and returns his/her weighted average.

* Define a function called `get_average` that takes one argument called `student`.
<p style="page-break-before: always;"></p>
<br>

* Make a variable homework that stores the average() of student["homework"].
* Repeat the above step for "quizzes" and "tests".
* Multiply the 3 averages by their weights and return the sum of those three. Homework is 10%, quizzes are 30% and tests are 60%.

<br>

**설명:** [ Instruction ]          
• 함수 get_average(students) 를 만들어라.     
• 이 함수는 students 를 입력값으을 받는다.          
• 이 함수는 입력 받은 학생별 개별 평균값을 반환한다.     
• 변수 homework 에 학생별 key 가 "homework" 인것의 평균값을 계산하여 저장한다.    
• 변수 quizzes  에 학생별 key 가 "quizzes" 인것의 평균값을 계산하여 저장한다.    
• 변수 tests    에 학생별 key 가 "test" 인것의 평균값을 계산하여 저장한다.    
• homework 에 10% 가중치를 반영한다.    
• quizzes 에 30% 가중치를 반영한다.     
• tests 에 60% 가중치를 반영한다.     
• 변수 homework + quizzes + tests 의 합한 값을 반환한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* you should make a variabel `homework`, `queezes`, `tests`, and `total`


**설명:** [ Hint ]         
• 변수 homework, queezes, tests 를 만들어서 각각 저장해야 한다.     
• 변수 total 에 (homework + queezes + tests ) 더한 값을 저장한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>

```python
lloyd = {
  "name": "Lloyd",
  "homework": [90.0, 97.0, 75.0, 92.0],
  "quizzes": [88.0, 40.0, 94.0],
  "tests": [75.0, 90.0]
}
alice = {
  "name": "Alice",
  "homework": [100.0, 92.0, 98.0, 100.0],
  "quizzes": [82.0, 83.0, 91.0],
  "tests": [89.0, 97.0]
}
tyler = {
  "name": "Tyler",
  "homework": [0.0, 87.0, 75.0, 22.0],
  "quizzes": [0.0, 75.0, 78.0],
  "tests": [100.0, 100.0]
}

# Add your function below!
def average(numbers):
  total = sum(numbers)
  total = float(total)
  return total / len(numbers)

def get_average(student):
  homework = average(student["homework"])
  quizzes = average(student["quizzes"])
  tests = average(student["tests"])
  
  total = homework *.1 + quizzes * .3 + tests * .6
  return total
```

**설명:** [ Solution ]    
• 함수 get_average(student) 를 작성하였다.   
• 이 함수는 학생들의 "homework", "quizzes","tests" 의 평균값을 구한다.    
• 학생들의 평균값 "homework", "quizzes","tests" 에 가중치를 준다.    
• 변수 total 에 각 가중치 평균값(homework, quizzes, tests)을 저장한다.    
• 변수 total 을 반환(return)한다.
{: .notice--info}



**결과** 
``` 
#skip
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 7. Sending a Letter    

Great work!

Now let's write a `get_letter_grade` function that takes a `number score `as input and returns a string with the letter grade that that student should receive.





**설명:** [ Learn ]          
• Ch7. Sending a Letter 에서는 학생들의 등급을 알려주는 함수를 만들어 본다.    
• 함수 get_letter_grade() 를 만들어 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a new function called `get_letter_grade` that has one argument called `score`. Expect score to be a number.

* Inside your function, test score using a chain of `if: / elif: / else:` statements, like so:

  * If score is 90 or above: return "A"
  * Else if score is 80 or above: return "B"
  * Else if score is 70 or above: return "C"
  * Else if score is 60 or above: return "D"
  * Otherwise: return "F"

* Finally, test your function!

* Print the resulting letter grade with print. Call the `get_letter_grade` function and pass in `get_average(lloyd)`.    

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]          
• 함수 get_letter_grade(score) 를 만들어라. 입력값은 score 를 받는다.    
• 함수의 내부 기능은 점수에 따라  if / elif / else 문을 사용한다.     
• - 90점 이상 "A"    
• - 80점 이상 "B"    
• - 70점 이상 "C"    
• - 60점 이상 "D"    
• - 그 외 "F"    
• 점수를 입력하면, 해당 등급을 알려주는 함수 get_letter_grade() 만들어라.    
• 함수 get_letter_grade(get_average(lloyd)) 호출하라. 그리고 출력하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Your function will probably contain a bunch of elif statements to figure out what to do with each grade. It might look something like this:    

```python
def get_letter_grade(score):
  if score >= 90:
    return "A"
  elif score >= 80:
    # ...and so on!
```    

* Your final print statement should be:    

```python
print get_letter_grade(get_average(lloyd))
```


**설명:** [ Hint ]          
• 함수 get_letter_grade(score) 를 만들경우,     
• 호출 및 출력은 다음 예와 같이 한다.    
• e.g. print get_letter_grade(get_average(lloyd))
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>

```python
lloyd = {
  "name": "Lloyd",
  "homework": [90.0, 97.0, 75.0, 92.0],
  "quizzes": [88.0, 40.0, 94.0],
  "tests": [75.0, 90.0]
}
alice = {
  "name": "Alice",
  "homework": [100.0, 92.0, 98.0, 100.0],
  "quizzes": [82.0, 83.0, 91.0],
  "tests": [89.0, 97.0]
}
tyler = {
  "name": "Tyler",
  "homework": [0.0, 87.0, 75.0, 22.0],
  "quizzes": [0.0, 75.0, 78.0],
  "tests": [100.0, 100.0]
}

# Add your function below!
def average(numbers):
  total = sum(numbers)
  total = float(total)
  return total/len(numbers)

def get_average(student):
  homework = average(student["homework"])
  quizzes = average(student["quizzes"])
  tests = average(student["tests"])
  return 0.1 * homework + 0.3 * quizzes + 0.6 * tests

def get_letter_grade(score):
  if score >= 90:
    return "A"
  elif score >=80:
    return "B"
  elif score >=70:
    return "C"
  elif score >=60:
    return "D"
  else:
    return "F"
  
print get_letter_grade(get_average(lloyd))
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• get_average(lloyd) 가 호출되어, lloyd 의 평균값이 계산된다.    
• 계산된 평균값을 get_letter_grade() 의 입력값이 되어 호출된다.    
• 입력값은 lloyd 의 등급을 반환한다.    
• print get_letter_grade(get_average(lloyd)) 는 lloyd 의 등급을 출력한다.
{: .notice--info}



**결과** 
``` 
B
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 8. Part of the Whole    

Good! Now let's calculate the class average.

You need to get the average for each student and then calculate the average of those averages.    



**설명:** [ Learn ]          
• Ch8. Part of the Whole 에서는 리스트에 항목값을 추가 하는것을 학습한다.        
• 각 학생의 평균점과 전체 학생의 평균점을 계산하는 프로그램을 추가해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function called `get_class_average` that has one argument `class_list`. You can expect `class_list` to be a list containing your three students.

* First, make an empty list called `results`.

* For each student item in the `class_list`, calculate `get_average(student)` and then call `results.append()` with that result.

* Finally, return the result of calling `average()` with results.


**설명:** [ Instruction ]          
• 함수 get_class_average(class_list) 를 정의하고 작성하라.    
• 이 함수는 입력값으로 리스트 class_list 를 받는다.    
• 리스트 results 를 만들고 초기화 하라.    
• 리스트 class_list 에는 학생들의 이름이 들어 있다.    
• for 문을 사용하여, class_list 의 학생 이름을 추출하여 변수 student 에 넣는다.    
• 함수 get_average(student) 를 호출한다.    
• 그 결과값을 변수 student_avg 에 대입한다. (학생별 평균값)   
• 리스트 변수 results 에 변수 student_avg 값을 메소드 .append 를 사용하여 추가한다.    
• 함수 average(results) 를 호출하여 계산후 반환(return) 한다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* use the variable `student_avg` in the 'for' state upon calculating each student average.


**설명:** [ Hint ]          
• for 문을 사용하여 각 학생별 평균값을 추출할때, 변수 student_avg 를 사용하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
lloyd = {
  "name": "Lloyd",
  "homework": [90.0, 97.0, 75.0, 92.0],
  "quizzes": [88.0, 40.0, 94.0],
  "tests": [75.0, 90.0]
}
alice = {
  "name": "Alice",
  "homework": [100.0, 92.0, 98.0, 100.0],
  "quizzes": [82.0, 83.0, 91.0],
  "tests": [89.0, 97.0]
}
tyler = {
  "name": "Tyler",
  "homework": [0.0, 87.0, 75.0, 22.0],
  "quizzes": [0.0, 75.0, 78.0],
  "tests": [100.0, 100.0]
}
```
<p style="page-break-before: always;"></p>
<br>

```python
# Add your function below!
def average(numbers):
  total = sum(numbers)
  total = float(total)
  return total/len(numbers)

def get_average(student):
  homework = average(student["homework"])
  quizzes = average(student["quizzes"])
  tests = average(student["tests"])
  return 0.1 * homework + 0.3 * quizzes + 0.6 * tests

def get_class_average(class_list):
  results = []
  for student in class_list:
    student_avg = get_average(student)
    results.append(student_avg)
  return average(results)

```

**설명:** [ Solution ]          
• 함수 get_class_average(class_list) 는 다음과 같이 동작한다.    
• 입력값 리스트 class_list 를 가진다.    
• 리스트 class_list 는 학생들 이름이 들어있다.    
• for 문을 사용하여 입력받은 리스트 class_list 의 학생이름을 추출한다.   
• 변수 student 에 추출한 이름을 저장한다.    
• 함수 get_average(student) 에 arguments 로 student 를 입력하여 호출한다.    
• 변수 student_avg 에 함수 get_average(studetn) 결과값(학생평균값)이 저장된다.    
• 리스트 results 에 학생별 평균값을 메소드 .append를 사용하여 추가한다.    
• 함수 average(results) 를 호출하여, 전체 학생의 평균값을 산출한다.    
• 그 전체 학생의 평균값을 반환(return) 한다.
{: .notice--info}



**결과** 
``` 
#skip
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 9. How is Everybody Doing?    

Awesome! You're doing great. Now let's use the functions you've created to check on the grade of the class overall.





**설명:** [ Learn ]          
• ch9. How is Everybody Doing? 에서는 지금까지 개발한 내용을 점검한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a list called `students` and fill it with the three students, alice, lloyd, and tyler.

* Find the average grade of the class. Print this numerical grade to the terminal.

* Finally, determine the letter grade for the class's average and print it to the terminal. 

**설명:** [ Instruction ]          
• 리스트 students 를 만들고 그 값으로 학생 alice, lloy, tyler 를 넣어라.    
• 전체 학생의 평균값을 산출한다. 그리고 출력한다.    
• 산출한 평균값의 등급을 계산한다. 그리고 출력한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* print the result of `get_letter_grade` for the class's average.

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]          
• 평균 점수의 등급은 함수 get_letter_grade의 결과로 산출된 값을 출력한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
lloyd = {
  "name": "Lloyd",
  "homework": [90.0, 97.0, 75.0, 92.0],
  "quizzes": [88.0, 40.0, 94.0],
  "tests": [75.0, 90.0]
}
alice = {
  "name": "Alice",
  "homework": [100.0, 92.0, 98.0, 100.0],
  "quizzes": [82.0, 83.0, 91.0],
  "tests": [89.0, 97.0]
}
tyler = {
  "name": "Tyler",
  "homework": [0.0, 87.0, 75.0, 22.0],
  "quizzes": [0.0, 75.0, 78.0],
  "tests": [100.0, 100.0]
}
    

# Add your function below!
def average(numbers):
  total = sum(numbers)
  total = float(total)
  return total/len(numbers)

def get_average(student):
  homework = average(student["homework"])
  quizzes = average(student["quizzes"])
  tests = average(student["tests"])
  return 0.1 * homework + 0.3 * quizzes + 0.6 * tests
```    
```python
def get_letter_grade(score):
  if score >= 90:
    return "A"
  elif score >=80:
    return "B"
  elif score >=70:
    return "C"
  elif score >=60:
    return "D"
  else:
    return "F"

def get_class_average(class_list):
  results = []
  for student in class_list:
    student_avg = get_average(student)
    results.append(student_avg)
  return average(results)

students = [lloyd, alice, tyler]

avg = get_class_average(students)
print(avg)
print(get_letter_grade(avg))
```


**설명:** [ Solution ]          
• 함수 get_class_average(students) 에 학생들 이름 리스트가 입력된다.    
• 함수 get_class_average() 는 학생 전체의 평균값을 계산한다.    
• 변수 avg 에 학생들 전체 평균값을 저장한다.     
• 변수 avg 를 출력한다.(학생 평균값 출력).     
• 함수 get_letter_grade(avg) 에 학생들 전체 평균값을 입력한다.    
• 학생 평균값의 등급을 계산한다.    
• 학생 평균값의 등급을 출력된다.
{: .notice--info}



**결과** 
``` 
83.8666666667
B
```
