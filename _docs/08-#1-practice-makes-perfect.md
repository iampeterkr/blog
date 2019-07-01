---
# layout : rchive
title: "Practice Makes Perfect"
permalink: /practice-makes-perfect/
excerpt: "We practice about loop."
# last_modified_at: 2019-01-15T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---



<hr style="border: solid 1px #dddddd ;">    

LESSON    

You know a lot of Python now. Let's do some practice problems!    

**설명:** [ 학습방향 ]     
Python 의 다양한 문제들을 연습하자.
{: .notice--info}     
     

    
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 1. Practice! Practice Practice!    

The best way to get good at anything is a lot of practice. This lesson is full of practice problems for you to work on. Each exercise will contain minimal instructions to help you solve these problems. The goal is to help you take your programming skills and apply them to real life problems.

The more challenging programs will contain some helpful hints to nudge you in the right direction.    



**설명:** [ Learn ]          
• Ch1. Practice! Practice Practice! 에서는 연습만이 살길이다.    
• 프로그램을 잘 짜는 방법은 오직 연습뿐이다.     
• loop를 배웠으니, 반복적으로 연습하면 프로그래밍 실력이 높아진다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Hit Run to continue.

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]          
• Run 을 클릭 후, 다음으로 넘어 가시오.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ Hint ]          
• skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
skip
```

**설명:** [ Solution ]          
• skip
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
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font>     

### 2. is_even    

All right! Let's get started.    

Remember how an even number is a number that is divisible by 2?    



**설명:** [ Learn ]          
• Ch2. is_even 에서는 모듈 연산자 % 를 학습한다.    
• 짝수는 2 로 나누어지는 것을 기억하고 있는가?     
• 2 로 나누어지는 숫자는 짝수이다.     
• 짝수인지를 어떻게 알수 있는지 모듈 연산자 % 를 학습한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function `is_even` that will take a number `x` as input.

* If `x` is even, then return **True**.

* Otherwise, return **False**.


**설명:** [ Learn ]          
• 함수 is_even(x) 을 작성하라.    
• 입력값 x 가 짝수이면 True를 반환하고, 홀수이면 False 를 반환한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>

* The modulo `%` operation is useful for determining if one number is divisible by another.

* Make sure to return True instead of printing it!


**설명:** [ Hint ]          
• 연산자 % 는 숫자를 나눈후 남는 나머지를 반환한다.     
• 나머지가 0 인것은, 나누어서 떨어진다는 의미이다.    
• 즉 2 로 나누어서 나머지가 0이면, 그것은 짝수이다.    
• 단, 0은 제외이다.    
• 함수를 만든후, 해당 함수를 호출하고 출력하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def is_even(x):
  if x % 2 == 0:
    return True
  else:
    return False
  
print is_even(5)
print is_even(6)
```

**설명:** [ Solution ]          
• 함수 is_even(x): 를 정의한다.    
• 이 함수는 parameter 로 X 를 가진다.    
• 이 함수는 연산자 %를 사용하여, 입력값 X 를 2로 나누어 나머지가 0 인지를 확인한다.    
• 이 함수는 나머지가 0 이면 True 를 반환한다.    
• 이 함수는 나머지가 0 이 아니면 False 를 반환한다.    
• 함수 is_even(5) 를 호출한다. 그리고 그 결과값을 출력한다.   
• 함수 is_even(6) 을 호출한다. 그리고 그 결과값을 출력한다.
{: .notice--info}


**결과** 
``` 
False
True
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 3. is_int    

An integer is just a number without a decimal part (for instance, -17, 0, and 42 are all integers, but 98.6 is not).    

For the purpose of this lesson, we'll also say that a number with a decimal part that is all 0s is also an integer, such as 7.0.    

This means that, for this lesson, you can't just test the input to see if it's of type int.    

If the difference between a number and that same number rounded is greater than zero, what does that say about that particular number?    

 



**설명:** [ Learn ]          
• Ch3. is_int 에서는 입력값이 정수인지를 확인하는 함수를 학습한다.    
• 정수(integer)는 소수점 값이 없는 10진수이다. (e.g. 98.6)    
• 소수점이 있지만, 이런 경우는 정수이다. (e.g. 7.0)    
• 프로그램에서 입력값이 정수인지를 어떻게 확인할 수 있을까?    
• 우리는 입력값을 다음과 같이 처리하면, 정수인지 아닌지를 알수 있다.    
• 입려값을 함수 abs()를 사용하여 절대값으로 변환한다.    
• 입력값을 함수 round()를 사용하여 소수점을 버린 값으로 변환한다.    
• 절대값에서 Round값을 뺀 결과가 0이면 정수이다. (절대값 - Round 값)    
• 절대값에서 Round값을 뺀 결과가 0이 아니면 실수이다. (절대값 - Round 값)
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function `is_int` that takes a number `x` as an input.

* Have it return True if the number is an **integer** (as defined above) and **False** otherwise.    

<p style="page-break-before: always;"></p>
<br>

* For example:    

```python
is_int(7.0)   # True    
is_int(7.5)   # False    
is_int(-1)    # True
```


**설명:** [ Instruction ]          
• 함수 is_int(x) 를 작성하라.   
• 이 함수는 입력값 x 가 정수(integer)이면 True를 반환하고, 아니면 False를 반환하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* To use the function `abs()`, `round()`


**설명:** [ Hint ]          
• 함수 abs() 는 절대값을 반환한다.   
• 함수 round() 는 소수점을 버린 정수만을 반환한다.    
• 이 두 함수를 활용하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def is_int(x):
  absolute = abs(x)
  rounded = round(absolute)
  return absolute - rounded == 0

print is_int(10)
print is_int(10.5)
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• 정의된 함수 is_int(x) 는 다음과 같이 동작한다.    
• 변수 absolute 에 입력값 x 의 절대값을 구하여 저장한다.    
• 변수 rounded 에 입력값 x 의 정수값만 구하여 저장한다.    
• 변수 absolute - rounded 한 결과를 반환한다.    
• 두 변수의 차가 0 이면, 정수이기에 True 가 자동으로 반환된다.    
• 두 변수의 차가 0 이 아니면 실수이기에 False 가 자동으로 반환된다.    
• 함수 is_int(10)을 호출하고, 그 결과값을 출력한다.    
• 함수 is_int(10.5)를 호출하고, 그 결과값을 출력한다.
{: .notice--info}



**결과** 
``` 
True
False
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 4. digit_sum    

