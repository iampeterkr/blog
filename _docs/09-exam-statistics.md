---
# layout : rchive
title: "Exam Statistics"
permalink: /exam-statistics/
excerpt: "We excercise EXAM STATISTICS by Exam Statistics ."
last_modified_at: 2019-01-17T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    
 <hr style="border: solid 1px #dddddd ;">

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 1. Let's look at those grades!    

Creating a program to compute statistics means that you won't have to whip out your calculator and manually crunch numbers. All you'll have to do is supply a new set of numbers and our program does all of the hard work.

This mini-project will give you some practice with functions, lists, and translating mathematical formulae into programming statements.

In order to use the scores in our program, we'll need them in a container, namely a list.

On the right, you'll see the **`grades`** listed (see what I did there). The data is anonymous to protect the privacy of the students.





**설명:**     
통계를 계산하는 프로그램을 만들어 보자. 즉 당신이 계산기를 두드리고, 수작업으로 수를 계산하고 하는 일을 할 필요가 없다. 당신은 숫자를 입력만 하면, 우리 프로그램이 모든것을 처리 할 것이다.    
미니 프로젝트를 통하여 우리는 함수, 리스트, 수학적 공식을 프로그램으로 변경하는것을 배우게 된다.    
우리 프로그램의 점수를 사용 하식 위해선, 우리는 리스트가 항목들이 필요합니다.    
Edit 창에서 학생들의 개인적인 점수들이 리스트에 있는것을 볼수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Hit Run to continue.


**설명:**     
① `Run`을 기동하세요.  
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
grades = [100, 100, 90, 40, 80, 100, 85, 70, 90, 65, 90, 85, 50.5]
print "Grades:", grades
```

**설명:**     
리스트 `grades`에 있는 항목들을 출력한다. 
{: .notice--info}


**결과** 
``` 
Grades: [100, 100, 90, 40, 80, 100, 85, 70, 90, 65, 90, 85, 50.5]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 2. Print those grades    

As a refresher, let's start off by writing a function to print out the list of grades, one element at a time. 



**설명:**     
복습 겸, 등급 리스트를 출력해주는 함수를 만들어 보자. 한번에 한 항목 하나씩 출력된다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function on line 3 called **`print_grades`** with one argument, a list called **`grades_input`**.

* Inside the function, iterate through **`grades_input`** and print each item on its own line.

* After your function, call **`print_grades`** with the grades list as the parameter.




**설명:**     
① 함수 `print_grades(grades_input)`를 만들어 보자.   
• `grade_input`을 반복적으로 돌면서 항목을 하나씩 추출하여 출력한다.     
•  `print_grade(grade)`로 호출 합니다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Need help with your for loop?
```python
numbers = [2, 3, 5, 8, 13]

for n in numbers:
  print n
```

**설명:**     
`for` 문을 활용하여 loop(반복) 한다. 
{: .notice--info}

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

**설명:**     
• `print_grades(grades)`를 호출하면, 해당 함수가 호출됩니다.   
• for 문을 반복하여 입력받은 리스트 `grades_input`을 하나씩 추출하여 변수 `grade` 에 저장합니다.    
• 변수 `grade`를 출력합니다. 
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
50.5
```

<br>
<br>    
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

 



**설명:**     
지금까지는, 다음 장에서 사용할 함수들을 만들었습니다. 또한 당신은 앞으로도 확실한 개념을 잡아갈 것입니다.     
다음 장에는 우리의 성적 통계를 평균값을 만드는것을 해 보도록 하겠습니다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Hit Run to continue.


**설명:**     
① `Run`을 실행하세요. 
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
print "Let's compute some stats!"
```

**설명:** 
{: .notice--info}



**결과** 
``` 
Let's compute some stats!
```

<br>
<br>    
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





