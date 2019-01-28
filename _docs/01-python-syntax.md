---
# layout : rchive
title: "Python Syntax"
permalink: /python-syntax/
excerpt: "We learn about Python Syntax."
last_modified_at: 2018-11-19T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
   
<hr style="border: solid 1px #dddddd ;">    
LESSON    

This lesson will introduce you to Python, a general-purpose, object-oriented interpreted language you can use for countless standalone projects or scripting applications.    


**설명:** [ 학습방향 ]     

이 장에서는 수많은 독립형 프로젝트와 스크립트 응용 프로그램에 사용할 수 있는 객체지향적 프로그램 언어 Python을 소개합니다.
{: .notice--info}     
     
 <hr style="border: solid 1px #dddddd ;">

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 1. Hello World!


If programming is the act of teaching a computer to have a conversation with a user, it would be most useful to first teach the computer how to speak. In Python, this is accomplished with the `print` statement.



accomplished with the print statement.
   

```python
print "Hello, world!"
print "Water—there is not a drop of water there! 
Were Niagara but a cataract of sand, would you travel 
your thousand miles to see it?"
```



A `print` statement is the easiest way to get your Python program to communicate with you. Being able to command this communication will be one of the most valuable tools in your programming toolbox.

**설명:** 우리가 배워야 할 첫번째 Python 문법은 `print` 문 이다. `print` 문 은 Python 프로그램이 컴퓨터와 대화하는것을 실질적으로 사람이 볼수 있게 해주는 도구이다. 상단 검정 박스안의 Python 소스를 **Coding** 창에 복사하여 실행(Run) 해 보자. 우리는 컴퓨터에게 *"Hellow World!"* 라는 문장을 화면에 출력 시키라고 명령한 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Using a print statement, output a message of your choosing to the terminal.   


**설명:** ① `print` 문 을 사용하여 당신이 쓰고 싶은 문장을 컴퓨터에게 화면에 출력하도록 시켜라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Print a message by typing `print` followed by your message in quotes, like this:

```python
print "Your Message!"
```


**설명:** `print` 문을 사용하여 *"Your Message!" 를 출력 한다. 
{: .notice--info}

<br>
<br>    
<br>   

----------------------
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 2. Print Statements

There are two different Python versions. Both Python 2 and Python 3 are used throughout the globe. The most significant difference between the two is how you write a print statement. In Python 3, print has parentheses.


```python
print("Hello World!")
print("Deep into distant woodlands winds a mazy way, reaching to overlapping spurs of mountains bathed in their hill-side blue.")
```   

In this course we will be using Python 2. If you go on to write Python 3 it will be useful to note this key difference.



**설명:** Python2 와 Python3는 문법이 조금 틀리다. 가장 크게 틀린 부분은 `print` 문을 사용시 `()` 를 사용하느냐 이다. 우리는 Python2 를 기본으로 배울 것이다. Python2와 Python3는 Python을 배우는데, 크게 차이는 없다. 그리고 Python version 3.x 이상은 Python2 문법도 모두 통용이 된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Print something using Python 3's syntax.

**설명:** ① `print` 문을 Python3 문법을 사용하여 출력 하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Remember to include parentheses!

```python
print("Your message!")
```


**설명:** Python3는 `print` 문을 사용시 `()` 가 필요하다.  
{: .notice--info}

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 3. String

When printing things in Python, we are supplying a text block that we want to be printed. Text in Python is considered a specific type of data called a string. A string, so named because they're a series of letters, numbers, or symbols connected in order — as if threaded together by string. Strings can be defined in different ways:

```python
print "This is a good string"
print 'You can use single quotes or double quotes for a string'
```    