Awesome! Now let's try something a little trickier. Try summing the digits of a number. 



**설명:** [ Learn ]          
• Ch4. digit_sum 에서는 각 자리의 수를 더하는 함수를 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write a function called `digit_sum` that takes a **positive integer `n` as input and returns the **sum of all** that number's digits. For example: digit_sum(1234) should return 10 which is 1 + 2 + 3 + 4. (Assume that the number you are given will always be positive.)

* Check the hint if you need help!


**설명:** [ Instruction ]          
• 함수 digit_sum(n) 을 작성하라.   
• 이 함수는 입력값 n 의 각 자리 수를 더하여 결과를 반환하는 함수이다.    
• e.g. digit_sum(1234) 의 반환값은 10이다.    
• 원리는 1 + 2 + 3 + 4 = 10 인 것이다.    
• 입력값은 항상 양수만 들어가야 한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>

* One way might be to convert the integer to a string with `str()`, iterate over it, and turn the substrings back into integers with `int()` to do the addition.    

* If you're looking for a challenge, try this: to get the rightmost digit of a number, you can modulo `(%)` the number by 10. To remove the rightmost digit you can floor divide (//) the number by 10. (Don't worry if you're not familiar with floor division—you can look up the documentation here. Remember, this is a challenge!)

* Try working this into a pattern to isolate all of the digits and add them to a total.    



**설명:** [ Hint ]          
• 함수 str() 를 사용하여 입력값을 문자열로 바꾼다.    
• for 문을 돌면서 각 값을 빼내어, 함수 int() 를 사용하여 변환한다.    
• 변환된 각 값을 합한다.    
• 다른 방법도 있다.    
• 연산자 % 를 사용하여 10으로 나누어 나머지 값을 더하면 되는 방법도 있다.    
• 연산자 % 와 비슷한 연산자 // 를 사용하는 방법도 있다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def digit_sum(n):
  total = 0
  string_n = str(n)
  for char in string_n:
    total += int(char)
  return total

#Alternate Solution:

#def digit_sum(n):
#  total = 0
#  while n > 0:
#    total += n % 10
#    n = n // 10
#  return total
  
print digit_sum(1234)
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• 입력값 n 을 문자열로 바꾼다. (e.g. str(n) )   
• for 문에서 문자열을 하나씩 뽑아내어, 변수 char 에 저장한다.    
• 함수 int(char) 을 사용하여, 변수 char 을 정수값으로 변환한다.         
• 변수 total 정수로 변환한 char 값을 더한다.    
• 변수 total 값을 반환한다.     
--------------------------------------     
• 다른 2 번째 방법은 다음과 같다.    
• 입력값 n 을  % 10 로 나눈 나머지를 변수 total 에 더한다.    
• 반복적으로 n 을 % 10 로 나눈 나머지를 더한다.     
--------------------------------------     
• 다른 3 번째 방법은 다음과 같다.    
• 입력값 n 을 연산자 ( n // 10 ) 를 계산하면 10 미만의 나머지가 계산된다.     
• 반복적으로 n 을 // 10 로 계산하면서 나머지를 더한다. 
{: .notice--info}



**결과** 
``` 
10
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font>     

### 5. factorial    

All right! Now we're cooking. Let's try a **factorial problem**.

To calculate the factorial of a non-negative integer **x**, just multiply all the integers from **1 through x**. For example:

factorial(4) would equal 4 * 3 * 2 * 1, which is 24.
factorial(1) would equal 1.
factorial(3) would equal 3 * 2 * 1, which is 6.    




**설명:** [ Learn ]      
• Ch5. factorial 에서는 수학의 factorial(계승) 함수를 학습한다.    
• 수학의 factorial(3) = 6 이다.    
• 계산하는 방법은 3 x 2 x 1 = 6 이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function `factorial` that takes an integer `x` as input.

* Calculate and return the factorial of that number.


**설명:** [ Instruction ]          
• 함수 factorial(x) 을 작성하라.    
• 함수 factorial(x) 는 입력한 값의 계산후 결과값을 반환한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>

* Consider having `factorial()` call itself. When the input is 1, your function could just return 1. Otherwise, it could return the number multiplied by `factorial(n - 1)`.

* Note that mathematically, factorial(0) is 1.


**설명:** [ Hint ]          
• 함수 facotorial(x) 는 입력값 n 이 1 이 될때까지 자신의 함수를 호출한다.    
• 최종적으로 입력값 x = 0 이 되어, factorial(0) 을 호출하면 최종값은 1을 반환한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def factorial(x):
    total = 1
    while x>0:
        total *= x
        x-=1
    return total
  
print factorial(5)

# def factorial2(n):
#     if n == 0:
#         return 1
#     else:
#         return n * factorial2(n-1)

# print factorial2(5)      
```

**설명:** [ Solution 1 ]          
• 정의된 함수 factorial(x) 에서는 입력값 x 를 가진다.    
• 변수 total = 1 로 초기화 한다.    
• while 문에서 입력값 ( x > 0 ) 동안 반복한다.    
• 변수 total 에 입력값 x 를 곱한후 더한다.    
• 입력값 x 의 값을 1씩 줄여준다.    
• while 문에서 입력값 (x > 0 ) 동안 반복한다.    
• while 문을 빠져나오면, 변수 total 값을 반환한다.     
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution 2 ]          
• 다른 방법은 다음과 같다.     
• 함수에서 함수를 재귀호출 하는 방법이다.     
• e.g. return  n * factorial2(n-1)     
• 자신의 함수를 다시 호출해서 사용하는 방법으로 나중에 배우게 될 것이다.
{: .notice--info}