**설명:**     
우리는 성적을 출력해주는 함수와, 시험 성적의 전체 합을 계산해주는 함수를 만든다    
이 두함수는 평균 점수를 계산할때 필요하며, 아주 유용하다.    
당신은 내재 함수인 `sum()`을 사용하면 간단할텐데 라고 생각할 것이다. 하지만, 그것은 너무 쉬운 방법이다.    
우리는 수동 으로 sum(합)을 계산하는 함수를 만든다.   
이 함수는 리스트를 읽으며 loop(반복)를 돈다. 그리고 각 점수들을 더하여 변수 `total` 에 저장한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** On line 3, define a function, **`grades_sum`**, that does the following:

* Takes in a list of scores, `scores`
* Computes the sum of the scores
* Returns the computed sum.
Call the newly created **`grades_sum`** function with the list of grades and print the result.




**설명:**     
① 함수 `grades_sum(scores)`를 만들어라.    
• 점수들이 들어 있는 리스트 `scores`를 가진다.   
• 점수들을 합하여라.     
• sum(합계)을 반환하라.   
함수 `grades_sum(grades)`를 호출하여 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
To compute a rolling sum, create a variable total that's initialized to zero. Then, as you loop through the list of grades, add the current grade to total.

Avoid using sum as a variable name as it has a special meaning in Python!


**설명:**     
합계를 반복적으로 돌리기 위해선, 변수 `total`를 0으로 초기화 해야 한다. 그런 다음 입력 받은 리스트를 하나씩 값을 읽으며 그 값을 변수 `total`에 저장해야 한다.    
단, 변수명을 지정할때, Python 예약어는 피해야 한다.  
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

**설명:**     
• 합계를 저장할 변수 `total`을 0으로 초기화 환다.    
• 입력받은 리스트 `scores`를 하나씩 읽어서 값을 추출한다.
• 추출한 값을 변수 `total`에 더한다.   
• for 반복문이 끝나면 변수 `total`값을 return(반환)한다.    
{: .notice--info}



**결과** 
``` 
1045.5
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 5. Computing the Average    

The average test grade can be found by **dividing** the sum of the grades by the total number of grades.

Luckily, we just created an awesome function, **`grades_sum`** to compute the sum.


**설명:**    
시험 점수의 평균을 구하기 위해선, 전체 점수를 과목별로 나누는 것이다. 우리는 앞에서 이미 `grade_sum()` 함수를 만들었다. 이장에서는 dividing(나누기)에 대하여 연습해 보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function, **`grades_average`**, below the **`grades_sum`** function that does the following:

* Has one argument, `grades_input`, a list
* Calls `grades_sum` with `grades_input`
* Computes the average of the grades by **dividing that sum by float(len(grades_input))**.
* Returns the **average**.
Call the newly created **`grades_average`** function with the list of grades and print the result.




**설명:**     
① 함수 `grades_average()`밑에 `grades_sum(grades_input)`함수를 만드시오.     
• 함수는 `grades_input` 입력값을 가진다.    
• `grades_sum(grades_input)`으로 함수를 호출한다.   
• 평균을 구하기 위하여 전체 합을 나눌때 `float(len(grades_input))`으로 나눈다.   
• `average`를 return(반환)한다.    
마지막에 `grades_average(grades)`을 호출하여 출력한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Your **`grades_average`** function should use the built-in Python **`len`** function and your **`grades_sum`** function to compute the average.

Remember that **integer division** in Python will always **result in an integer**. We convert **len(grades_input) is a float** so that the average is a float.


**설명:**     
`grades_average()`함수는 내재 함수인 `len()`을 사용하면 된다. 그리고, `grades_sum()`함수는 평균을 구하면 된다.    
정수로 나누면 정수가 반환되고, 실수로 나누면 실수가 반환된다. 우리는 실수로 나눌 것이다.
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

**설명:**     
• `grades_input`을 입력 받는다.    
•  함수 `grades_average(grades_input)`는 전체 성적의 합(`sum_of_grades`)을 구한다.    
• `float(len(grades_input))` 리스트의 갯수를 구하고 그 값은 float(실수) 로 변환한다.        
• `sum_of_grades`전체 합을 `float(len(grades_input))`으로 나눈다.       
• `average`계산된 평균값을 return(반환)한다.    
{: .notice--info}



**결과** 
``` 
1045.5
80.4230769231
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 6. Review    

