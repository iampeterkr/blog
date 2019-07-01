---
# layout : rchive
title: "Exam Statistics"
permalink: /exam-statistics/
excerpt: "We excercise EXAM STATISTICS by Exam Statistics ."
# last_modified_at: 2019-02-25T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    

<hr style="border: solid 1px #dddddd ;">    

LESSON    

Your students just took their first test. It's time to see how everyone did. Let's write a program to compute the mean, variance, and standard deviation of the test scores.    

**설명:** [ 학습방향 ]     
학생들의 시험 점수를 가지고, 평균, 분산 및 표준편차를 계산하는 연습을 해보자.
{: .notice--info}     
     


<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 1. Let's look at those grades!    

Creating a program to compute statistics means that you won't have to whip out your calculator and manually crunch numbers. All you'll have to do is supply a new set of numbers and our program does all of the hard work.

This mini-project will give you some practice with functions, lists, and translating mathematical formulae into programming statements.

In order to use the scores in our program, we'll need them in a container, namely a list.

On the right, you'll see the `grades` listed (see what I did there). The data is anonymous to protect the privacy of the students.





**설명:** [ Learn ]    
• Ch1. Let's look at those grades! 에서는 통계 프로그램을 학습한다.    
• 통계를 계산하는 프로그램을 만든다.     
• 이 프로그램을 사용하면, 계산기를 두드리거나, 수작업으로 계산하는 일은 없다.    
• 당신은 숫자를 입력만 하면, 이 프로그램이 모든것을 처리 할 것이다.    
• 미니 프로젝트를 통하여 우리는 함수, 리스트, 수학적 공식을 프로그램화 하는것을 배운다.    
• 이 프로그램을 통하여 점수를 계산하기 위해선, 리스트 항목들이 필요하다.    
• Editor 화면에서 학생들의 개인적인 점수들이 리스트에 있는것을 볼수 있다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    


* Hit Run to continue.


**설명:** [ Instruction ]          
• Run 클릭후, 기동하라.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ hint ]          
• skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
grades = [100, 100, 90, 40, 80, 100, 85, 70, 90, 65, 90, 85, 50.5]
print "Grades:", grades
```

**설명:** [ Solution ]          
• 리스트 grades 에 있는 항목 값들이 출력된다. 
{: .notice--info}


**결과** 
``` 
Grades: [100, 100, 90, 40, 80, 100, 85, 70, 90, 65, 90, 85, 50.5]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 2. Print those grades    

As a refresher, let's start off by writing a function to print out the list of grades, one element at a time. 



**설명:** [ Learn ]          
• Ch2. Print those grades 에서는 다음과 같은 작업을 학습한다.    
• 등급 리스트를 출력해주는 함수를 만든다.    
• 한번에 하나씩 한 항목만 출력된다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function on line 3 called `print_grades` with one argument, a list called `grades_input`.

* Inside the function, iterate through `grades_input` and print each item on its own line.

* After your function, call `print_grades` with the grades list as the parameter.




**설명:** [ Instruction ]          
• 함수 print_grades(grades_input) 를 작성한다.    
• 입력값 리스트 grade_input 을 반복적으로 돌면서 항목을 하나씩 추출하여 출력한다.     
• 함수 print_grade(grade) 를 출력한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>


* Need help with your for loop?     

```python

numbers = [2, 3, 5, 8, 13]
for n in numbers:
  print n

```    

**설명:** [ Hint ]          
• for 문을 활용하여 반복(loop)한다. 
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python

grades = [100, 100, 90, 40, 80, 100, 85, 70, 90, 65, 90, 85, 50.5]

def print_grades(grades_input):
  for grade in grades_input:
    print grade

print_grades(grades)

```

**설명:** [ Solution ]          
• 정의된 함수 print_grades(grades) 는 다음과 같이 동작한다.    
• 이 함수는 입력값 grades_input 을 받은후, 해당 입력값의 항목값을 출력한다.       
• for 문에서 입력값 리스트 grades_input 항목값을 추출하여, 변수 grade 에 저장한다.    
• 변수 grade 를 출력한다.
{: .notice--info}

**결과** 
``` 
100
100
90
```
<p style="page-break-before: always;"></p>
<br>
```
40
80
100
85
70
90
65
90
85
50.5
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 3. Review    