**결과** 
``` 
120
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font>     

### 6. is_prime    

A prime number is a positive integer greater than 1 that has no positive divisors other than 1 and itself. (That's a mouthful!)

In other words, if you want to test if a number in a variable `x` is prime, then no other number should go into `x` evenly besides 1 and x. So 2 and 5 and 11 are all prime, but 4 and 18 and 21 are not.

If there is a number between 1 and x that goes in evenly, then x is not prime.





**설명:** [ Learn ]     
• Ch6. is_prime 에서는 prime(소수) 함수를 만드는 법을 학습한다.    
• Prime(소수)는 1 과 자신 이외에는 나눌수 없는 값을 말한다.    
• 입력값 x 를 입력해서 소수 인지를 확인하는 함수를 만들어 본다.    
• 1, 2, 3, 5, 7, 11 은 소수의 예이다.     
• 4는 2로 나누어지기에 소수가 아니다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function called `is_prime` that takes a number `x` as input.

* For each number n **from 2 to x - 1**, test if x is evenly divisible by **n**.

* If it is, return False.

* If none of them are, then return True.

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]          
• 함수 is_prime(x) 을 작성하라.    
• 이 함수는 1과 자신 x 이외에는 나누어 지지 않는다.    
• 입력값 x 를 2 부터 ( x - 1 ) 사이의 값중 하나로 나누어서 0이 나오면 소수가 아니다.    
• 소수가 아니면 False 를 반환한다.    
• 소수이면 True 를 반환한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember: all numbers less than 2 are not prime numbers!


**설명:** [ Hint ]          
• 2 보다 작은 모든 숫자는 소수가 아니다.
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def is_prime(x):
    if x < 2:
        return False
    else:
        for n in range(2, x-1):
            if x % n == 0:
                return False
        return True

print is_prime(13)
print is_prime(10)

```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• 정의된 함수 is_prime(x): 은 입력값 x 를 가진다.    
• 이 함수는 다음과 같이 동작한다.    
• 입력값 x 가 2 보다 작으면 소수가 아니므로 False 를 반환한다.    
• for 문에서 입력값 x 를 2 부터 ( x - 1 )까지 추출한다.    
• 변수 n 에 추출한 값을 저장한다.    
• 입력값 x 를 n 으로 모듈 연산자를 하여, 나머지가 0 이면 소수가 아니다.    
• 소수가 아니면 False 를 반환한다.    
• for 문이 정상 종료(x -1 까지 반복)되어 빠져 나오면, 이 값은 소수이다.    
• 소수이면 True 를 반환한다.    
• 함수 is_prime(13) 을 호출하고, 그 결과값을 출력한다.    
• 함수 is_prime(10) 을 호출하고, 그 결과값을 출력한다.
{: .notice--info}



**결과** 
``` 
True
False
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font>     

### 7. reverse    

Great work so far! Let's practice writing some functions that work with strings.



**설명:** [ Learn ]          
• Ch7. reverse 에서는 문자열을 조작하는 학습을 한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function called `reverse` that takes a string textand returns that string in reverse. For example: reverse("abcd") should return "dcba".

* You may not use reversed or [::-1] to help you with this.

* You may get a string containing special characters (for example, !, @, or #).


**설명:** [ Instruction ]          
• 함수 reverse() 를 작성한다.    
• 이 함수는 입력한 문자열을 반대로 출력하는 함수이다.    
• e.g. reverse("abcd") 를 입력하면 *dcba* 를 반환한다.   
• 물론 앞에서 배운 [::-1] , 함수 reversed() 을 사용해도 된다.    
• 이 장에서는 직접 함수를 만들어 본다. (특수 문자도 포함된다.)
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>

* Consider how you would loop through text starting from the last character through the first character.


**설명:** [ Hint ]          
• 입력받은 문자열의 마지막 부터 추출하여 리스트에 저장한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def reverse(text):
    word = ""
    l = len(text) - 1
    while l >= 0:
        word = word + text[l]
        l -= 1
    return word
  
print reverse("Hello World")
#print ''.join(reversed("abcd"))
#print ("Hello world")[::-1]

```

**설명:** [ Solution ]          
• 정의된 함수 reverse(text):는 다음과 같이 동작한다.    
• while 문에서 입력한 문자열의 길이 -1 만큰 반복한다.    
• e.g. text ="abcd" -> 변수 l = 3, 2, 1, 0 값이 된다.    
• text[l] 의 index 값으로 읽어서 변수 word 해당 문자를 저장한다.    
• 변수 l 을 -1 씩 차감한다.    
• 변수 word 를 반환한다. 
{: .notice--info}



