---
# layout : rchive
title: "Student becomes the teacher"
permalink: /student-becomes-teacher/
excerpt: "We learn about using the list, dictionary Syntax."
last_modified_at: 2018-12-31T09:00:00-04:00
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

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 1. Lesson Number One   

Welcome to this **"Challenge Course"**. Until now we've been leading you by the hand and working on some short and relatively easy projects. This is a challenge so be ready. We have faith in you!

We’re going to switch it up a bit and allow you to be the teacher of your own class. Make a gradebook for all of your students.
```python
animal = {
  "name": "Mr. Fluffles",
  "sounds": ["meow", "purr"]
}
print animal["name"]
```
The example above is just to remind you how to create a dictionary and then to access the item stored by the "name" key.

 



**설명:**     
이 장은 지금껏 배운 내용을 응용하는 장이다. 기존 배운 딕셔너리에 대한 개념 정리를 해보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create three dictionaries: `lloyd`, `alice`, and `tyler`.

* Give each dictionary the keys "name", "homework", "quizzes", and "tests".

* Have the "name" key be the name of the student (that is, lloyd's name should be "Lloyd") and the other keys should be an empty list (We'll fill in these lists soon!)




**설명:**    
**①** 딕셔너리 `lloyd`, `alice`, `tyler`를 만들어라.    
• 각각의 딕셔너리에 key 명을 "name", "homework", "quizzes", "tests"를 갖는다.    
• "name" key에는 학생들의 이름이 values로 매칭된다.(예, lloyd딕셔너리의 key "name"에는 "Lloyd"가 매칭된다. )    
• 그리고 다른 key "homework", "quizzes", "tests"는 values 값에 리스트로 비워 둔다.(나중에 채워 넣을 예정이다.)  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Note, "homework", "quizzes", "tests" should be an empty list    
key's name is not `name` but `"name"` 


**설명:**     
주의, "homework", "quizzes", "tests"는 빈 리스트 이다.     
key 이름은 `name`이 아니고, `"name"`으로 사용해야 한다.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


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

**설명:**     
각 사람의 이름으로 딕셔너리를 만든다.    
key 명으로 "name", "homework", "quizzes", "tests"로 정의한다.    
key "name" 에만, 이름을 쓴다. 
homework", "quizzes", "tests"는 빈 리스트 이다. 
{: .notice--info}


**결과** 
``` 
skip
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 2.  What's the Score?    

Great work!



**설명:**     
소스를 읽고 이해해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Now fill out your `lloyd` dictionary with the appropriate scores. To save you some time, we've filled out the rest for you.

Homework: 90.0, 97.0, 75.0, 92.0

Quizzes: 88.0, 40.0, 94.0

Test Scores: 75.0, 90.0

**Make sure to include the decimal points** so your grades are stored as floats! This will be important later.


**설명:**     
**①** 딕셔너리 `lloyd`에 아래의 "homework", "quizzes", "test" 값을 넣어라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
skip


**설명:**     
skip
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

**설명:**     
`lloyd` 딕셔너리의 "homework", "quizzes", "tests"에 각 값을 float 형식으로 넣었다. 
{: .notice--info}


**결과** 
``` 
skip
```

<br>
<br>    
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

 



**설명:**     
리스트를 어떻게 사용하는지 재 상기 해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Below your code, create a **list** called `students` that contains `lloyd`, `alice`, and `tyler`.


**설명:**     
**①** 리스트 `studetns`를 만들고, 그 리스트 값 으로 `lloyd`, `alice`, `tyler`를 넣어라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
skip


**설명:**     
skip
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

**설명:**     
각 딕서너리 `lloyd`, `alice`, `tyler`를 리스트 `studetns`의 값으로 만든다. 
{: .notice--info}



**결과** 
``` 
skip
```

<br>
<br>    
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





**설명:**     
딕셔너리를 어떻게 만드는지, 그리고 딕셔너리 특정 key의 values 값에 접근 하는지 알아 보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** for each student in your students list, print out that student's data, as follows:

* print the student's name
* print the student's homework
* print the student's quizzes
* print the student's tests


**설명:**     
**①** 리스트 `students`에 있는 각 학생들의 name, homework, quizzes, tests의 값을 출력하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Use the for loop with list `students`


**설명:**     
리스트 `students`를 for 문을 활용하여라. 
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

**설명:**     
리스트 `students`를 for 문을 활용하여 딕셔너리를 이름을 추출하고, 해당 딕셔너리 이름의 key값을 출력한다.  
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

<br>
<br>    
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

When you divide an **integer** by another **integer**, the result is always an **integer** (rounded down, if needed).
When you divide a **float** by an **integer**, the result is always a **float**.
To divide two **integers** and end up with a **float**, you must first use `float()` to convert one of the **integers** to a **float**.
 



**설명:**     
• python에서 정수를 정수로 나누면 정수가 반환된다.
• 실수를 정수로 나누면 실수가 반환된다.
• 실수를 실수로 나누면 실수가 반환된다.
• 정수를 실수 내재함수 `float()`를 사용하여 정수로 나누면 실수가 반환된다.
즉, 둘중 하나가 실수이면 반환값도 실수이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Write a function average that takes a list of numbers and returns the average.

* Define a function called `average` that has one argument, `numbers`.
* Inside that function, call the built-in `sum()` function with the numbers list as a parameter. Store the result in a variable called `total`.
* Like the example above, use `float()` to convert `total` and store the result in `total`.
* Divide total by the length of the `numbers` list. Use the built-in `len()` function to calculate that.
* Return that result.


**설명:**     
① 리스트 `studetns`의 값들을 가져와서, 평균값을 만들어 주고 반환하는 함수를 만들어라.    
• 평균값을 계산해주는 함수 `average(numbers)`를 만들어라.
• `average()`함수는 내부함수 `sum()`을 활용하여 변수 `total`에 결과 값을 저장하라.
• `float()`함수를 사용하여 `float(total)`과 같이 변경 후 저장하여라.
•  변수 `total`를 리스트의 수만큼 나누어라. 리스트의 수는 내장함수 `len()`를 사용하라.
• 평균값을 반환하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Don't use `list` as a parameter name because it is a special function in Python. Many people also say you shouldn't use `l` because it looks too much like a `1`.


**설명:**     
파라미터 변수로 `list`를 사용하지 못한다. `list`는 이미 특수 함수로 지정되어 있기 때문이다. 그리고 변수 `l`도 되도록 사용하지 말자. 숫자 `1`과 혼동되기 때문이다. 
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
  return total / len(numbers)
```