So far, you've created a helper function that will be used in the next sections.

You also have a solid handle on the concepts that we'll need to continue.

The next step in the creation of our grade statistics program involves computing the mean (average) of the grades.

Onwards.

 



**설명:** [ Learn ]          
• Ch3. Review 에서는 평균값을 만드는 함수를 학습한다.    
• 지금 까지는, 다음 장에서 사용할 함수들을 만들었다.     
• 그리고, 함수 및 통계 프로그램의 확실한 개념을 잡아갈 것이다.     
• 다음 장에는 우리의 성적 점수를 활용하여, 평균값을 만들어 본다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Hit Run to continue.


**설명:** [ Instruction ]          
• Run 을 클릭하여, 실행하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>

* skip


**설명:** [ Hint ]          
• skip 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print "Let's compute some stats!"
```

**설명:** [ Solution ]      
• *Let's compute some stats!* 이 출력된다.
{: .notice--info}



**결과** 
``` 
Let's compute some stats!
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 4. The sum of scores    

Now that we have a function to **print the grades**, let's create another function to compute the sum of all of the test grades.

This will be super-helpful when we need to compute the average score.

I know what you're thinking, "let's just use the built-in sum function!" The built-in function would work beautifully, but it would be too easy.

Computing the sum manually involves computing a rolling sum. As you loop through the list, add the current grade to a variable that keeps track of the total, let's call that variable total.





**설명:** [ Learn ]          
• Ch4. The sum of scores 에서는 성적 출력과 전체합을 계산하는 함수를 학습한다.    
• 이 두 함수는 평균 점수를 계산할때 필요하며, 아주 유용하다.    
• Python 함수 sum() 을 사용하면 간단하다.   
• 하지만, 우리는 수동 으로 sum(합)을 계산하는 함수를 만든다.   
• 이 함수는 리스트를 읽으며 loop(반복)를 돈다.    
• 그리고 각 점수들을 더하여 변수 total 에 저장한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On line 3, define a function, `grades_sum`, that does the following:

* Takes in a list of scores, `scores`
* Computes the sum of the scores
* Returns the computed sum.
* Call the newly created `grades_sum` function with the list of grades and print the result.

<p style="page-break-before: always;"></p>
<br>



**설명:** [ Learn ]          
• 함수 grades_sum(scores) 를 작성하라.    
• 이 함수는 입력값으로 리스트 scores 를 가진다.   
• 리스트의 점수들을 합하라.     
• sum(합계)을 반환하라.   
• 함수 grades_sum(grades) 를 호출후, 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* To compute a rolling sum, create a variable total that's initialized to zero. Then, as you loop through the list of grades, add the current grade to total.

* Avoid using sum as a variable name as it has a special meaning in Python!


**설명:** [ Hint ]          
• 변수 total 을 0 으로 초기화 한다.    
• 반복문에서 입력 받은 리스트의 값을 하나씩 추출하여 변수 total 에 저장한다.     
• 변수명을 지정할때, Python 예약어는 피해야 한다.   
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
grades = [100, 100, 90, 40, 80, 100, 85, 70, 90, 65, 90, 85, 50.5]

def grades_sum(scores):
  total = 0
  for score in scores: 
    total += score
  return total

print grades_sum(grades)
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• 정의된 함수 grades_sum(scores): 은 다음과 같이 동작한다.    
• 합계를 저장할 변수 total 을 0 으로 초기화 한다.    
• for 문에서 입력받은 리스트 scores 에서 하나씩 값을 추출한다.    
• 추출한 값을 변수 total 에 더한다.   
• for 반복문이 끝나면 변수 total 값을 반환(return)한다.    
{: .notice--info}