**결과** 
``` 
dlroW olleH
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font>     

### 8. anti_vowel    

Nice work. Next up: vowels!



**설명:** [ Learn ]          
• Ch8. anti_vowel 에서는 모음을 찾아서 조작하는 방법을 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function called `anti_vowel` that takes one string, `text`, as input and returns the text with all of the **vowels removed**.

* For example: anti_vowel("Hey You!") should return "Hy Y!". Don't count Y as a vowel. Make sure to remove lowercase and uppercase vowels. 


**설명:** [ Instruction ]          
• 함수 anti_vowel(text) 을 작성하라.    
• 이 함수는 모음을 찾아서 없앤 문자열을 반환한다.     
• 예를 들면 anti_vowel("Hey You!") 를 호출하면, *Hy Y!* 를 반환한다.    
• 단, 대문자 Y 를 없애지 말라.    
• 그 외 대/소문자 모음 모두를 삭제하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* To check to see if `c` is a vowel, you can do: c in "aeiouAEIOU".

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]       
• 모음 모둠인 *aeiouAEIOU* 에 해당 문자가 속하는지를 점검한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def anti_vowel(text):
    result = ""
    vowels = "ieaouIEAOU"
    for char in text:
          if char not in vowels:
            result += char
    return result

print anti_vowel("hello book")
```

**설명:** [ Solution ]          
• 입력한 문자열을 한 글자씩 추출하여 *ieaouIEAOU* 에 속하는지를 점검한다.    
• 정의된 함수 anti_vowel(text): 다음과 같이 동작한다.      
• 입력된 값 변수 text 의 글자를 하나씩 추출한다.    
• 추출한 문자를 변수 char 에 저장한다.   
• 저장한 변수 char 의 문자가 모음값이 저장된 변수 vowels에 속하는지 확인한다.    
• 속하지 않는 변수 char 의 글자를 변수 result 에 저장한다.    
• 변수 result 값을 반환한다.
{: .notice--info}



**결과** 
``` 
hll bk
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font>     

### 9. scrabble_score    

Scrabble is a game where players get points by spelling words. Words are scored by adding together the point values of each individual letter (we'll leave out the double and triple letter and word scores for now).

To the right is a dictionary containing all of the letters in the alphabet with their corresponding Scrabble point values.

For example: the word "Helix" would score 15 points due to the sum of the letters: 4 + 1 + 1 + 1 + 8.

 



**설명:** [ Learn ]          
• Ch9. scrabble_score 에서는 딕셔너리를 활용하는 법을 학습한다.    
• Scrabble 게임은 각 알파벳에 각각 다른 점수를 매긴다.    
• 입력된 문자열의 각 단어의 알파벳 점수를 합한 값을 가지는 게임이다.    
• 앞에서 배운 딕셔너리 변수에 각 알파벳의 점수를 할당하여 각 단어별 점수를 매긴다.    
• 예를 들면, *Helix* 는 각 알파벳 점수는 H:4, e:1, l:1, i:1, x:8이다.    
• 이들 점수의 합은 15점이다.    
• Scrabble 게임을 통하여 딕셔너리 활용법을 배워보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function `scrabble_score` that takes a string `word` as input and returns the **equivalent scrabble score** for that word.

* Assume your input is only one word containing no spaces or punctuation.
* As mentioned, no need to worry about score multipliers!
* Your function should work even if the letters you get are uppercase, lowercase, or a mix.
* Assume that you're only given non-empty strings.

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]          
• 함수 scrabble_score(word) 를 작성하라.     
• 이 함수는 입력한 parameter 변수 word 의 점수를 반환한다.     
• 입력 단어는 공백이나, 구두점이 없어야 한다.     
• 점수 배열에 대해서는 걱정하지 마라.      
• 함수는 대문자, 소문자, 또는 대/소문자가 섞여 있어도 동작한다.     
• 입력은 반드시 있어야 한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Have your function loop through the word that you are given as input and look up the score for each letter in the score dictionary. Add the score for each letter into a total of some sort.

* Remember you can use a string's .lower() method to make your string lower case!




**설명:** [ Hint ]          
• 입력된 워드의 알파벳을 순차적으로 딕셔너리 score 에 있는 각 알파벳 점수와 비교한다.    
• 모든 입력된 문자는 함수 .lower() 를 사용하여 소문자로 만든다.    
• 소문자된 입력된 문자를 딕셔너리 score 서 찾는다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
score = {"a": 1, "c": 3, "b": 3, "e": 1, "d": 2, "g": 2, 
         "f": 4, "i": 1, "h": 4, "k": 5, "j": 8, "m": 3, 
         "l": 1, "o": 1, "n": 1, "q": 10, "p": 3, "s": 1, 
         "r": 1, "u": 1, "t": 1, "w": 4, "v": 4, "y": 4, 
         "x": 8, "z": 10}
         
```

<p style="page-break-before: always;"></p>
<br>

```python         
def scrabble_score(word):
  word = word.lower()
  total = 0
  for letter in word:
    for leter in score:
      if letter == leter:
        total = total + score[leter]
  return total

print scrabble_score("pizza")

# def scrabble_score(word):
#   totla = 0
#   for i in word:
#      w = i.lower()
#      r = score[w]
#      totla += r
#   return totla

# print scrabble_score("pizza")
```