**설명:**     
새로운 함수 `average(numbers)`를 만들자. 
이 함수는 입력받은 argument `numbers`의 값을 내부함수 `sum(number)`으로 합한 값을 `total`변수에 저장한다. 변수 `total`을 `float(total)`로 변환하여 저장한다. 이후, 최종 `total/len(numbers)`를 반환한다.  
{: .notice--info}



**결과** 
``` 
skip
```

<br>
<br>    
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
Then, we calculate the average cost of apples and the average cost of bananas. Since we like apples much more than we like bananas, we weight the average cost of apples by **90%** and the average cost of bananas by **10%**.
The `\` character is a continuation character. The following line is considered a continuation of the current line.





**설명:**     
딕셔너리 `cost`의 과일을 평균값을 계산한 후, 최종 반환하기 전에 각 과일별 가중 평균값을 반환한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Write a function called `get_average` that takes a student dictionary **(like lloyd, alice, or tyler)** as input and returns his/her weighted average.

* Define a function called `get_average` that takes one argument called `student`.
* Make a variable homework that stores the average() of student["homework"].
* Repeat the above step for "quizzes" and "tests".
* Multiply the 3 averages by their weights and return the sum of those three. Homework is 10%, quizzes are 30% and tests are 60%.


**설명:**     
① `get_average`함수를 만들어라. 이함수는 리스트 `students`를 입력값으로 받고, 각자의 가중 평균값을 반환한다.     
• `get_average(student)`함수를 정의하자.     
• 입력값 `student`의 "homework" key 값의 평균값을 변수 `homework`에 저장하다.
• "quizzes", "tests" 도 동일하게 변수를 만들어 평균값을 저장한다. 
• 3개(homework, quizzes, test)를 합해서 반환할때, 각 homework : 10%, quizzes :  30%, tests :  60%를 가중치를 반영해서 반환하자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
you should make a variabel `homework`, `queezes`, `tests`, and `total`


**설명:**    
변수 `homework`, `queezes`, `tests`를 만들어서 각각 저장해야 한다. 이후 `total`변수를 활용해서 모두 더해야 한다. 
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
  return total / len(numbers)

def get_average(student):
  homework = average(student["homework"])
  quizzes = average(student["quizzes"])
  tests = average(student["tests"])
  
  total = homework *.1 + quizzes * .3 + tests * .6
  return total
```

**설명:**    
함수 `get_average()`에서, 각 학생의 `homework`, `quizzes`,`tests`의 평균을 계산하고, 총합을 구할때, 각 항목별 가중치를 곱한후, 최종 `total`을 반환한다.

{: .notice--info}