Above we printed two things that are strings and then attempted to print two things that are not strings. While double-quotes (") and single-quotes (') are both acceptable ways to define a string, a string needs to be opened and closed by the same type of quote mark.

We can combine multiple strings using +, like so:

```python
print "This is " + "a good string"

This code will print out "This is a good string".
```


**설명:** 문자열을 Python 에서는 `String` 이라고 부른다. `String`은 `' '` 또는 `" "` 사이에 문자를 넣는다. 그리고 문자열은 여러 문자열을 위와 같이 `+` 를 사용하여 붙일수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Try adding your name to the print statement with the + operator so that this Python program prints "Hello [your_name]"


**설명:** ① `+` 를 사용하여 두개의 `String`을 연결하여 *Hello Hongkildong* 이 출력 하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

```python
print "Hello " + "Nicole"
```

**설명:** 우리는 두개의 `String`을 `+` 를 사용하여, 문장을 연결 할 수 있다. 
{: .notice--info}

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
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



**설명:** ① 쿼트(quotes)가 시작과 끝이 같지 않으면, Python은 `EOL` Error를 발생시킨다. 시작이 `'` 이면 끝도 `'`이어야 하면, 시작이 `"`이면, 끝도 `"` 이어야 한다. ② 문자열을 만들때, 양 끝을 쿼트(quotest)가 없으면 Python은 해당 문자열을 `print`와 같은 명령문으로 인식한다. 이런경우 해당 문자열이 명령어 리스트에 없으면 `NameError`를 발생시킨다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** We've written two print statements that will raise errors. One has mismatched quotes and the other has no quotes at all.

Fix the two print statements to successfully debug the program!

**설명:** ① 쿼트(quotes)를 잘못 적용하여 Error가 발생하는 Python 프로그램을 고쳐라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

A print statement should start with the word print and then should have the message inside matching quote marks.

```python
print 'This is a good print statement'
```   

Double quotes are also fine:

```python
print "This is also a good print statement"
```


**설명:** 문자열은 처음과 시작은 같은 쿼트(quotes)가 되어야 한다. 
{: .notice--info}

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
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




**설명:** 변수란? 문자열이나, 숫자를 저장하기 위한 상자 이름 이다. ① 우리는 `greeting_message`라는 변수를 만들고 거기에 *"Welcome to Codecademy!"* 라는 문자열을 저장하면, 해당 변수 `greeting_message`는 문자를 담은 변수가 된다. 
② 그리고 그 변수를 변수 `greeting_message`라고 부른다. 마찬가지로 우리는 숫자를 담기위한 `current_exercise`라는 변수를 만들고, 거기에 숫자 *5*를 담는다. `current_exercise`는 숫자를 담은 변수가 되고, 우리는 이를 변수 `current_exercise`라고 부른다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a variable called `toodays_date` and assign a value that will represent today's date to that variable.

**설명:** ① 변수 `todays_date`를 만들고 이 변수에 오늘 날짜를 담아라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

```python
todays_date = "March 31, 2023"
```


**설명:** 
{: .notice--info}
<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
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



**설명:** 컴퓨터의 많은 기능 중 하나는 계산하는 것이다. Python도 사칙연산(`+`,`−`,`×`,`÷`)를 지원한다. 다만, Python에선 `×`→ `*`, `÷` → `/` 로 표시한다.
이외에도 모듈(module)연산자도 지원한다. 모듈연산자 중 하나인 `%`는 나머지를 계산해준다.(ex: `15 % 2 = 1`, 만약 `133 % 7` 같이 딱 떨어지면 나머지는 `0`이다.  )
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Multiply two numbers together and assign the result to a variable called `product`.

**설명:** ①변수 `product`를 만들고 ② 변수 `product`에 2개의 숫자를 곱셈 하여라. 
{: .notice--info}

**②** What is the remainder when 1398 is divided by 11? Save the results in a variable called remainder.   

**설명:** ① `1398 / 11` 의 나머지는 무엇일까? 변수 `remainder`를 만들고 ② 변수 `reminder`에 `1397 / 11` 의 나머지 값을 저장하여라.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Remember creating a variable is as simple as setting it equal to something else. To define a variable called quotient you would write the following:

```python
quotient = 30 / 5
```

Remember that remainders can be found using the modulus operator. Calculate a remainder with `%`.

```python
1908 % 3
```

Will be `0` because `1908` is divisible by `3`.

**설명:** ①상기의 예는 변수 `quotient`에 두 수를 나눗셈 한 것이다.
② `%`는 나머지를 구하는 모듈(module) 이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
product = 18 * 13
remainder = 1398 % 11
```

**설명:** ① `*` 는 곱셈 ② `%`는 나머지를 구하는 모듈(module) 이다. 
{: .notice--info}

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
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

**설명:** ①각 변수 `fish_in_clarks_pond`, `number_of_fish_caught` `50`, `10`을 넣고, ② 변수 `fish_in_clarks_pond`에 `fish_in_clarks_pond` -  `number_of_fish_caught` 값을 넣는다. 
③ 이럴 경우, 변수 `fish_in_clarks_pond`에는 `50 - 10`의 값이 계산된 `40`이 저장된다.  
{: .notice--info}


```python
money_in_wallet = 40
sandwich_price = 7.50
sales_tax = .08 * sandwich_price

sandwich_price += sales_tax
money_in_wallet -= sandwich_price
```

In the above example, we use the price of a sandwich to calculate sales tax. After calculating the tax we add it to the total price of the sandwich. Finally, we complete the transaction by reducing our `money_in_wallet` by the cost of the sandwich (with tax).


**설명:** 위 예제는 샌드위치 세금을 계산하는 예를 들면서, 변수에 숫자를 곱하여도 사용할 수 있음을 보여준다. `+=` 연산자를 사용한 `sandwich_price += sales_tax` 는 `sandwich_price = sandwich_price + sales_tax` 와 같은 기능을 한다. 
물론 `-=` 연산자를 사용한 `money_in_wallet -= sandwich_price`는 `money_in_wallet = money_in_wallet - sandwich_price` 와 같은 기능을 한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    
**①** We're trying to figure out how much it rained in the past year! Update the `annual_rainfall` variable to include the values from September to December.

**설명:** ① 우리는 작년에 얼마나 많은 비가 왔는지 계산 하려고 한다. `annual_rainfall` 변수에 9월 부터 12월까지의 비의 양을 값을 더하여라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Use the += syntax to add a value to an existing variable:

```python
annual_rainfall += september_rainfall
```

Add all of the remaining months to


**설명:**  `+=` 모듈을 사용하여라.  
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

**설명:** ① `+=` 연산자를 사용하여 추가한다. ② 최종 `annual_rainfall`를 출력 한다. 
{: .notice--info}

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 8. Comments

Most of the time, code should be written in such a way that it is easy to understand on its own. However, if you want to include a piece of information to explain a part of your code, you can use the # sign. A line of text preceded by a # is called a comment. The machine does not run this code — it is only for humans to read. When you look back at your code later, comments may help you figure out what it was intended to do.

```python
# this variable counts how many rows of
the spreadsheet we have:
row_count = 13
```


**설명:** Python에서 프로그램으로 인식되지 않는 부분을 주석(Comment) 이라고 부르며, 이들의 사용 목적은 프로그램에 정보를 남겨두거나 설명하기 위해서이다. 주석 처리된 부분은 컴퓨터는 인식 못하고 오직 프로그램을 읽는 사람만이 인식한다. 주석을 만들때는 `#` 을 사용한다. 한줄 주석(Comment)은 `#`으로 처리한다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Add a comment above the declaration of `city_pop` with a description of what you think the variable contains.


**설명:** ① 변수 `city_pop` 위에 주석을 만들어라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** # 
{: .notice--info}   


<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
city_name = "St. Potatosburg"

# This number tracks the population count of the spudizens of St. Potatosburg
city_pop = 340000
```

**설명:**  **#** 을 사용하여, 변수 `city_pop`에 저장한 `34000`에 대한 설명을 남겨둔다.  
{: .notice--info}

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
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

You can also define a **float** using scientific notation, with e indicating the power of 10:

```python
# this evaluates to 150:
float4 = 1.5e2
```


**설명:** Python에서는 숫자 관련 변수는 정수(integer)와 실수(float)2종류가 있다. 정수는 소숫점 이하를 표현 할수 없으며, 실수는 소수점을 표현할 수 있다. 
생서하는 변수가 정수인지, 실수인지는 해당 값을 대입할때 정해진다. 즉, 변수에 정수를 넣으면 정수형 변수가 되고, 실수를 넣으면 실수형 변수가 된다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** You are going shopping. Let's make a grocery list so that you can plan your budget. Store the number of cucumbers you want to buy in a variable called `cucumbers`. Make sure it's at least `1`, and that it's the appropriate datatype! The store doesn't sell partial cucumbers.

**설명:** ① `cucumbers` 변수를 만들고, 정수 `1`을 대입하라.
{: .notice--info}

**②** Each cucumber costs 3.25 doubloons. Store the price per cucumber in a variable called price_per_cucumber.

**설명:** ② `price_per_cucumber` 변수를 만들고, `3.25`를 대입하라. 
{: .notice--info}

**③** Create a new variable called total_cost which is the product of how many cucumbers you are going to buy and the cost per cucumber.

**설명:**  ③ `total_cost` 변수를 만들고, 구매할 오이의 총 가격을 계산하라. 
{: .notice--info}

**④** Print out total_cost.
What datatype is it?

**설명:** ④ `total_cost` 를 `print` 명령어를 사용하여 출력하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** `*` 연산자를 사용하여 총 합을 계산하라. 
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

**설명:** ① `*` 을 이용하여 총합을 구합니다. Python은 정수와 실수의 곱을 자동으로 계산해 준다. 입력 된 두 값(`3`,`3.25`)중 하나(`3.25`)가 실수 이기에 Python은 내부적으로 그 계산 결과값은 실수로 계산되어지고, `total_cost`는 실수형 변수가 된다.  
{: .notice--info}


<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
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



**설명:** Python은 두수를 나누어 정수로 딱 떨어지면, 해당 변수를 정수형 변수로 인식한다. 그러나 입력된 값이 정수(`7/3`) 이면 그 계산한 결값이 실수이어도 정수(`3`)만 남고, 나머지는 `0.5`는 버려진다. 이런 실수를 방지하기 위하여 값을 대입할때, 계산한 결과 값이 실수 일 것을 대비하여야 한다. 입력값을 실수형으로 넣어주거나, 임의적으로 입력값을 `float(7)` 실수형 값으로 변경후 입력 후 계산 처리하면 이를 방지할 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** You have come home from the grocery store with 100 cucumbers to split amongst yourself and your 5 roommates (6 people total).

Create a variable cucumbers that holds 100 and num_people that holds 6.

**설명:**  100개의 오이를 룸메이트 6명과 나눠 가질려고 한다. 
①`cucumbers`변수를 만들고 값 `100`을 대입하고, 변수 `num_people`를 만들고 값 `6`을 대입하라.
{: .notice--info}

**②** Create a variable called whole_cucumbers_per_person that is the integer result of dividing cucumbers by num_people.

Print whole_cucumbers_per_person to the console.

**설명:** ② 변수 `whole_cucumbers_per_person` 에 `cucumbers` / `num_people` 한 값을 계산한후 그 결과값을 출력하라. 
{: .notice--info}


**③** You realize that the numbers don't divide evenly and you don't want to throw out the remaining cucumbers. Create a variable called float_cucumbers_per_person that holds the float result of dividing cucumbers by num_people.

Print float_cucumbers_per_person to the console.

**설명:** `100/6` 의 계산값은 `16.66...` 으로 예상했지만, ② 결과에서 `16`만 출력 되는것을 볼 것이다. ③ `float_cucumbers_per_person` 변수를 만들고, 이변수에 실수 값이 출력 될수 있도록 만들어라. 그리고 출력하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can do float division by casting either the numerator or denominator as a float:

```python
quotient_with_decimals = float(5)/2
#yields 2.5
```

**설명:** `float()` 함수를 사용하여라. 
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

**설명:** `float_cucumbers_per_person` 변수를 계산할때, `float()`함수를 사용하여 `float(cucumbers)`를 실수로 변경하여 계산한다.  
{: .notice--info}

**출력**
```
16
16.6666666667
```


<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
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




**설명:** `""" """` or `''' '''` 를 이용하여 여러줄의 문자열을 만들수 있다.
이는 문자열도 만들수 있지만, 한 줄 주석(`#`)외에 여러줄의 주석을 만들때도 사용한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a variable called `haiku` and store this haiku as a multi-line string: The old pond, A frog jumps in: Plop!

**설명:** ① 변수 `haiku`를 만들고, `The old pond, A frog jumps in: Plop!` 여러줄의 문자열을 대입하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** `""" """` or `''' '''` 를 사용 하여라. 
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

**설명:** `""" """` 사용하여 여러줄의 문자열을 변수에 대입한다.  
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
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
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


**설명:** Python에서 `참`, `거짓`을 표현해야 할 때가 있다. `참`은 문자열로 `True`로 표현하고, `거짓`은 문자열로 `False`로 표현한다. 그리고 `참`의 값은 숫자 `1` 이고,  `거짓`의 값은 숫자  `0` 이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    
**①** Someone has introduced themselves to you using comments in script.py.

Read the comments and then create a variable called `age_is_12` and set it to be `True` or `False` depending on if this person's age is 12.

**설명:** ① 변수 `age_is_12`를 만들고, 주석에서 설명하는 사람의 나이가 12살이면 `True`, 그렇지 않으면 `False`를 입력하라. 
{: .notice--info}

**②** Create a variable called `name_is_maria` and set it to be `True` or `False` depending on if this person's name is Maria.

**설명:** ② 변수 `name_is_maria`를 만들고, 주석에서 설명하는 사람의 이름이 Maria 이면 `True`, 그렇지 않으면 `False`를 입력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

To set a boolean to True, you would use:

```python
some_variable = True
```
**설명:** 주석 문을 읽고 `True`, `False`를 이용하여 대입하라. 
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

**설명:** 주석에서 Python coder 나이는 21살, 이름은 Maria 이다.  
{: .notice--info}



<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
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
**설명:** 변수 `age`가 정수 `13`이 대입되어 정수형 변수이다. 이를 `str()` 함수를 사용하여 `str(age)`로 바꾸면 이는 **string** 형으로 바뀌게 된다. *주의)* 정수형 `age`를 출력 할때 **string** 형태로 출력하는 것이지, `age`가 **string**형이 되는것은 아니다.  
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
**설명:** 변수 `number1, number2`는 문자형 변수이다. Python 에서는 문자형 데이타 이지만, 데이타가 숫자 이면 계산을 할수가 있다. 단, 계산할때, `int()`함수를 사용하여 정수형으로 바꾸어 주어야 한다. *주의)* 문자형 `number1, number2`를 계산 목적으로  **integer** 로 바꾸어 주는 것이지, `number1, number2`가 **integer**형이 되는것은 아니다.  
{: .notice--info}