**설명:** [ Solution ]         
• 정의된 함수 scrabble_score(word): 는 다음과 같이 동작한다.    
• 입력 문자열을 소문자로 만든다( e.g. word.lower() ).    
• 전체값을 저장할 변수 total 을 0 으로 초기화 한다.    
• 변수 word 의 문자를 하나씩 뽑아낸다.    
• 뽑아낸 문자를 딕셔너리 score 에서 반복적으로 찾는다.    
• 찾았으면 그 문자의 값을 딕셔너리 score 의 값을 찾는다(e.g. score[letter] ).    
• 변수 total 에 딕셔너리 score 에서 찾은 문자의 점수를 더한다.     
• 결과 total 값을 반환(return)한다.
{: .notice--info}




**결과** 
``` 
25
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font>     

### 10. censor    

You're doing great with these string function challenges. Last one!



**설명:** [ Learn ]          
• Ch10. censor 에서는 문자열 조작 기능을 하나 더 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write a function called `censor` that takes two strings, `text` and `word`, as input.     
* It should return the text with the word you chose **replaced with asterisks**.     

For example:    
```python
censor("this hack is wack hack", "hack")
```    
should return:    
```python
"this **** is wack ****"
```    
* Assume your input strings won't contain punctuation or upper case letters.    
* The number of asterisks you put should correspond to the number of letters in the censored word.    



**설명:** [ Instruction ]          
• 함수 censor(text, word): 를 작성하라.    
• 이 함수는 입력받은 text 중 word 글자 부분만 ( * ) 로 변경하는 함수이다.     
• 입력값으로 대문자는 입력하지 않는다.    
• ( * ) 로 대체할때, 변수 word 수 만큼만 * 로 대체해야 한다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can use    

<br>
```python
string.split()
# and 
" ".join(list)
```    
<br>    

* to help you here.    

* Remember: "*" * 4 equals "****"

* After splitting the string with string.split(), you can loop through the indices in the list and replace the words you are looking for with their asterisk equivalent.     
* Join the list at the end to get your sentence!




**설명:** [ Hint ]          
• 함수 string.split() 와  " ".join(list) 를 활용한다.     
• `*` x 4 는  `****` , 즉 `*` 를 4개로 만든다.     
• 입력된 문자열을 반복하면서 하나씩 읽는다.    
• 해당 문자가 대치할 문자와 같은지 비교한다.     
• 해당 문자가 같으면, 그 문자 크기만큼 ( * ) 를 변경한다.    
• 비교한 문자열을 리스트에 저장한다.    
• 저장된 리스트를 하나의 문자열로 만든다.     
• 최종 반환한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>

```python
def censor(text, word):
    words = text.split()
    result = ''
    stars = '*' * len(word)
    count = 0
    for i in words:
        if i == word:
            words[count] = stars
        count += 1
    result =' '.join(words)

    return result

print censor("this hack is wack hack", "hack")

# def censor2(text, word):
#   low_text = text.lower()
#   low_word = word.lower()
  
#   list_text = []
#   for t in low_text.split():
#     if t == low_word:
#        t = "*" * len(t)
#        list_text.append(t)
#     else:
#       list_text.append(t)
  
#   return " ".join(list_text)

# print censor2("this hack is wack hack", "hack")
```

**설명:** [ Solution ]    
• 정의된 함수 def censor(text, word): 는 다음과 같이 동작한다.    
• 입력된 문장(text) 중 특정단어(word)를 ( * )로 변환한다.    
• 메서드 .split() 를 사용하여 입력받은 text 의 문자열을 단어별로 자른다.    
• 잘라진 단어를 리스트 words 에 저장한다.        
• 결과물을 저장할 변수 result 를 초기화한다.    
• 변수 starts 에 ( * ) 를 변경할 word 갯수만큼 저장한다.    
• 변수 count 를 0 으로 초기화 한다.    
• for 문에서 리스트 words 에서 하나씩 단어를 추출하여 변수 l 에 저장한다.    
• 변수 l 과 ( * ) 로 바꿀 입력값 word 와 같은지 비교한다.    
• 만약, 같으면 words[count] = stars 를 저장한다.   
• 만약, 틀리면 count 를 값 1 을 증가후 다시 for 문을 진행한다.     
• result 에 word 의 빈공백 `' '` 를 추가하여 저장한다.    
• e.g. `result =' '.join(words)`    
• result 값을 반환한다.
{: .notice--info}



**결과** 
``` 
this **** is wack ****
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font>     

### 11. count     

Great work so far. Let's finish up by practicing with a few functions that take lists as arguments.



**설명:** [ Learn ]          
• Ch11. count 에서는 입력값 중 찾고자 하는 Item 이 몇개 있는지 찾는것을 학습한다.    
• 리스트를 arguments 값으로 갖는 함수들을 연습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function called `count` that has two arguments called `sequence` and `item`.

* Return the number of times the item occurs in the list.

* For example: count([1, 2, 1, 1], 1) should return 3 (because 1 appears 3 times in the list).

* There is a list method in Python that you can use for this, but you should do it the long way for practice.    
* Your function should return an integer.    
* The item you input may be an integer, string, float, or even another list!    
* Be careful not to use list as a variable name in your code—it's a reserved word in Python!    



**설명:** [ Instruction ]          
• 함수 count(sequence, item) 를 작성하라.    
• 이 함수는 다음과 같이 동작한다.     
• 함수 count( [1, 2 ,1, 1], 1 ) 을 호출하면 3이 반환된다.    
• 이유는 리스트 [1, 2, 1, 1] 에 1 이 3개가 들어 있기 때문이다.    
• python 자체 함수에는 리스트의 특정 항목의 갯수를 찾아주는 기능이 있다.    
• e.g. str.count()    
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