Great work creating the capability to compute the average of the test grades.

We're going to use the average for computing the variance. The variance allows us to see how widespread the grades were from the average.



**설명:**     
지금껏 우리는 시험 점수의 평균을 계산하는 작업을 수행하였다.   
다음장에서 우리는 평균으로 부터 variance(분산)을 통하여 성적의 분포도를 볼 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Hit Run to continue.


**설명:**     
① `Run`을 실행 하여라.  
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
print "Time to conquer the variance!"
```

**설명:** 
skip
{: .notice--info}



**결과** 
``` 
Time to conquer the variance!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 7. The Variance    

Let's see how the grades varied against the average. This is called computing the variance.

A very large variance means that the students' grades were all over the place, while a small variance (relatively close to the average) means that the majority of the students had similar grades.


**설명:**    
성적들이 평균과 얼마나 떨어져 있는지를 살펴보자. 이것을 분산이라고 부른다.    
평균에서 많이 떨어져 있다는 것은 학생들의 점수가 다양하게 넓게 흩어져 있다는 의미이고, 반대인 경우는 학생들의 점수가 좁게 분포되어 있다는 의미이다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① On line 18, define a new function called **`grades_variance`** that accepts one argument, **`scores`**, a list.

* First, create a variable **`average`** and store the result of calling **`grades_average(scores)`**.
* Next, create another variable **`variance`** and set it to zero. We will use this as a rolling sum.
* for each score in scores: Compute its squared difference: `(average - score) ** 2` and add that to `variance`.
* Divide the total `variance` by the number of scores.
* Then, return that result.
Finally, after your function code, print `grades_variance(grades)`.



**설명:**    
① 함수 `grades_variance(scores)`를 만들어라.    
• 먼저, 변수 `average`를 만들고, `grades_average(scores)`를 호출하여 얻은 결과값을 저장하라.    
• 다음으로, 변수 `variance`를 만들고, 0으로 초기화 하라. 나중에 분산값들을 합을 구할때 사용할 것이다.       
• for 문에서 각각의 점수들을 추출하여 차이를 계산한다.`( average - score)**2`, 그리고 그 결과값을 `variance`에 저장한다.     
• 전체 `variance`를 점수들의 갯수(`len(grades)`) 로 나눈다      
• 그리고, 그 결과 값을 return(반환)한다.    
마지막으로 `grades_variance(grades)`를 호출하여 출력한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
return variance / len(grades)
```


**설명:**     
최종 점수 값들의 수만큼 나눠 줘야 한다. 
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

def grades_variance(scores):
    average = grades_average(scores)
    variance = 0
    for score in scores:
        variance += (average - score) ** 2
    return variance / len(scores)

print grades_variance(grades)
```

**설명:**     
• 변수 `average`에 `grades_average(scores)`호출하여 얻은 결과값을 저장한다.   
• 변수 `variance = 0` 0으로 초기화 한다.   
• for 문을 돌면서 입력값 리스트 `scores`의 항목 값들을 하나씩 추출한다.   
• `(average - score) ** 2` 변수 `average`과 `score`의 차이를 구하고, 그 결과값을 제곱근하여 값을 구한다.    
• 변수 `variance`에 `(average - score) ** 2`결고 값을 반복하여 저장한다.     
• 합해진 `variance`에 `len(scores)`를 나누어 산출된 그 결과 값을 return(반환)한다.    
함수 `grades_variance(grades)`를 호출하여 출력한다.
{: .notice--info}



**결과** 
``` 
334.071005917
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 8. 



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}



**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 9. 



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}



**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 10. 



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}



**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 11. 



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}



**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 12. 



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}



**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 13.



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 14. 



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

**결과** ``` ```

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```



<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 15.



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 16. 



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 17.



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 18.



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">EXAM STATISTICS</font> 
### 19.



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```


<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
