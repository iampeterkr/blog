---
# layout : rchive
title: "Python Syntax"
permalink: /p3-python-syntax/
excerpt: "We learn about Python Syntax."
last_modified_at: 2019-04-08T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
   
<hr style="border: solid 1px #dddddd ;">    
LESSON    

In this course we'll learn about the syntax of the Python programming language! We will go over fundamental commands that store variables, print messages, and perform mathematical operations.  


**설명:** [ 학습방향 ]     
이 장에서는 객체 지향 프로그램 언어인 Python을 소개합니다.     
기본적인 명령어와, 변수, 메시지 출력방법, 수학연산을 배운다.
{: .notice--info}     
     
 <hr style="border: solid 1px #dddddd ;">

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 1. Welcome    


Python is a programming language. Like other languages, it gives us a way to communicate ideas. In the case of a programming language, these ideas are “commands” that people use to communicate with a computer!

We convey our commands to the computer by writing them in a text file using a programming language. These files are called programs. Running a program means telling a computer to read the text file, translate it to the set of operations that it understands, and perform those actions.


**설명:** [ Learn ]     
• Ch1. Hello World! 에서는 print 문을 학습한다.      
• 우리가 배워야 할 첫번째 Python 문법은 print 문이다.     
• print 문은 컴퓨터와 대화 하는것을 실질적으로 사람이 볼수 있게 해준다.     
• 상단 검정 박스안의 Python 소스를 Editor 화면에 복사하여 실행(Run) 해 보자.     
• 우리는 컴퓨터에게 *Hello World!* 라는 문장을 화면에 출력 시키라고 명령한 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

Change Codecademy to your name in the script to the right. Run the code to see what it does! As soon as you’re ready, move on to the next exercise to begin learning to write your own Python programs!    

```python
my_name = "Codecademy"
print("Hello and welcome " + my_name + "!")
```


**설명:** [ Instruction ]    
변수 my_name 의 Codecademy 를 당신의 이름으로 변경하라.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Skip


**설명:** [ Hint ]    
skip
{: .notice--info}

<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
my_name = "LWY"
print("Hello and welcome " + my_name + "!")
```


**설명:** [ Solution ]    
변수 my_name 의 변경 내용이 출력된다.
{: .notice--info}

**결과**    
```
Hello and welcome LWY !
```

<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 2. Comments    

Ironically, the first thing we’re going to do is show how to tell a computer to ignore a part of a program. Text written in a program but not run by the computer is called a comment. Python interprets anything after a # as a comment.

Comments can:    

* Provide context for why something is written the way it is:

```python
# This variable will be used to count the number of times anyone tweets the word persnickety
persnickety_count = 0    
```

* Help other people reading the code understand it faster:    

```python
# This code will calculate the likelihood that it will rain tomorrow
complicated_rain_calculation_for_tomorrow()    
```    

* Ignore a line of code and see how a program will run without it:

```python
# useful_value = old_sloppy_code()
useful_value = new_clean_code()




**설명:** [ Learn ]    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

Documentation is an important step in programming. Write a comment describing the first program you want to write!

**설명:** [ Instruction ]     
코멘트 처리를 하여라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Start your comment with # and write the rest of your comment afterwards.    


**설명:** [ Hint ]     
{: .notice--info}

<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
# Start your comment with # and write the rest of your comment afterwards.
```

**설명:** [ Solution ]    
{: .notice--info}

**결과**    
```
Skip
```
<br>
<br>
<br>
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 3. Print    

Now what we’re going to do is teach our computer to communicate. The gift of speech is valuable: a computer can answer many questions we have about “how” or “why” or “what” it is doing. In Python, the print() function is used to tell a computer to talk. The message to be printed should be surrounded by quotes:

```python
# from Mary Shelley's Frankenstein
print("There is something at work in my soul, which I do not understand.")    
```

In the above example, we direct our program to print() an excerpt from a notable book. The printed words that appear as a result of the print() function are referred to as output. The output of this example program would be:

```
There is something at work in my soul, which I do not understand.
```


**설명:** [ Learn ]      
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Print the distinguished greeting “Hello world!”

**설명:** [ Instruction ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

```python
print ("Hello world")
```

**설명:** [ Hint ]     

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print "Hello " + "Wonyoung Lee"
```

**설명:** [ Solution ]     
• 두 개의 스트링을 연결 할때는 ( + )를 사용한다.
{: .notice--info}


**결과**     
``` 
Hello Wonyoung Lee
```   