• 하지만, 연습을 위해서 이번 장에서 우리는 직접 만들어 본다.     
• return(반환값)은 정수(integer) 이다.    
• 입력값은 정수(integer), 문자(string), 실수(float) 또는 다른 것일 수 있다.    
• 리스트 변수명을 정할때, python에서 예약된 코드는 사용 금지한다.     
• e.g. 예약어 : if , else  등
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can set a `sum` variable inside count.     
* You can then iterate over sequence and increment `sum` every time you find an element in the sequence that matches item.


**설명:** [ Hint ]          
• 변수 sum 을 만든다.    
• 찾고자 하는 숫자와 같은 것이 있으면 변수 sum 을 값 1 씩 증가시킨다.
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def count(sequence, item):
    count = 0
    for i in sequence:
        if i == item:
            count += 1
    return count
  
print count([1, 2, 1, 1], 1)

```

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• 정의된 함수 count(sequence, item): 는 다음과 같이 동작한다.     
• 입력값 리스트 [1, 2, 1, 1] 에 값 1 이 몇개 있는지 찾는 함수다.    
• 변수 count 를 0 으로 초기화 한다.    
• for 문에서, 입력값 리스트 sequence 를 하나씩 추출하여 변수 i 에 저장한다.     
• 추출한 변수 i 의 값과 입력값 item 을 비교한다.     
• 만약, 같으면 변수 count 의 값을 1 증가한다.    
• for 문이 완료되면, 변수 count 값을 반환(return) 한다.
{: .notice--info}


<br>

**결과** 
``` 
3
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font>     

### 12. purify    

Awesome! Now let's practice filtering a list.      



**설명:** [ Learn ]          
• Ch12. purify 에서는 리스트의 필터링을 학습한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function called `purify` that takes in a list of numbers, **removes all odd numbers** in the list, and **returns the result**. For example, purify([1,2,3]) should return [2].

* Do not directly modify the list you are given as input; instead, return a new list with only the **even numbers**.




**설명:** [ Instruction ]          
• 함수 purify(list) 를 작성하라.    
• 이 함수는 리스트의 값중 홀수값이 있으면 삭제하고 해당 리스트를 return(반환)한다.     
• 입력받은 리스트를 바로 수정하지 말고, 새로운 리스트를 만들어 결과값을 저장하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Your code should share something in common with the `is_even` function you defined earlier.

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]     
• 앞에서 연습한 함수 is_even() 의 기능을 활용하여 홀수인지 짝수인지를 판단하라.    
• e.g. `if i % 2 == 0` 이면 짝수이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def purify(lst):
    res = []
    for ele in lst:
        if ele % 2 == 0:
            res.append(ele)
    return res
  
print purify([1, 2, 3, 4])
```

**설명:** [ Solution ]          
• 정의된 함수 purify(lst): 는 다음과 같이 동작한다.    
• 이 함수는 입력값중 특정(홀수)값을 삭제하는 함수이다.    
• 이 함수는 다음과 같이 동작한다.   
• 빈 리스트 res 를 정의한다.    
• for 문에서 입력받은 lst 를 하나씩 추출하여, 변수 ele 에 저장한다.    
• 변수 ele 의 값이 짝수 이면, 리스트에 추가한다.(e.g. res.append(ele))    
• for 문이 종료되면 리스트 res 를 반환한다.    
• 함수 purify([1, 2, 3, 4]) 를 호출 후 반환값을 출력한다.
{: .notice--info}



**결과** 
``` 
[2, 4]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font>     

### 13. product    

Great! Now let's try a little multiplication.



**설명:** [ Learn ]         
• Ch13. product 에서는 리스트의 항목 내용을 모두 곱하는 부분을 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function called `product` that takes a list of integers as input and **returns** the product of all of the elements in the **list**. For example: product([4, 5, 5]) should return 100 (because 4 * 5 * 5 is 100).

* Don't worry about the list being empty.
* Your function should return an integer.



**설명:** [ Instruction ]          
• 함수 product(lst) 를 작성하라.    
• 이 함수는 입력값으로 가지는 리스트의 모든 값을 곱한 결과를 반환(return)한다.    
• 리스트의 항목은 정수값 이다.    
• e.g. 함수 product([4,5,5]) 를 호출하면, 반환(return)값은 100 이다.    
• 리스트가 비어 있을 경우는 없다.    
• return(반환)값은 정수이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>

* You can use a loop to go through the elements of the list.

* It'll probably be useful to use the `*=` operator.

* Be careful **not to start your total at 0**, as this would make the overall result of the multiplication equal to 0! (Anything multiplied by zero equals zero.)




**설명:** [ Hint ]          
• 입력받은 리스트의 값을 하나씩 추출하여 ( *= ) 기능을 사용하라.    
• 전체 값을 담는 변수 total 의 초기값은 0으로 해선 안된다.     
• 이유는 곱셈에서 0은 어떤 값을 곱해도 0이다.    
• 변수 total 의 초기값은 1로 초기화 하라.  
{: .notice--info}

<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def product(list):
  total = 1
  for num in list:
    total = total * num
    #total *=num
  return total