If you use `int()` on a floating point number, it will round the number down. To preserve the decimal, you can use `float()`:

```python
string_num = "7.5"
print int(string_num)
print float(string_num)
>>> 7
>>> 7.5
```

**설명:** `int()` 함수를 사용하면 정수형 이 되고, `float()`를 사용하면 실수형 모양이 된다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a variable called `product` that contains the result of multiplying the float value of `float_1` and `float_2`.

**설명:** ① 변수 `product`를 만들고 거기에 `float_1`, `float_2` 곱한 값을 대입하라.  
{: .notice--info}

**②**Create a string called `big_string` that says:

The product was X
with the value of product where the X is.
<br>
<hr/>

**설명:** ② 변수 `big_string`를 만들고 거기에 "with the value of product where the `X` is." `X` 자리에는 `product` 값이 출력 되게 하라.    
{: .notice--info}


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can combine strings by casting the numerical value to a string and using the + operator:

```python
"I have " + str(18) + " dogs at home!"
```

**설명:** `product`를 문자 데이타형으로 변환하라. 
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

**설명:** **float** 데이타형인 `product`를 **string** 형으로 변환해주고 대입한다. 
{: .notice--info}


<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
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



**설명:** 지금까지 1장 Python Syntax에서는 `print`문 **사용법**, **변수 생성**, **사칙연산**, **주석처리**, **데이터 종류(integer, float, string, boolean)환**, **테이타 형변환** 을 공부하였다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Let's apply all of the concepts you have learned one more time!