**결과** 
``` 
1045.5
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 5. Computing the Average    

The average test grade can be found by **dividing** the sum of the grades by the total number of grades.

Luckily, we just created an awesome function, `grades_sum` to compute the sum.


**설명:** [ Learn ]         
• Ch5. Computing the Average 에서는 평균을 계산하는 프로그램을 학습한다.     
• 시험 점수의 평균은, 전체 점수를 과목별로 나눈 것이다.    
• 우리는 앞에서 grade_sum() 함수를 이미 만들었다.    
• 이 장에서는 dividing(나누기) 사용법을 연습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function, `grades_average`, below the `grades_sum` function that does the following:    

* Has one argument, `grades_input`, a list     
* Calls `grades_sum` with `grades_input`    
* Computes the average of the grades by **dividing that sum by float(len(grades_input))**.    
* Returns the **average**.    
Call the newly created `grades_average` function with the list of grades and print the result.    




**설명:** [ Instruction ]          
• 함수 grades_sum() 다음에, 함수 grades_average(grades_input) 를 작성하라.     
• 함수는 입력값으로 grades_input 를 가진다.    
• 함수 grades_sum(grades_input) 를 호출한다.    
• 평균을 구하기 위하여 전체 합을 나눌때 float(len(grades_input)) 으로 나눈다.    
• 평균값 average 를 반환(return)한다.    
• 마지막으로, 함수 grades_average(grades) 를 호출 후 출력한다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Your `grades_average` function should use the built-in Python `len` function and your `grades_sum` function to compute the average.

* Remember that **integer division** in Python will always **result in an integer**. We convert **len(grades_input) is a float** so that the average is a float.


**설명:** [ Hint ]      
• 함수 grades_average() 는 함수 len() 을 사용한다.    
• 함수 grades_sum() 는 평균을 구한다.         
• 정수로 나누면 정수가 반환되고, 실수로 나누면 실수가 반환된다.     
• 우리는 실수로 나눌 것이다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
grades = [100, 100, 90, 40, 80, 100, 85, 70, 90, 65, 90, 85, 50.5]

def grades_sum(scores):
  total = 0
  for score in scores: 
    total += score
  return total

print grades_sum(grades)

def grades_average(grades_input):
  sum_of_grades = grades_sum(grades_input)
  average = sum_of_grades / float(len(grades_input))
  return average

print grades_average(grades)
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• 함수 grades_average(grades_input) 는 전체 성적의 합을 구한다.     
• 정의된 함수 grades_average(grades_input) 는 다음과 같이 동작한다.    
• 이 함수는 grades_input 을 입력 받는다.    
• 함수 grades_sum(grades_input) 를 호출한다.    
• 호출후 결과값을 변수 sum_of_grades 에 저장한다.    
• 변수 sum_of_grades 에 float(len(grades_input)) 으로 나눈다.    
• 나눈값을 변수 average 에 저장한다.     
• 계산된 평균값 average 를 반환(return)한다.
{: .notice--info}



**결과** 
``` 
1045.5
80.4230769231
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 6. Review    

Great work creating the capability to compute the average of the test grades.

We're going to use the average for computing the variance. The variance allows us to see how widespread the grades were from the average.



**설명:** [ Learn ]          
• Ch6. Review 에서는 현재까지 프로그램을 검토 학습한다.    
• 지금껏 우리는 시험 점수의 평균을 계산하는 작업을 수행하였다.    
• 다음장에서 성적의 분포도를 보기 위하여 평균을 이용한 분산(variance)을 학습한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Hit Run to continue.


**설명:** [ Instruction ]          
• Run 을 실행후 진행하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ Hint ]          
• skip
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print "Time to conquer the variance!"
```

**설명:** [ Solution ]      
• skip
{: .notice--info}



**결과** 
``` 
Time to conquer the variance!
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 7. The Variance    

Let's see how the grades varied against the average. This is called computing the variance.

A very large variance means that the students' grades were all over the place, while a small variance (relatively close to the average) means that the majority of the students had similar grades.


**설명:** [ Learn ]         
• Ch7. The Variance 에서는 분산 프로그램을 학습한다.     
• 성적들이 평균과 얼마나 떨어져 있는지를 살펴보자. 이것을 분산이라고 부른다.    
• 평균에서 많이 떨어져 있다는 것은 학생들의 점수가 다양하게 넓게 흩어져 있다는 의미이다.    
• 반대의 경우는 학생들의 점수가 좁게 분포되어 있다는 의미이다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On line 18, define a new function called `grades_variance` that accepts one argument, `scores`, a list.    