print product([4, 5, 5])
```

**설명:** [ Solution ]          
• 정의된 함수 product(list):는 다음과 같이 작동한다.    
• 이 함수는 입력받은 리스트의 값들을 모두 곱한 결과를 반환한다.    
• 변수 total 을 값 1 로 초기화 한다.    
• for 문에서 입력받은 list 의 값을 하나씩 추출하여 변수 num 에 저장한다.    
• 변수 total 과 변수 num을 곱한 값을 다시 변수 total 에 저장한다.    
• for 문이 종료되면, 변수 total 값을 반환한다.
{: .notice--info}


**결과** 
``` 
100
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font>     

### 14. remove_duplicates    

Awesome! Now for something a bit trickier.



**설명:** [ Learn ]          
• Ch14. remove_duplicates 에서는 리스트 값의 중복을 제거하는것을 학습한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write a function `remove_duplicates` that takes in a list and removes elements of the list that are the same.

* For example: remove_duplicates([1, 1, 2, 2]) should return [1, 2].

* Don't remove every occurrence, since you need to keep a single occurrence of a number.    
* The order in which you present your output does not matter. So returning [1, 2, 3] is the same as returning [3, 1, 2].    
* Do not modify the list you take as input! Instead, return a new list.



**설명:** [ Instruction ]          
• 함수 remove_duplicates(lst) 는 다음과 같이 동작한다.    
• 이 함수는 리스트 안에 중복 값이 있으면 해당 값 하나만 남겨 놓고 나머지는 삭제한다.    
• e.g. remove_duplicates([1,1,2,2]) 호출하면, [1,2]를 반환(return)한다.     
• 모두 다 지우는 것이 아니라, 중복된 값 하나만 남겨둔다.    
• 반환(return)값의 순서는 중요치 않다.    
• e.g. [1,2,3] : ok, [3,2,1] : ok      
• 입력받은 리스트 lst 를 직접 수정하지 않는다.    
• 새로운 빈 리스트 new_lst=[] 를 만들어 저장후 반환(return) 한다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* The easiest way to approach this problem is to create a new list in your function, loop through your input list, and add items from your input list to your new list if the current item is not already contained in your new list. Using the a not in b syntax might help you here.

* Also, note that destructively modifying a list while you are looping through it is bad practice and will likely lead to bugs somewhere down the line! That's why we always make a fresh copy to work on.



**설명:** [ Hint ]          
• 가장 쉬운 방법은 함수안에 새로운 리스트를 하나 만든다.    
• 입력 받은 리스트를 반복하여 돌면서 해당 항목값을 추출하여 새로운 리스트에 추가한다.    
• 추가할때, 새로운 리스트에 내가 추가할 항목이 있는지를 점검한다.    
• 만약 없으면 추가하고, 있으면 다음 단계로 넘어간다.     
• 기존 리스트를 수정하는 것보단, 새로운 리스트를 구성하는 방식이 안전하다.    
• 이유는 기존 리스트를 잘못 수정하면 복원하기 어렵기 때문이다.    
• 새로운 리스트를 잘못 수정했으면, 다시 지우고 만들면 된다. 
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def remove_duplicates(inputlist):
    if inputlist == []:
        return []
    
    # Sort the input list from low to high    
    inputlist = sorted(inputlist)
    # Initialize the output list, and give it the first value of the now-sorted input list
    outputlist = [inputlist[0]]
```
<p style="page-break-before: always;"></p>
<br>

```python
    # Go through the values of the sorted list and append to the output list
    # ...any values that are greater than the last value of the output list
    for i in inputlist:
        if i > outputlist[-1]:
            outputlist.append(i)
        
    return outputlist
  
print remove_duplicates([1, 1, 2, 2])

```


**설명:** [ Solution ]          
• 정의된 함수 remove_duplicates(inputlist): 는 다음과 같이 동작한다.    
• 이 함수는 입력된 리스트의 중복값을 제거해주는 함수이다.    
• 이 함수는 입력값으로 리스트 inputlist 를 받는다.   
• 입력값 리스트 inputlist 가  비어 있으면 빈 리스트 ( [] ) 를 반환(return)한다.    
• 입력값 리스트 inputlist 를 정렬한다.    
• e.g. inputlist = sorted(inputlist)    
• 정렬된 첫번째 값(inputlist[0])을 리스트 outputlist 에 추가한다.     
• for 문에서 정렬된 inputlist 의 값을 하나씩 추출하여 변수 i 에 저장한다.    
• 추출한 값 i 와 제일 마지막값(outputlist[-1])을 비교한다.    
• 마지막 값과 비교하는 이유는 이미 outputlist 값을 정렬해 놓았기 때문이다.    
• 만약 i 값이 마지막값 보다 크면 변수 outputlist.append(i)와 같이 추가한다.    
• 최종 outputlist 를 반환(return) 한다.
{: .notice--info}


**결과** 
``` 
[1, 2, 4]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font>     

### 15. median    

Great work! You've covered a lot in these exercises. Last but not least, let's write a function to **find the median of a list**.

The median is the middle number in a sorted sequence of numbers.

Finding the median of [7, 12, 3, 1, 6] would first consist of sorting the sequence into [1, 3, 6, 7, 12] and then locating the middle value, which would be 6.

If you are **given** a sequence with an **even number** of elements, you must **average the two elements surrounding the middle**.

For example, the median of the sequence [7, 3, 1, 4] is 3.5, since the middle elements after sorting the list are 3 and 4 and (3 + 4) / (2.0) is 3.5.

You can sort the sequence using the sorted() function, like so:    
```python
sorted([5, 2, 3, 1, 4])
[1, 2, 3, 4, 5]
```