**결과** 
``` 
skip
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 7. Sending a Letter    

Great work!

Now let's write a `get_letter_grade` function that takes a `number score `as input and returns a string with the letter grade that that student should receive.





**설명:**     
함수 `get_letter_grade()`를 만들자. 점수를 입력 받으면 해당 등급을 학생에게 알려주는 서비스이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a new function called `get_letter_grade` that has one argument called `score`. Expect score to be a **number**.

* Inside your function, test score using a chain of `if: / elif: / else:` statements, like so:

* If score is **90** or above: return "A"
* Else if score is **80** or above: return "B"
* Else if score is **70** or above: return "C"
* Else if score is **60** or above: return "D"
* Otherwise: return "F"

Finally, test your function!

Print the resulting letter grade with print. Call the `get_letter_grade` function and pass in `get_average(lloyd)`.




**설명:**     
① `get_letter_grade(score)`를 만들어라.
  • 함수의 내부 기능은 점수에 따라 `if: / elfi: /else:`문을 사용한다.     
  • 90점 이상 "A"    
  • 80점 이상 "B"
  • 70점 이상 "C"
  • 60점 이상 "D"
  • 그외 "F"    

 점수를 입력하면, 해당 등급을 알려주는 함수 `get_letter_grade()`만들고, 호출 입력값으로 `get_average(lloyd)`를 넣어라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Your function will probably contain a bunch of elif statements to figure out what to do with each grade. It might look something like this:
```python
def get_letter_grade(score):
  if score >= 90:
    return "A"
  elif score >= 80:
    # ...and so on!
```    
Your final print statement should be:
```python
print get_letter_grade(get_average(lloyd))
```


**설명:**     
함수 `get_letter_grade(score)`를 만들고, 호출은 `print get_letter_grade(get_average(lloyd))` 로 한다. 
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

**설명:**     
함수 `get_letter_grade(get_average(lloyd))`로 호출한다. 
{: .notice--info}



**결과** 
``` 
B
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 8. Part of the Whole    

Good! Now let's calculate the class average.

You need to get the average for **each student** and then calculate the average of those averages.





**설명:**     
각 학생의 평균점과 전체 학생의 평균점을 계산하는 프로그램을 추가해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function called `get_class_average` that has one argument `class_list`. You can expect `class_list` to be a list containing your three students.

* First, make an empty list called `results`.

* For each student item in the `class_list`, calculate `get_average(student)` and then call `results.append()` with that result.

* Finally, return the result of calling `average()` with results.




**설명:**     
① 함수 `get_class_average()`를 정의하고, argument로 `class_list`를 받는다.    
  함수의 기능은 다음과 같다. 
• 리스트 `results`를 만들고 초기화 하라.    
• 리스트 `get_average(class_list)`에 `class_list`의 값에 student 이름이 들어 있기에, for 문을 사용하여 변수 `student_avg`에 각 학생 이름을 넣는다.     
• 그리고, `results.append(student_avg)` 하여 각 학생별 avg를 `results`에 저장한다.     
• 마지막으로, return 할때, `average(results)`하여 반환한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
use the variable `student_avg` in the 'for' state upon calculating each student average.


**설명:**     
for문을 사용하여 각 학생별 평균값을 사용할때, `student_avg`변수를 사용하라. 
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

def get_class_average(class_list):
  results = []
  for student in class_list:
    student_avg = get_average(student)
    results.append(student_avg)
  return average(results)

```

**설명:**     
`class_list`를 입력받아, 각 학생의 이름을 for 문을 통하여 뽑아낸다.    
학생별 `get_average(student)`를 계산한후, 해당 값을 리스트 results에 저장한다.
최종 return 할때, 해당 리스트의 평균값 `average(restults)`를 반환한다. 
{: .notice--info}



**결과** 
``` 
skip
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">STUDENTS BECOMES THE TEACHER</font> 
### 9. How is Everybody Doing?    

Awesome! You're doing great. Now let's use the functions you've created to check on the grade of the class overall.





**설명:**     
지금껏 개발한 내용을 점검해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a list called `students` and fill it with the three students, alice, lloyd, and tyler.

**②** Find the average grade of the class. Print this numerical grade to the terminal.

**③** Finally, determine the letter grade for the class's average and print it to the terminal. 

**설명:**     
① 리스트 `students`를 만들고 그 값으로 학생 `alice, lloy, tyler`를 넣자.    
② 변수 `avg`에 학생들의 평균값저장하고, `avg`를 출력해 보자. (`avg=get_class_average(student)`, `print(avg)`)    

③ 마지막으로 `get_letter_grade(avg)` 를 출력하자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

② print out the result of calling get_class_average with your students list.
③ Fprint the result of get_letter_grade for the class's average.

**설명:**     
② `get_class_average(students)`를 호출하여, 변수 `avg`에 저장하자. print 문으로 avg를 출력하자. 
③ `get_letter_grade(avg)`를 호출하여 그 결과 값을 출력하자.   
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

**설명:**     
`get_class_average`에 학생들 이름 리스트가 입력되고, 학생 전체의 평균값을 계산한다.    
`get_class_average`에서 학생 전체의 평균값 등급이 출력된다.  
{: .notice--info}



**결과** 
``` 
83.8666666667
B
```

<br>    