Create a variable called `skill_completed` and set it equal to the string "Python Syntax".

**설명:** ① 변수 `skill_completed` 에 "Python Syntax"를 대입 하시오. 
{: .notice--info}

**②** Create a variable called `exercises_completed` and set it equal to `13`. Create another variable called `points_per_exercise` and set it equal to `5`.

**설명:** 
② 변수 `exercises_completed` 에 `13`을 대입하고, 변수 `points_per_exercise` 에 값 `5`를 대입 하시오.  
{: .notice--info}

**③** Create a variable called `point_total` and set it equal to `100`.

**설명:**  
③ 변수 `point_total` 에 값 `100`을 대입 하시오.
{: .notice--info}


**④** Update `point_total` to be what it was before plus the result of multiplying `exercises_completed` and `points_per_exercise`.

**설명:**  
④ 변수 `point_total` 에 변수 `exercises_completed` * `points_per_exercise` 곱한 결과값을 더하라. 
{: .notice--info}

**⑤** Add a comment above your declaration of points_per_exercise that says:
```
The amount of points for each exercise may change, because points don't exist yet
```
**설명:**  
⑤ The amount 부터 yet 까지의 문자열을 주석 처리 하라.   
{: .notice--info}


**⑥** Print a string to the console that says:

```
I got X points!
```

with the value of `point_total` where `X` is.

**설명:**  
⑥ The amount 부터 yet 까지의 문자열을 주석 처리 하라.   
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

④ You can add to a variable by using +=:

```python
total += number_to_add
```

which is shorthand for:

```python
[new value of] total = [old value of] total + number_to_add
```

**설명:** ④ `+=` 기법을 사용하라. 
{: .notice--info}


⑥ You can cast a numerical variable to a string and then add it to another string:

```python
print("This is " + str(1) + " long string!")
>>> "This is 1 long string!"
```

**설명:** ⑥ `str()` 사용하여, 숫자를 문자열로 바꾸어 출력한다. 
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

**설명:** 문자열, integer, 주석, `+=` 연산, 사칙연산, 문자형 변환을 참조 하세요. 
{: .notice--info}

**결과**
```
I got 165 points!
```