<br>
<br>    
<br>    
<p style="page-break-before: always;"></p>      
<br>



![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 4. Handling Errors    

As we get more familiar with the Python programming language, we run into errors and exceptions. These are complaints that Python makes when it doesn't understand what you want it to do. Everyone runs into these issues, so it is a good habit to read and understand them. Here are some common errors that we might run into when printing strings:

```python
print "Mismatched quotes will cause a SyntaxError'
print Without quotes will cause a NameError
```

If the quotes are mismatched Python will notice this and inform you that your code has an error in its syntax because the line ended (called an `EOL`) before the double-quote that was supposed to close the string appeared. The program will abruptly stop running with the following message:

```bash
SyntaxError: EOL while scanning a string literal
This means that a string wasn't closed, or wasn't closed 
with the same quote-character that started it.
```

Another issue you might run into is attempting to create a string without quotes at all. Python treats words not in quotes as commands, like the print statement. If it fails to recognize these words as defined (in Python or by your program elsewhere) Python will complain the code has a NameError. This means that Python found what it thinks is a command, but doesn't know what it means because it's not defined anywhere.



**설명:** [ Learn ]        
• Ch4. Handling Errors 에서는 Error에 대하여 학습한다.     
• 쿼트(quotes)가 시작과 끝이 같지 않으면, Python은 *EOL Error*를 발생시킨다.   
• e.g. SyntaxError: EOL while scanning string literal    
• *EOL : End Of Line*  
• *EOL Error*는 Python이 문자열을 만드는 과정에서 문법적 Error가 발생했다는 뜻이다.    
• 시작이 (') 이면 끝도 (') 이어야 한다.    
• 시작이 (") 이면 끝도 (") 이어야 한다.     
• 문자열의 양 끝에 쿼트(quotest)가 없으면 Python은 해당 문자열을 변수로 인식한다.    
• 또는 print 와 같은 명령문으로 인식한다.    
• 이런 경우 Python 은 해당 문자열을 명령어(or 변수) 리스트에서 찾는다.    
• 만약, 리스트에서 찾을수 없으면 *NameError* 를 발생시킨다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* We've written two `print` statements that will raise errors.     
* One has mismatched quotes and the other has no quotes at all.

* Fix the two print statements to successfully debug the program!

**설명:** [ Instruction ]    
• 쿼트(quotes)를 잘못 사용하면 Error 가 발생한다.    
• 잘못된 Python 프로그램을 고쳐라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* A `print` statement should start with the word print and then should have the message inside matching quote marks.

```python
print 'This is a good print statement'
```   

* Double quotes are also fine:

```python
print "This is also a good print statement"
```


**설명:** [ Hint ]    
• 문자열은 쿼트(quotes)의 처음과 끝이 같은 모앙이어야 한다. 
{: .notice--info}


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print("How do you make a hot dog stand?")
print("You take away its chair!")
```

**설명:** [ Solution ]     
• 문자열을 표현할때는 처음과 끝의 쿼트 모양이 같아야 한다.
{: .notice--info}


**결과**     
``` 
How do you make a hot dog stand?
You take away its chair!
```   

<br>
<br>    
<br>   
<p style="page-break-before: always;"></p>     
<br>    

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 5. Variables    

In Python, and when programming in general, we need to build systems for dealing with data that changes over time. That data could be the location of a plane, or the time of day, or the television show you're currently watching. The only important thing is that it may be different at different times. Python uses variables to define things that are subject to change.

```python
greeting_message = "Welcome to Codecademy!"
current_excercise = 5
```

In the above example, we defined a variable called `greeting_message` and set it equal to the string "Welcome to Codecademy!". It also defined a variable called `current_exercise` and set it equal to the number 5.




**설명:** [ Learn ]       
• Ch5. Variables 에서는 변수를 학습한다.    
• 변수는 문자열이나, 숫자를 저장하기 위한 상자이름 이다.     
• 우리는 greeting_message 라는 변수 상자를 만든다.    
• 그 변수 상자에 *Welcome to Codecademy!* 라는 문자열을 저장한다.    
• greeting_message 는 문자를 담은 변수 상자가 된다.    
• Python 에서는 greeting_message 를 변수라 부른다.    
• 마찬가지로 우리는 숫자를 담기 위한 current_exercise 라는 변수 상자를 만든다.    
• 그 변수 상자에 숫자 5 를 담는다.    
• current_exercise 는 숫자를 담은 변수 상자가 된다.   
• 우리는 이것을 변수 current_exercise 라고 부른다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a variable called `toodays_date` and assign a value that will represent today's date to that variable.

**설명:** [ Instruction ]     
• 변수 todays_date 를 만들고, 이 변수에 오늘 날짜를 넣어라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

```python
todays_date = "March 31, 2023"
```


**설명:** [ Hint ]    
• 변수 todays_date 를 만들고 거기에 *March 31, 2023* 문자열을 넣는다.
{: .notice--info}
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
todays_date = "November 19, 2018"
```

**설명:** [ Solution ]     
• 변수 todays_date 에 문자열을 넣는다.
{: .notice--info}


**결과**     
``` 
#skip
```   

<br>
<br>    
<br>   
<p style="page-break-before: always;"></p>     
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 6. Arithmetic    

One thing computers are capable of doing exceptionally well is performing arithmetic. Addition, subtraction, multiplication, division, and other numeric calculations are easy to do in most programming languages, and Python is no exception. Some examples:

```python
mirthful_addition = 12381 + 91817
amazing_subtraction = 981 - 312
trippy_multiplication = 38 * 902
happy_division = 540 / 45
sassy_combinations = 129 * 1345 + 120 / 6 - 12
```

Above are a number of arithmetic operations, each assigned to a variable. The variable will **hold the final result** of each operation. Combinations of arithmetical operators follow the usual order of operations.

Python also offers a companion to division called the modulo operator. The modulo operator is indicated by % and returns the remainder after division is performed.

```python
is_this_number_odd = 15 % 2
is_this_number_divisible_by_seven = 133 % 7
```   

In the above code block, we use the modulo operator to find the remainder of `15` divided by `2`. Since `15` is an odd number the remainder is `1`.

We also check the remainder of `133 / 7`. Since `133` divided by `7` has no remainder, `133 % 7` evaluates to `0`.



**설명:** [ Learn ]     
• Ch6. Arithmetic 에서는 수식을 학습한다.     
• 컴퓨터의 많은 기능 중 하나는 계산하는 것이다.     
• Python도 사칙연산( + , − , × , ÷ )을 지원한다.    
• Python 에선 × → * , ÷ → / 로 표시한다.    
• 모듈(module)연산자도 지원한다.     
• 모듈 연산자 중 하나인 % 는 나머지를 계산 해준다.    
• e.g. 15 % 2 = 1, 만약 133 % 7 같이 딱 떨어지면 나머지는 0 이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Multiply two numbers together and assign the result to a variable called `product`.    

* What is the remainder when 1398 is divided by 11? Save the results in a variable called `remainder`.    

**설명:** [ Instruction ]    
• 변수 product 를 만들어라.    
• 변수 product 에 2개의 숫자를 곱하여 대입하라.  
• 1398 / 11  의 나머지는 무엇일까?     
• 변수 remainder 를 만들어라.    
• 변수 remainder 에 1397 / 11 의 나머지 값을 저장하라.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Remember creating a variable is as simple as setting it equal to something else. To define a variable called quotient you would write the following:

```python
quotient = 30 / 5
```

* Remember that remainders can be found using the modulus operator. Calculate a remainder with `%`.

```python
1908 % 3
```

* Will be `0` because `1908` is divisible by `3`.

**설명:** [ Hint ]    
• 상기 예는 변수 quotient 에 두 수를 나눗셈 한 것이다.    
• % 는 나머지를 구하는 모듈(module) 연산자 이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
product = 18 * 13
remainder = 1398 % 11
```

**설명:** [ Solution ]     
•  곱셈 연산자는 * 이다.     
•  나머지를 구하는 모듈(module) 연산자는 % 이다. 
{: .notice--info}    


**결과**     
``` 
#skip
```   

<br>
<br>    
<br>    
<p style="page-break-before: always;"></p>     
<br>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 7. Updating Variables    

Changing the contents of a variable is one of the essential operations. As the flow of a program progresses, data should be updated to reflect changes that have happened.

```python
fish_in_clarks_pond = 50

print "Catching fish"

number_of_fish_caught = 10

fish_in_clarks_pond = 
fish_in_clarks_pond - 
number_of_fish_caught
```

In the above example, we start with `50` fish in a local pond. After catching `10` fish, we update the number of fish in the pond to be the original number of fish in the pond minus the number of fish caught. At the end of this code block, the variable `fish_in_clarks_pond` is equal to `40`.

Updating a variable by adding or subtracting a number to the original contents of the variable has its own shorthand to make it faster and easier to read.

**설명:** [ Learn ]       
• Ch7. Updating Variables 에서는 변수 변경을 학습한다.    
• 변수 fish_in_clarks_pond 에 50 을 대입하라.    
• 변수 number_of_fish_caught 에 10 을 대입하라.    
• 변수 fish_in_clarks_pond = fish_in_clarks_pond - number_of_fish_caught    
• 변수 fish_in_clarks_pond 에는 50 - 10 의 값이 계산된 40 이 저장된다. 
{: .notice--info}


```python
money_in_wallet = 40
sandwich_price = 7.50
sales_tax = .08 * sandwich_price

sandwich_price += sales_tax
money_in_wallet -= sandwich_price
```

In the above example, we use the price of a sandwich to calculate sales tax. After calculating the tax we add it to the total price of the sandwich. Finally, we complete the transaction by reducing our `money_in_wallet` by the cost of the sandwich (with tax).


**설명:** [ Learn ]     
• 변수에 숫자를 곱하여도 계산 할 수 있음을 보여준다.     
• +=, -= 연산자를 활용하는 법을 보여준다.     
• a = a + 1, a += 1, 이 두 표현은 같은 표현이다.    
• a = a - 1, a -= 1, 이 두 표현은 같은 표현이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    
* We're trying to figure out how much it rained in the past year! Update the `annual_rainfall` variable to include the values from September to December.

**설명:** [ Instruction ]    
• 작년에 얼마나 많은 비가 왔는지 계산 하는 문제이다.    
• 변수 annual_rainfall 에, 9월 부터 12월 까지의 비의 양을 누적하여 값을 더하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Use the `+=` syntax to add a value to an existing variable:

```python
annual_rainfall += september_rainfall
```

* Add all of the remaining months to


**설명:** [ Hint ]    
• += 연산자를 사용하라.  
{: .notice--info}

<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
january_to_june_rainfall = 1.93 + 0.71 + 3.53 + 3.41 + 3.69 + 4.50
annual_rainfall = january_to_june_rainfall

july_rainfall = 1.05
annual_rainfall += july_rainfall

august_rainfall = 4.91
annual_rainfall += august_rainfall

september_rainfall = 5.16
annual_rainfall += september_rainfall

october_rainfall = 7.20
annual_rainfall += october_rainfall

november_rainfall = 5.06
annual_rainfall += november_rainfall

december_rainfall = 4.06
annual_rainfall += december_rainfall
print annual_rainfall
```

**설명:** [ Solution ]    
• += 연산자를 사용하여 매월 비의 양을 추가 한다.     
• 변수 annual_rainfall 의 마지막 값을 출력 한다. 
{: .notice--info}


**결과**     
``` 
45.21
```   

<br>
<br>    
<br>    
<p style="page-break-before: always;"></p>     
<br>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 8. Comments    

Most of the time, code should be written in such a way that it is easy to understand on its own. However, if you want to include a piece of information to explain a part of your code, you can use the `#` sign. A line of text preceded by a `#` is called a comment. The machine does not run this code — it is only for humans to read. When you look back at your code later, comments may help you figure out what it was intended to do.

```python
# this variable counts how many rows of
the spreadsheet we have:
row_count = 13
```


**설명:** [ Learn ]     
• Ch8. Comments 에서는 주석을 학습한다.    
• Python 에서 프로그램으로 인식되지 않는 부분을 주석(Comment) 이라고 한다.    
• 주석의 사용 목적은 프로그램에 정보를 남겨두거나 설명하기 위해서이다.     
• 주석 처리된 부분은 컴퓨터는 인식 못하고 오직 프로그램을 읽는 사람만이 인식한다.    
• 주석을 만들때는 # 을 사용한다.     
• 한줄 주석(Comment)은 # 으로 처리 한다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Add a comment above the declaration of `city_pop` with a description of what you think the variable contains.


**설명:** [ Instruction ]    
• 변수 city_pop 위에 주석을 만들어라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the `#` 


**설명:** [ Hint ]    
• # 을 활용 하라.
{: .notice--info}   


<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
city_name = "St. Potatosburg"

# This number tracks the population count of the spudizens of St. Potatosburg
city_pop = 340000
```

**설명:** [ Soluction ]    
• # 을 사용하여, 변수 city_pop 에 저장한  34000 에 대한 설명을 남겨둔다.  
{: .notice--info}    


**결과**     
``` 
#skip
```   

<br>
<br>    
<br>    
<p style="page-break-before: always;"></p>     
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 9. Numbers    

Variables can also hold numeric values. The simplest kind of number in Python is the **integer**, which is a whole number with no decimal point:

```python
int1 = 1
int2 = 10
int3 = -5
```

A number with a decimal point is called a **float**. You can define **floats** with numbers after the decimal point or by just including a decimal point at the end:

```python
float1 = 1.0
float2 = 10.
float3 = -5.5
```

You can also define a **float** using scientific notation, with e indicating the power of `10`:

```python
# this evaluates to 150:
float4 = 1.5e2
```


**설명:** [ Learn ]      
• Ch9. Numbers 에서는 숫자를 학습한다.     
• Python 에서는 숫자 관련 변수는 정수(integer)와 실수(float) 2 종류가 있다.    
• 정수는 소숫점 이하를 표현할수 없다.    
• 실수는 소수점을 표현할 수 있다.     
• 생성되는 변수가 정수인지, 실수 인지는 해당 값을 대입 할때 정해진다.    
• 즉, 변수에 정수를 넣으면 정수형 변수가 되고, 실수를 넣으면 실수형 변수가 된다.   
• 과학적 표기법인(scientific notation) e 도 실수(float)로 표현한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* You are going shopping. Let's make a grocery list so that you can plan your budget. Store the number of cucumbers you want to buy in a variable called `cucumbers`. Make sure it's at least `1`, and that it's the appropriate datatype! The store doesn't sell partial cucumbers.    

* Each cucumber costs `3.25` doubloons. Store the price per cucumber in a variable called `price_per_cucumber`.

* Create a new variable called `total_cost` which is the product of how many cucumbers you are going to buy and the cost per cucumber.    

* Print out `total_cost`.   
* What datatype is it?

**설명:** [ Instruction ]     
• 변수 cucumbers 를 만들어라.    
• 변수 cucumbers 에 정수 1 을 대입하라.    
• 변수 price_per_cucumber 를 만들고, 3.25 를 대입하라.    
• 변수 total_cost 를 만들고, 구매 할 오이의 총 가격을 계산하여 대입하라.    
• 변수 total_cost 를 print 문을 사용하여, console 창에 출력하라.
{: .notice--info}    


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the operator `*` 


**설명:** [ Hint ]    
• 연산자 * 를 사용하여 총 합을 계산하라. 
{: .notice--info}

<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
cucumbers = 3
price_per_cucumber = 3.25

total_cost = cucumbers * price_per_cucumber
print total_cost
```

**설명:** [ Solution ]    
• 오이가 3개, 개당 가격이 3.25 이다.    
• 전체 오이의 가격은 cucumbers * price_per_cucumber 이다.    
• 변수 total_cost 에 계산한 결과 값을 저장한다.    
• 정수 3과 실수 3.25의 계산값은 실수로 자동 계산된다.    
• 입력 된 두 값( 3 , 3.25 ) 중 하나 ( 3.25 )가 실수 값 이다.    
• Python은 내부적으로 실수로 계산되어지고, total_cost 는 실수형 변수가 된다.
{: .notice--info}


**결과**     
``` 
9.75
```   

<br>
<br>    
<br>    
<p style="page-break-before: always;"></p>     
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 10. Two Types of Division     

In Python 2, when we divide two integers, we get an integer as a result. When the quotient is a whole number, this works fine:

```python
quotient = 6/2
# the value of quotient is now 3, which makes sense
```

However, if the numbers do not divide evenly, the result of the division is truncated into an integer. In other words, the quotient is rounded down to a whole number. This can be surprising when you expect to receive a decimal and you receive a rounded-down integer:

```python
quotient = 7/2
''' the value of quotient is 3, even though the result
  of the division here is 3.5 '''
```

To yield a float as the result instead, programmers often change either the numerator or the denominator (or both) to be a float:

```python
quotient1 = 7./2
# the value of quotient1 is 3.5
quotient2 = 7/2.
# the value of quotient2 is 3.5
quotient3 = 7./2.
""" the value of quotient3 is 3.5
 An alternative way is to use the float() method: """

quotient1 = float(7)/2 
# the value of quotient1 is 3.5
```

**설명:** [ Learn ]       
• Ch10. Two Types of Division 에서는 나눗셈의 주의점을 학습한다.    
• 두수를 나누어 정수로 딱 떨어지면, 해당 변수를 정수형 변수로 인식한다.    
• 정수 ( 7/2 ) 은 그 계산하면 3.5 이다. 3.5는 실수이다.    
• 하지만, Python은 정수( 3 )만 남고, 나머지 0.5는 버린다.    
• 이런 실수를 방지하기 위하여 값을 대입 할때 주의 해야한다.    
• 항상, 계산한 결과값이 실수 일 것을 대비하여야 한다.     
• 입력값을 실수형으로 넣어 준다. ( e.g. 7.0 / 3)    
• 입력값을 float(7) 실수형 값으로 변경 후 계산 되도록 한다.
{: .notice--info}    

**설명:** [ Python3 ]    
• python3 에서는 이문제를 해결 하였다.    
• 정수 ( 7/2 ) 은 그 계산하면 3.5 로 자동 출력된다.
{: .notice--info}



<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* You have come home from the grocery store with `100` cucumbers to split amongst yourself and your `5` roommates (`6` people total).

* Create a variable `cucumbers` that holds `100` and `num_people` that holds `6`.

* Create a variable called `whole_cucumbers_per_person` that is the integer result of dividing `cucumbers` by `num_people`.

* Print `whole_cucumbers_per_person` to the console.

* You realize that the numbers don't divide evenly and you don't want to throw out the remaining cucumbers.     
* Create a variable called `float_cucumbers_per_person` that holds the float result of dividing `cucumbers` by `num_people`.

* Print `float_cucumbers_per_person` to the console.

**설명:** [ Instruction ]     
• 100 개의 오이를 룸메이트 6 명과 나눠 가지는 프로그램을 만든다.     
• 변수 cucumbers 에  100 을 대입하라.    
• 변수 num_people 에 6 을 대입하라.     
• 변수 whole_cucumbers_per_person 에 (cucumbers / num_people)을 대입하라.    
• 변수 whole_cucumbers_per_person 를 출력하라.    
• 16 이 출력되어 놀라운가?     
• 예상한 바로는 100/6 은 16.66...으로 출력을 예상했는가?     
• 변수 float_cucumbers_per_person 를 만들고, 실수 값이 출력 되도록 고쳐라.    
• 변수 float_cucumbers_per_person 를 출력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can do float division by casting either the numerator or denominator as a float:

```python
quotient_with_decimals = float(5)/2
#yields 2.5
```

**설명:** [ Hint ]    
• float() 함수를 사용하라. 
{: .notice--info}


<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
cucumbers = 100
num_people = 6

whole_cucumbers_per_person = cucumbers/num_people
print whole_cucumbers_per_person

float_cucumbers_per_person = float(cucumbers)/num_people
print float_cucumbers_per_person
```

**설명:** [ Solution ]    
• float_cucumbers_per_person 변수를 계산할때, float() 함수를 사용한다.    
• float(cucumbers) 를 실수로 변경하여 계산한다.
{: .notice--info}

**결과**
```
16
16.6666666667
```


<br>
<br>    
<br>    
<p style="page-break-before: always;"></p>     
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 11. Multi-line Strings     


We have seen how to define a string with single quotes and with double quotes. If we want a string to span multiple lines, we can also use triple quotes:

```python
address_string = """136 Whowho Rd
Apt 7
Whosville, WZ 44494"""
```

This address spans multiple lines, and is still contained in one variable, `address_string`.

When a string like this is not assigned to a variable, it works as a multi-line comment. This can be helpful as your code gets more complex:

```python
""" The following piece of code does the following steps:
takes in some input
does An Important Calculation
returns the modified input and a string that says "Success!" or "Failure..."
"""
... a complicated piece of code here...
```




**설명:** [ Learn ]      
• Ch11. Multi-line Strings 에서는 다중 주석을 학습한다.     
• """ """  or ''' ''' 를 이용하여 여러줄의 문자열을 만들수 있다.    
• 문자열도 만들수 있지만, 한 줄 주석(#) 외에 여러줄의 주석을 만들때도 사용한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a variable called `haiku` and store this haiku as a multi-line string: The old pond, A frog jumps in: Plop!

**설명:** [ Instruction ]    
• 변수 haiku 를 만들어라.    
• 변수 haiku 에 다음 여러줄의 문자열을 저장하라.     
• e.g. 문자열 : *The old pond, A frog jumps in: Plop!* 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the """ """ or ''' '''


**설명:** [ Hint ]    
• """ """ or ''' ''' 를 사용하라. 
{: .notice--info}

<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
haiku = """The old pond,
A frog jumps in:
Plop!"""

print haiku
```

**설명:** [ Solution ]    
• """ """ 사용하여 여러줄의 문자열을 변수에 대입한다.  
{: .notice--info}

**결과** 
```
The old pond,
A frog jumps in:
Plop!
```


<br>
<br>    
<br>    
<p style="page-break-before: always;"></p>     
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 12. Booleans    

Sometimes we have a need for variables that are either true or false. This datatype, which can only ever take one of two values, is called a boolean. In Python, we define booleans using the keywords True and False:

```python
a = True
b = False
```

A boolean is actually a special case of an integer. A value of True corresponds to an integer value of 1, and will behave the same. A value of False corresponds to an integer value of 0.


**설명:** [ Learn ]       
• Ch12. Booleans 에서는 boolean 연산자를 학습한다.    
• Python에서 참, 거짓을 표현해야 할 때가 있다.     
• 참 은 문자열로 *True* 로 표현한다.    
• 거짓 은 문자열로 *False* 로 표현한다.     
• 참  의 값은 숫자 *1* 이다.    
• 거짓 의 값은 숫자 *0* 이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    
* Someone has introduced themselves to you using comments in script.py.

* Read the comments and then create a variable called `age_is_12` and set it to be `True` or `False` depending on if this person's age is 12.

* Create a variable called `name_is_maria` and set it to be `True` or `False` depending on if this person's name is Maria.

**설명:** [ Instruction ]    
• 변수 age_is_12 를 만들어라.    
• 주석에서 설명하는 사람의 나이가 12 살이면 True 를 대입하라.    
• 12 살이 아니면, False 를 입력하라.     
• 변수 name_is_maria 를 만들어라.    
• 주석에서 설명하는 사람의 이름이 Maria 이면 True 를 대입하라.    
• Maria 가 아니면, False 를 입력하라. 
{: .notice--info}



<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* To set a boolean to True, you would use:

```python
some_variable = True
```
**설명:** [ Hint ]    
• 주석 문을 읽고 True, False 를 이용하여 대입하라. 
{: .notice--info}

<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Hi! I'm Maria and I live in script.py.
# I'm an expert Python coder.
# I'm 21 years old and I plan to program cool stuff forever.

age_is_12 = False
name_is_maria = True
```

**설명:** [ Solution ]    
• 주석에서 Python coder 나이는 21 살, 이름은 Maria 이다.  
{: .notice--info}



<br>
<br>    
<br>    
<p style="page-break-before: always;"></p>     
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 13. ValueError    

Python automatically assigns a variable the appropriate datatype based on the value it is given. A variable with the value `7` is an **integer**, `7.` is a **float**, "7" is a **string**. Sometimes we will want to convert variables to different datatypes. For example, if we wanted to print out an **integer** as part of a **string**, we would want to convert that **integer to a string** first. We can do that using `str()`:

```python
age = 13
print "I am " + str(age) + " years old!"
```
**설명:** [ Learn ]       
• Ch13. ValueError 에서는 출력시 주의할 점을 학습한다.     
• 변수 age 는 정수 13 이 대입 되었기에 정수형 변수가 된다.     
• 정수형 변수 age 를 문자열로 출력 하기 위해선, 함수 str()를 사용한다.    
• 정수 변수 age를 str(age)로 바꾸면 age 는 문자열 형태로 출력된다.    
• *주의)* 정수형 age 를 출력 할때 문자열 형태로 출력하는 것이지, age 가 문자열 형 변수가 되는것은 아니다.  
{: .notice--info}

This would print:
``` python
>>> "I am 13 years old!"
```
Similarly, if we have a string like "7" and we want to perform arithmetic operations on it, we must convert it to a numeric datatype. We can do this using `int()`:

```python
number1 = "100"
number2 = "10"

string_addition = number1 + number2 
#string_addition now has a value of "10010"

int_addition = int(number1) + int(number2)
#int_addition has a value of 110
```
**설명:** [ Learn ]     
• 변수 number1 , number2 는 문자형 변수이다.     
• Python 에서는 문자형 데이타 이지만, 데이타가 숫자를 뜻하면 계산을 할수가 있다.     
• e.g. 문자열 "4", "5.0"    
• 단, 계산할때, 함수 int()를 사용하여 정수형으로 바꾸어 주어야 한다.     
• *주의)* 문자형 number1 , number2를 계산 목적으로 integer 로 바꾸어 주는 것이지, number1 , number2 가 integer 형이 되는것은 아니다.  
{: .notice--info}

If you use `int()` on a floating point number, it will round the number down. To preserve the decimal, you can use `float()`:

```python
string_num = "7.5"
print int(string_num)
print float(string_num)
>>> 7
>>> 7.5
```

**설명:** [ Learn ]    
• 함수 int()를 사용하면 정수형 값으로 변경되어 반환된다.    
• 함수 float()를 사용하면 실수형 값으로 변경되어 반환된다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a variable called `product` that contains the result of multiplying the float value of `float_1` and `float_2`.

* Create a string called `big_string` that says:

```
The product was X
```
* with the value of product where the X is.

**설명:** [ Instruction ]     
• 변수 product 를 만들어라.    
• 그리고, 그 변수에 float_1 , float_2 곱한 값을 대입하라.  
• 변수 big_string 를 만들어라.    
• 그리고, 그 변수에 *The product was* + str(product) 를 대입하라.   
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can combine strings by casting the numerical value to a string and using the + operator:

```python
"I have " + str(18) + " dogs at home!"
```

**설명:** [ Hint ]    
• 변수 product 를 문자형으로 변환하라. 
{: .notice--info}


<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
float_1 = 0.25
float_2 = 40.0

product = float_1 * float_2
big_string = "The product was " + str(product)
```

**설명:** [ Solution ]     
• float type 변수 product 를 문자열 type 으로 변환 해주고 대입한다. 
{: .notice--info}



**결과**     
```
#skip 
```   

<br>
<br>    
<br>    
<p style="page-break-before: always;"></p>     
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 14. Review    

Great! So far we’ve looked at:

* Print statements
* How to create, modify, and use variables
* Arithmetic operations like addition, subtraction, division, and multiplication
* How to use comments to make your code easy to understand
* Different data types, including strings, ints, floats, and booleans
* Converting between data types



**설명:** [ Learn ]     
• 지금까지 1장 Python Syntax에서는     
• print 문 사용법    
• 변수 생성    
• 사칙연산    
• 주석처리    
• 데이터 종류(integer, float, string, boolean)    
• 테이터 type 변환을 공부하였다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Let's apply all of the concepts you have learned one more time!    

* Create a variable called `skill_completed` and set it equal to the string "Python Syntax".    

* Create a variable called `exercises_completed` and set it equal to `13`. Create another variable called `points_per_exercise` and set it equal to `5`.    

* Create a variable called `point_total` and set it equal to `100`.    

* Update `point_total` to be what it was before plus the result of multiplying `exercises_completed` and `points_per_exercise`.    

* Add a comment above your declaration of points_per_exercise that says:     

```
The amount of points for each exercise may change, because points don't exist yet    
```    
     
* Print a string to the console that says:    

```    
I got X points!
```    
    

with the value of `point_total` where `X` is.

**설명:** [ Instruction ]     
• 변수 skill_completed 에 문자열 *Python Syntax* 를 대입하라.     
• 변수 exercises_completed 에 13 을 대입하라.        
• 변수 points_per_exercise 에 5 를 대입하라.      
• 변수 point_total 에  100 을 대입하라.    
• 변수 point_total 에 변수 exercises_completed * points_per_exercise 곱한 결과 값을 더하라.     
• *The amount* 부터 *yet* 까지의 문자열을 주석 처리하라.     
• *I got X points!* 를 콘솔창에 출력하라.    
• 변수 X 값은 변수 point_total 값이다.
{: .notice--info}



<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

• You can add to a variable by using `+=`:

```python
total += number_to_add
```

• which is shorthand for:

```python
[new value of] total = [old value of] total + number_to_add
```
• You can cast a numerical variable to a string and then add it to another string:

```python
print("This is " + str(1) + " long string!")
>>> "This is 1 long string!"
```    

**설명:** [ Hint ]    
• += 기법을 사용하라. 
• 함수 str() 사용하여, 숫자를 문자열로 바꾸어 출력한다. 
{: .notice--info}


<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
skill_completed = "Python Syntax"
exercises_completed = 13
#The amount of points for each exercise may change, because points don't exist yet
points_per_exercise = 5
point_total = 100
point_total += exercises_completed * points_per_exercise

print("I got "+str(point_total)+" points!")
```

**설명:** [ Solution ]    
• 문자열, 정수형, 주석, += 연산, 사칙연산, 문자형 변환을 참조 하세요. 
{: .notice--info}

**결과**
```
I got 165 points!
```    

<p style="page-break-before: always;"></p>
<br>
