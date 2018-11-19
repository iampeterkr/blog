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
    
    
    
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

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

1. Using a print statement, output a message of your choosing to the terminal.   


**설명:** 1. `print` 문 을 사용하여 당신이 쓰고 싶은 문장을 컴퓨터에게 화면에 출력하도록 시켜라. 
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
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

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

1. Print something using Python 3's syntax.

**설명:** 1. `print` 문을 Python3 문법을 사용하여 출력 하라. 
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
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

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

1. Try adding your name to the print statement with the + operator so that this Python program prints "Hello [your_name]"


**설명:** `+` 를 사용하여 두개의 `String`을 연결하여 *Hello Hongkildong* 이 출력 하라. 
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
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

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



**설명:** ①쿼트(quotes)가 시작과 끝이 같지 않으면, Python은 `EOL` Error를 발생시킨다. 시작이 `'` 이면 끝도 `'`이어야 하면, 시작이 `"`이면, 끝도 `"` 이어야 한다. ② 문자열을 만들때, 양 끝을 쿼트(quotest)가 없으면 Python은 해당 문자열을 `print`와 같은 명령문으로 인식한다. 이런경우 해당 문자열이 명령어 리스트에 없으면 `NameError`를 발생시킨다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

1. We've written two print statements that will raise errors. One has mismatched quotes and the other has no quotes at all.

Fix the two print statements to successfully debug the program!

**설명:** 쿼트(quotes)를 잘못 적용하여 Error가 발생하는 Python 프로그램을 고쳐라.  
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
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

### 5. Variables

In Python, and when programming in general, we need to build systems for dealing with data that changes over time. That data could be the location of a plane, or the time of day, or the television show you're currently watching. The only important thing is that it may be different at different times. Python uses variables to define things that are subject to change.

```python
greeting_message = "Welcome to Codecademy!"
current_excercise = 5
```

In the above example, we defined a variable called `greeting_message` and set it equal to the string "Welcome to Codecademy!". It also defined a variable called `current_exercise` and set it equal to the number 5.




**설명:** 변수란? 문자열이나, 숫자를 저장하기 위한 상자 이름 이다. 우리는 `greeting_message`라는 변수를 만들고 거기에 *"Welcome to Codecademy!"* 라는 문자열을 저장하면, 해당 변수 `greeting_message`는 문자를 담은 변수가 된다. 
그리고 그 변수를 변수 `greeting_message`라고 부른다. 마찬가지로 우리는 숫자를 담기위한 `current_exercise`라는 변수를 만들고, 거기에 숫자 *5*를 담는다. `current_exercise`는 숫자를 담은 변수가 되고, 우리는 이를 변수 `current_exercise`라고 부른다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

1. Create a variable called `toodays_date` and assign a value that will represent today's date to that variable.

**설명:** 변수 `todays_date`를 만들고 이 변수에 오늘 날짜를 담아라.
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
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

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

1. Multiply two numbers together and assign the result to a variable called `product`.

**설명:** ①변수 `product`를 만들고 ② 변수 `product`에 2개의 숫자를 곱셈 하여라. 
{: .notice--info}

2. What is the remainder when 1398 is divided by 11? Save the results in a variable called remainder.   

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
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

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
1. We're trying to figure out how much it rained in the past year! Update the `annual_rainfall` variable to include the values from September to December.

**설명:** 우리는 작년에 얼마나 많은 비가 왔는지 계산 하려고 한다. `annual_rainfall` 변수에 9월 부터 12월까지의 비의 양을 값을 더하여라. 
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
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

### 8. 





**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    


**설명:** 
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

**설명:** ① `*` 는 곱셈 ② `%`는 나머지를 구하는 모듈(module) 이다. 
{: .notice--info}

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

### 9. 





**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    


**설명:** 
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

**설명:** ① `*` 는 곱셈 ② `%`는 나머지를 구하는 모듈(module) 이다. 
{: .notice--info}


<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

### 10. 





**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    


**설명:** 
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

**설명:** ① `*` 는 곱셈 ② `%`는 나머지를 구하는 모듈(module) 이다. 
{: .notice--info}


<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

### 11. 





**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    


**설명:** 
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

**설명:** ① `*` 는 곱셈 ② `%`는 나머지를 구하는 모듈(module) 이다. 
{: .notice--info}



<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

### 12. 





**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    


**설명:** 
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

**설명:** ① `*` 는 곱셈 ② `%`는 나머지를 구하는 모듈(module) 이다. 
{: .notice--info}



<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

### 13. 





**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    


**설명:** 
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

**설명:** ① `*` 는 곱셈 ② `%`는 나머지를 구하는 모듈(module) 이다. 
{: .notice--info}


<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<br>
PYTHON SYNTAX

### 14. 





**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    


**설명:** 
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

**설명:** ① `*` 는 곱셈 ② `%`는 나머지를 구하는 모듈(module) 이다. 
{: .notice--info}