* First, create a variable `average` and store the result of calling `grades_average(scores)`.    
* Next, create another variable `variance` and set it to zero. We will use this as a rolling sum.    
* for each score in scores: Compute its squared difference: `(average - score) ** 2` and add that to `variance`.    
* Divide the total `variance` by the number of scores.    
* Then, return that result.    
* Finally, after your function code, print `grades_variance(grades)`.    

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]         
• 함수 grades_variance(scores) 를 작성하라.    
• 변수 average 를 생성하라.    
• 함수 grades_average(scores) 를 호출후 결과값을 변수 average 에 저장하라.    
• 변수 variance 를 생성하고 0 으로 초기화 하라.     
• 추후, 분산값을 구할때 사용할 것이다.       
• for 문에서 각각의 점수들을 추출하여 차이를 계산한다.    
• e.g. ( average - score ) ** 2     
• 결과값을 변수 variance 에 저장한다.     
• 전체 variance 를 점수들의 갯수(len(grades)) 로 나눈다      
• 그리고, 그 결과 값을 반환(return)한다.    
• 마지막으로 함수 grades_variance(grades) 를 호출후 출력한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
return variance / len(grades)
```


**설명:** [ Hint ]          
• 최종 점수 값들의 수만큼 나눠 줘야 한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
grades = [100, 100, 90, 40, 80, 100, 85, 70, 90, 65, 90, 85, 50.5]

def print_grades(grades_input):
  for grade in grades_input:
    print grade

```

<p style="page-break-before: always;"></p>
<br>

```python
def grades_sum(scores):
  total = 0
  for score in scores: 
    total += score
  return total
    
def grades_average(grades_input):
  sum_of_grades = grades_sum(grades_input)
  average = sum_of_grades / float(len(grades_input))
  return average

def grades_variance(scores):
    average = grades_average(scores)
    variance = 0
    for score in scores:
        variance += (average - score) ** 2
    return variance / len(scores)

print grades_variance(grades)
```

**설명:** [ Solution ]          
• 정의된 함수 grades_variance(scores): 는 다음과 같이 동작한다.    
• 변수 average 에 함수 grades_average(scores) 호출후 얻은 결과값을 저장한다.    
• 변수 variance 은 0 으로 초기화 한다.   
• for 문에서 입력값 리스트 scores 의 항목 값을 하나씩 추출후, 변수 score 에 저장한다.    
• 평균에서 점수를 뺀후, 제곱 한다.    
• e.g. (average - score) ** 2     
• 변수 variance 에 추가한다.    
• e.g. variance += (average - score) ** 2    
• for 문이 완료되면 변수 variance 에 len(scores) 를 나눈값을 반환(return)한다.    
• 함수 grades_variance(grades) 를 호출후 출력한다.
{: .notice--info}



**결과** 
``` 
334.071005917
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 8. Standard Deviation    

Great job computing the variance! The last statistic will be much simpler: standard deviation.

The standard deviation is the square root of the variance. You can calculate the square root by raising the number to the one-half power.



**설명:** [ Learn ]     
• Ch8. Standard Deviation 에서는 표준편차 프로그램을 학습한다.    
• 분산(variance)에 이어, 우리가 연습할 것은 표준편차(Deviation) 이다.    
• 표준편차는 분산을 square root(√, 양의 제곱근)한 것이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function, `grades_std_deviation`, that takes one argument called `variance`.    

* return the result of `variance ** 0.5`    

* After the function, create a new variable called `variance` and store the result of calling `grades_variance(grades)`.    

* Finally print the result of calling `grades_std_deviation(variance)`.    




**설명:** [ Instruction ]          
• 함수 grades_std_deviation(variance) 를 작성하라.    
• 함수는 variance ** 0.5 를 반환(return)한다.        
• 함수 밖에서 변수 variance 를 생성하라.    
• 함수 grades_variance(grades) 호출후 받은 결과값을 변수 variance 에 저장하라.    
• 함수 grades_std_deviation(variance) 를 호출후, 그 결과 값을 출력하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, raising a number to an exponent involves using the exponentiation `` operator.


**설명:** [ Hint ]     
• ( ** ) 연산자는 지수를 계산해주는 연산자 이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
grades = [100, 100, 90, 40, 80, 100, 85, 70, 90, 65, 90, 85, 50.5]

def print_grades(grades_input):
  for grade in grades_input:
    print grade

def grades_sum(scores):
  total = 0
  for score in scores: 
    total += score
  return total
    
def grades_average(grades_input):
  sum_of_grades = grades_sum(grades_input)
  average = sum_of_grades / float(len(grades_input))
  return average

def grades_variance(grades):
    variance = 0
    for number in grades:
        variance += (grades_average(grades) - number) ** 2
    return variance / len(grades)

```