**설명:** [ Learn ]          
• Ch15. median 에서는 리스트 중간값 찾는것을 학습한다.    
• 리스트의 중앙에 위치한 값을 찾는 함수를 만들어 보자.    
• 리스트 [7, 12, 3, 1, 6] 이 입력되면, 먼저 정렬하여 [1, 3, 6, 7, 12] 를 만든다.    
• 그리고 리스트의 중앙에 위치한 6 을 반환(return)한다.    
• 리스트 [7, 3, 1, 4] 와 같이  짝수개가 입력되면,    
• 정렬 후 [1, 3, 4, 7] 중앙값 3 과 4 의 평균값이 3.5가 반환(return)된다.    
• 정렬은 함수 sorted([5, 2, 3, 1, 4])를 사용하면 [1, 2, 3, 4, 5] 로 정렬이 된다.
{: .notice--info}



<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

* Write a function called `median` that takes a list as an input and **returns the median** value of the list.     

* For example: median([1, 1, 2]) should return 1.    

* The list can be of any size and the numbers are not guaranteed to be in any particular order. Make sure to sort it!    
* If the list contains an **even number** of elements, your function should **return the average of the middle two**.
 


**설명:** [ Instruction ]          
• 함수 median(lst) 를 작성하라.    
• 이 함수는 입력된 리스트의 중간 항목값을 반환(return)한다.    
• 입력되는 리스트의 크기는 다를수 있다.   
• 리스트에 들어있는 값들은 정렬되어 있지않다.     
• 짝수개의 리스트가 입력되면 중간 항목 2개의 평균값을 반환(return)한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* In order to find the median of a list with an even number of elements, you're going to need to find the indices of the middle two elements.

* You can find the middle two elements by halving the length of the array to find the index of the first element, and subtracting one from the first index to find the second index.

* For example, with an array of length 6 like [0, 1, 2, 3, 4, 5], the two middle elements that need to be averaged in order find the median would be 2 and 3. You get 3 by cutting the length of the array in half and 2 by subtracting 1 from the previous index: 3. You can use a similar pattern to find the middle element of an odd-length list.

* Last but not least, note that (2 + 3) / 2 is not the same as (2 + 3) / 2.0! The former is integer division, meaning Python will try to give you an integer back. You'll want a float, so something like (2 + 3) / 2.0 is the way to go.



<p style="page-break-before: always;"></p>
<br>


**설명:** [ Hint ]          
• 짝수개의 리스트가 들어오면 중간값을 찾는 방법은 다음과 같다.    
• 입력된 리스트의 길이를 구한다.     
• 만약 [0, 1, 2, 3, 4, 5] 가 입력되면 길이는 6 이다.    
• 이를 반으로 나누면 중간 값은 3 이다.    
• 리스트의 index 값이 3인 자리의 값은 3 이다.    
• 우리가 필요한 값은 index 2 와 index 3 이다.    
• e.g. index 3 에서 index 1 을 뺀 index 2 를 선택한다.     
• 주의, 두개의 값을 나누어 중간값을 계산할때, 다음 2가지 경우의 결과 값은 다르다.    
• e.g. ( (2 + 3) / 2 ) 과 ( (2 + 3) / 2.0 )     
• 앞의 경우는 2 가 반환되고, 후자는 2.5 가 반환다.    
• 이 함수에서는 후자의 방식( (2+3)/2.0 )을 이용해야 한다.    
• e.g. Python3 에서는 이 문제가 해결되어, 2를 사용해도 문제없다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def median(lst):
    sorted_list = sorted(lst)
    if len(sorted_list) % 2 != 0:
        #odd number of elements
        index = len(sorted_list)//2 
        return sorted_list[index]
    elif len(sorted_list) % 2 == 0:
        #even no. of elements
        index_1 = len(sorted_list)/2 - 1
        index_2 = len(sorted_list)/2
        mean = (sorted_list[index_1] + sorted_list[index_2])/2.0
        return mean
   
print median([2, 4, 5, 9])

```

**설명:** [ Solution ]          
• 정의된 함수 median(lst): 는 다음과 같이 동작한다.    
• 이 함수는 입력값 리스트의 중간값을 반환한다.    
• 이 함수는 lst 를 입력값으로 받는다.    
• 입력된 리스트를 정렬한다.(e.g. sorted_list = sorted(lst) )    
• if 절의 block 내용은 리스트의 갯수가 홀수개가 입력 되었을때 동작한다.     
• if 절의 내용은 다음과 같이 처리한다.    
• 리스트의 갯수가 홀수이면 index 중간값을 구한다.    
• e.g. 리스트의 중간값을 ( //2 )로 소수점 버리는 중간값으로 계산한다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

• 리스트 sorted_list[index]가 중간 값이므로 해당 값을 반환(return)한다.    
• else 절의 block 내용은 짝수 개가 입력 되었을때 동작한다.       
• else 절의 내용은 다음과 같이 처리한다.    
• 리스트의 길이를 구하여 반으로 나누면 중간 index 값이 된다.    
• e.g. len(sorted_list)/2     
• e.g. 입력 리스트 [0, 1, 2, 3] 는 길이는 4, 중간 index 계산값은 2가 나온다.    
• 우리가 필요한 1, 2의 index 값은 1, 2 이므로,    
• 변수 index_1 = 중간 index -1 이 된다.    
• 변수 index_2 = 중간 index 이다.     
• 두개의 index 값을 더하여 평균값을 구하여 반환(return)한다.
{: .notice--info}


**결과** 
``` 
4.5
```