<p style="page-break-before: always;"></p>
<br>

```python

def grades_std_deviation(variance):
  return variance ** 0.5

variance = grades_variance(grades)

print grades_std_deviation(variance)

```

**설명:** [ Solution ]     
• 정의된 함수 grades_std_deviation(variance) 는 다음과 같이 동작한다.    
• 입력값 variance 를 가진다.    
• 변수 variance ** 0.5 를 계산후 결과값을 반환(return)한다.    
• 분산을 계산하는 함수 grades_variance(grades) 을 호출한다.     
• 그 결과값을 외부 변수 variance 에 저장한다.    
• 함수 grades_std_deviation(variance) 를 호출한다.    
• 그 결과값 표준편차를 출력한다.
{: .notice--info}



**결과** 
``` 
18.2776094147
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 9. Review    

You've done a great job completing this program.

We've created quite a few meaningful functions. Namely, we've created helper functions to print a list of grades, compute the sum, average, variance, and standard deviation about a set of grades.

Let's wrap up by printing out all of the statistics.

Who needs to pay for grade calculation software when you can write your own? :)





**설명:** [ Learn ]    
• Ch9. Review 에서는 합, 평균, 분산, 표준편차 프로그램을 학습했다.     
• 이 장에서는 모든 통계값들을 출력해 보자.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Print out the following:

  * all of the grades
  * sum of grades
  * average grade
  * variance
  * standard deviation

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]    
• 아래 내용들을 출력하여라.    
• 모든 점수들    
• 점수의 합   
• 평균 점수   
• 분산 값    
• 표준편차 값
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You need to use all of the helper functions that you've created and print out their results.


**설명:** [ Hint ]      
• 지금껏 만든 함수를 호출한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
grades = [100, 100, 90, 40, 80, 100, 85, 70, 90, 65, 90, 85, 50.5]

def print_grades(grades_input):
  for grade in grades_input:
    print grade

def grades_sum(scores):
  total = 0
  for score in scores: 
    total += score
  return total

def grades_average(grades_input):
  sum_of_grades = grades_sum(grades_input)
  average = sum_of_grades / float(len(grades_input))
  return average
```
<p style="page-break-before: always;"></p>
<br>

```python

def grades_variance(grades):
    variance = 0
    for number in grades:
        variance += (grades_average(grades) - number) ** 2
    return variance / len(grades)

def grades_std_deviation(variance):
  return variance ** 0.5

variance = grades_variance(grades)

for grade in grades:
  print grade

print grades_sum(grades)
print grades_average(grades)
print grades_variance(grades)
print grades_std_deviation(variance)

```

**설명:** [ Solution ]     
• 각 점수를 for문을 통하여 출력한다.     
• e.g. for grade in grades:        
• 점수 합 : print grades_sum(grades)    
• 평균 점수 : print grades_average(grades)    
• 분산 값 : print grades_variance(grades)   
• 표준편차 값 : print grades_std_deviation(variance)
{: .notice--info}


**결과** 
``` 
100
100
90
40
80
100
85
70
90
65
90
85
```
<p style="page-break-before: always;"></p>
<br>

```

50.5
1045.5
80.4230769231
334.071005917
18.2776094147

```