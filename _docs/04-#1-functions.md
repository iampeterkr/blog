---
# layout : rchive
title: "Functions"
permalink: /functions/
excerpt: "We learn about Functions Syntax."
# last_modified_at: 2018-12-04T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---


<hr style="border: solid 1px #dddddd ;">    

LESSON    

A function is a reusable section of code written to perform a specific task in a program. We gave you a taste of functions in Unit 3; here, you'll learn how to create your own.

**설명:** [ 학습방향 ]     
이 장에서는 함수에 대해서 기본적으로 배웁니다.    
함수는 프로그램 내에서 특정 작업을 수행 하도록 만들어진 재사용 가능한 코드이다.
{: .notice--info}     
     
    
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 
### 1. What Good are Functions?    

You might have considered the situation where you would like to reuse a piece of code, just with a few different values. Instead of rewriting the whole code, it's much cleaner to define a *function*, which can then be used repeatedly.


**설명:** [ Learn ]    
• Ch1. What Good are Functions? 에서는 함수의 필요성을 학습한다.     
• 자주 사용되는 기능은 반복적으로 사용하게 된다.    
• 이런경우, 매번 만들것이 아니라, 해당 기능을 함수로 만들어 놓고 재 사용한다.       
• 코딩중 해당 기능이 필요시 불러서 재 사용하는 것이 현명하다.
{: .notice--info}




![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the code in the editor.     
* If you completed the Tip Calculator lesson, you'll remember going through and calculating `tax` and `tip` in one chunk of program.     
* Here you can see we've `def`ined two functions: `tax` to calculate the tax on a bill, and `tip` to compute the tip.

<p style="page-break-before: always;"></p>
<br>

* See how much of the code you understand at first glance (we'll explain it all soon).     
* When you're ready, click Run to continue.



**설명:** [ Instruction ]     
• Editor 화면에 구현되어 있는 함수 tax() 와, 함수 tip() 를 해석해 보자.    
• 참고로, 함수 tax() 는 세금을 계산해 주고, 함수 tip() 은 팁을 계산해주는 함수이다.    
• 각 함수가 어떻게 작동 되는지를 이해해 보자.    
• 그리고 실행해 보고, 당신이 생각한대로 동작 되는지 확인해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Remember how we used `%s` to print strings? We can use `%f` to print floats! (That is, numbers with decimals in them.)

**설명:** [ Hint ]    
• %s 는 문자열을 출력할때, %f 는 실수를 출력할때 사용한다. 
{: .notice--info}

<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def tax(bill):
  """Adds 8% tax to a restaurant bill."""
  bill *= 1.08
  print "With tax: %f" % bill
  return bill

def tip(bill):
  """Adds 15% tip to a restaurant bill."""
  bill *= 1.15
  print "With tip: %f" % bill
  return bill
  
meal_cost = 100
meal_with_tax = tax(meal_cost)
meal_with_tip = tip(meal_with_tax)
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 변수 meal_cost 에 100 을 대입한다.    
• 함수 tax() 에 변수 meal_cost 를 대입하여 호출한다.    
• 변수 meal_with_tax 에 함수 tax() 를 호출한 결과값을 저장한다.    
• 함수 tip() 에 변수 meal_with_tax 를 대입하여 호출한다.    
• 변수 meal_with_tip 에 함수 tip() 호출한 결과값을 저장한다.
{: .notice--info}


**결과** 
``` 
With tax: 108.000000
With tip: 124.200000
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 2. Function Junction    

Functions are defined with three components:

1. The header, which includes the def keyword, the name of the function, and any parameters the function requires. Here's an example:

```python
def hello_world(): # There are no parameters
```

**설명:** [ Learn ]    
• Ch2. Function Junction 에서는 함수의 구성 요소를 학습한다.      
• 함수를 사용하기 위해선 크게 3 단계의 절차로 진행된다.    
• 함수 정의 절차는 다음과 같다.         
• - def 함수를 선언한다.    
• - 함수 이름을 선언한다.    
• - 함수 인자를 가진다.
{: .notice--info}


2. An optional comment that explains what the function does.

```python
"""Prints 'Hello World!' to the console."""
```

**설명:** [ Learn ]     
• 함수가 하는 기능을 문자열 주석( """ """ ) 처리한다.    
{: .notice--info}


3. The body, which describes the procedures the function carries out. The body is indented, just like conditional statements.

```python
print "Hello World!"
```
* Here's the full function pieced together:

```python
def hello_world():
  """Prints 'Hello World!' to the console."""
  print "Hello World!"
```

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Learn ]     
• 함수가 처리할 기능을 구현한다.     
• 정의된 함수 def hello_world() 는 인자가 없다.    
• 이 함수는 문자열 "Hello world" 를 출력한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Go ahead and create a function, spam, that prints the string "Eggs!" to the console. Don't forget to include a comment of your own choosing (enclose it in triple quotes!).


**설명:** [ Instruction ]     
• 함수 spam 을 작성하라.    
• 함수 spam 은  "Eggs!" 를 출력하는 기능을 한다.    
• 함수 spam 이 무슨 기능을 하는지 주석( """ """ )을 사용하여 설명한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* If you're stuck, look closely at the example function syntax in the instructional text. Remember: whitespace counts in Python!


**설명:** [ Hint ]     
• 앞장의 함수를 구성하는 3단계를 다시 학습해보자.     
• 함수를 선언할때, 함수 끝에 ( : ) 를 주의 하자. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Define your spam function starting on line 5. You
# can leave the code on line 10 alone for now--we'll
# explain it soon!

def spam():
  """Prints 'Eggs!'"""
  print "Eggs!"

# Define the spam function above this line.
spam()

```

**설명:** [ Solution ]    
• 함수 spam(): 을 선언한다.    
• 함수 spam 내부에 어떤 기능을 처리 하는지를 주석 처리한다.    
• 함수 spam 기능, 즉 "Eggs!" 를 출력하는 기능을 구현한다. 
{: .notice--info}


**결과** 
```
Eggs!
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 3. Call and Response    

After defining a function, it must be *called* to be implemented. In the previous exercise, **spam()** in the last line told the program to look for the function called **spam** and execute the code inside it.

 
**설명:** [ Learn ]     
• Ch3. Call and Response 에서는 함수 호출을 학습한다.     
• 함수를 사용하기 위해선, 먼저 함수 선언을 해야 한다.    
• 함수 선언이 되어 있으면, 해당 함수를 호출 할수 있다.    
• 함수는 호출을 받으면, 해당 함수가 실행되고, 실행 결과값을 처음 호출한 곳으로 반환한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* We've set up a function, `square`.    
* Call it on the number `10` (by putting 10 between the parentheses of `square()`) on line 10!


**설명:** [ Instruction ]    
• 함수 square() 를 호출하라.     
• 호출할때, 인자 값으로 10 을 준다.    
• e.g. square(10)
{: .notice--info}




![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember when we called `spam` in the previous exercise,    
* like this: `spam()`    
* You can do the same here with `square()`, only you'll need to put `10` in between the parentheses so square knows what number to... well, square.  

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]    
• 앞에서 배운 함수 spam() 은 함수를 호출할때 인자값 없이 호출 하였다.    
• 이 장에서는 인자값을 괄호 사이에 주어 함수를 호출한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def square(n):
  """Returns the square of a number."""
  squared = n ** 2
  print "%d squared is %d." % (n, squared)
  return squared
  
# Call the square function on line 10! Make sure to
# include the number 10 between the parentheses.

square(10)
```

**설명:** [ Solution ]   
• 함수 square(n) 를 정의한다.     
• 함수 square(n) 는 parameter 값으로 n 을 입력 받는다.     
• 함수 square(n) 는 입력 받은 값 n 을 제곱 한다.    
• 함수 square(n) 는 입력값 n 과 결과값 squared 를 출력한다.    
• 함수 square(n) 는 결과값 squared 를 반환한다.
{: .notice--info}



**결과** 
``` 
10 squared is 100.
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 4. Parameters and Arguments    

Let's take another look at the definition of the function square from the previous exercise:

```python
def square(n):
```
Here, `n` is a **parameter** of square. A parameter is a variable that is an input to a function. It says, "Later, when square is used, you'll be able to input any value you want, but for now we'll call that future value `n`." A function can have any number of parameters.

The values of the parameters passed into a function are known as the **arguments**. Recall in the previous example, we called:

```python
square(10)
```
Here, the function square was called with the **parameter** `n` set to the **argument** `10`.

Typically, when you call a function, you should pass in the same number of arguments as there are parameters.

To summarize:

When defining a function, placeholder variables are called parameters.
When using, or calling, a function, inputs into the function are called arguments.


**설명:** [ Learn ]      
• Ch4. Parameters and Arguments 에서는 Parameter와 Arguments를 학습한다.     
• 함수 square(n) 에서 n 은 parameter 라고 부른다.    
• 함수 square(10) 호출 할때, 값 10 을 arugument 라고 부른다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the function in the editor, `power`.    
* It should take two **arguments**, a base and an exponent, and raise the first to the power of the second.     
* It's currently broken, however, because its **parameters** are missing.

* Replace the `___s` with the **parameters** base and exponent and then call the `power` function with a base of `37` and an exponent of `4`.

**설명:** [ Instruction ]   
• 함수 power 가 어떻게 동작 되는지를 먼저 확인한다.        
• 함수 power 는 2개의 parameter 를 가진다.     
• e.g. def power(base, exponent):    
• e.g. 37^4 = 1874161 ( 37의 4 승 )    
• e.g. base : 37, exponent : 4    
• 함수 power(37 , 4) = 1874161
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Make sure to include the parameters base and exponent between the parentheses on line 1, and the arguments 37 and 4 between the parentheses on line 5.     
* Your parameters and arguments need to be separated by a comma, like this: (base, exponent).


**설명:** [ Hint ]    
• base : 37    
• exponent : 4    
• def power(base, exponent): 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def power(base, exponent):  # Add your parameters here!
  result = base ** exponent
  print "%d to the power of %d is %d." % (base, exponent, result)

power(37, 4)  # Add your arguments here!
```

**설명:** [ Solution ]    
• 함수 power(37, 4)에 2개의 arguments로 37, 4를 입력하여 호출한다.    
• 함수 power(base, exponent)에 정의된 parameter에 값이 전달된다.    
• 파라미터 base = 37, exponent = 4 에 값이 전달된다.     
• 거듭 제곱 공식인 37 ** 4 의 결과값이 출력된다.
{: .notice--info}



**결과** 
``` 
37 to the power of 4 is 1874161.
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 5. Functions Calling Functions    

We've seen functions that can print text or do simple arithmetic, but functions can be much more powerful than that. For example, a function can call another function:

```python
def fun_one(n):
  return n * 5

def fun_two(m):
  return fun_one(m) + 7
```


**설명:** [ Learn ]      
• Ch 5. Functions Calling Functions 에서는 함수가 함수를 호출하는것을 학습한다.    
• 함수는 단순히 계산하고, 출력하는것 기능 외에도, 함수가 함수를 호출할 수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Let's look at the two functions in the editor: `one_good_turn` (which adds `1` to the number it takes in as an argument) and `deserves_another` (which adds `2`).

* Change the body of `deserves_another` so that it always adds `2` to the output of `one_good_turn`.


**설명:** [ Instruction ]    
• Editor 화면에 함수 2개가 있다.    
• e.g. 함수 one_good_turn(), deserves_another().    
• 함수 one_good_turn(n) 은 parameter 1개인 n 을 받는다.    
• 함수 one_good_turn(n) 은 n 값에 + 1 결과를 반환한다.    
• 함수 deserves_another(n) 는 parameter 1개인 n 을 받는다.    
• 함수 deserves_another(n) 는 n 값에 + 2 결과를 반환한다.    
• 함수 deserves_another(n) 를 다음과 같이 변경하라.    
• 함수 one_good_turn(n) 값에 + 2 결과를 반환하는 프로그램으로 변경하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* The n in the body of deserves_another should be replaced by a call to the function `one_good_turn(n)`.

**설명:** [ Hint ]   
• 함수 deserves_another(n) 의 return 문을 변경한다.    
• return 문의 변수 n 자리에 함수 one_good_turn(n)를 넣어라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def one_good_turn(n):
  return n + 1
    
def deserves_another(n):
  return one_good_turn(n) + 2
```

**설명:** [ Solution ]    
• 함수 deserves_another(n) 의 return 문에서, 함수 one_good_turn(n)을 호출한다.     
• 함수 one_good_turn(n) 결과값에 + 2를 한 결과값을 반환한다.
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
<font size="3"  face="돋움">FUNCTIONS</font> 

### 6. Practice Makes Perfect    

Let's create a few more **functions** just for good measure.

```python
def shout(phrase):
  if phrase == phrase.upper():
    return "YOU'RE SHOUTING!"
  else:
    return "Can you speak up?"

shout("I'M INTERESTED IN SHOUTING")
```

The example above is just there to help you remember how functions are structured.

Don't forget the **colon** at the end of your function definition!

**설명:** [ Learn ]      
• Ch6. Practice Makes Perfect 에서는 함수를 조건문에 따라 호출하는법을 학습한다.    
• 함수를 어떻게 호출하고 처리 되는지 다시한번 상기하자.     
• 함수 뒤에 ( : ) 을 생략하지 않도록 주의하자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* First, def a function called `cube` that takes an **argument** called `number`.     
* Don't forget the parentheses and the **colon**!

**설명:** [ Instruction ]    
• 함수 cube() 를 작성하라.    
• 함수 cube(number) 는 parameter 로 number 를 가진다.    
• 함수 cube(number): 끝에 ( : ) 를 생략하지 않도록 주의하라.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

* Make that function return the `cube` of that `number` (i.e. that number multiplied by itself and multiplied by itself once again).


**설명:** [ Instruction ]     
• 함수 cube(number) 를 작성하라.    
• 함수 cube(number) 는 number 의 argument 값을 다음과 같이 계산한다.    
• 받은 number 의 값을 세번 곱한 결과값(number * number * number)을 반환한다.   
• 함수 cube(number) 끝에는 ( : ) 를 생략하지 않도록 주의한다.
{: .notice--info}

* Define a second function called `by_three` that takes an argument called `number`.

**설명:** [ Instruction ]    
• 함수 by_three(number) 를 작성하라.   
• 함수 by_three(number) 는 parameter로 number 를 가진다.  
{: .notice--info}

* if that `number` is divisible by `3`, `by_three` should call `cube(number)` and return its result. Otherwise, `by_three` should return **False**.

**설명:** [ Instruction ]    
• 함수 by_three(number) 는 다음과 같이 동작한다.    
• 3 으로 나누어 떨어지면 함수 cube(number) 를 호출한다.    
• 그리고 그 결과값을 출력한다.    
• 3 으로 나누어 떨어지지 않으면, False를 반환한다. 
{: .notice--info}

* Don't forget that `if` and `else` statements need a `:` at the end of that line!

**설명:** [ Instruction ]    
• if 문과 else 문의 끝에는 꼭 ( : ) 가 존재한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
if n % 3 == 0:
  print "n is divisible by 3"
else:
  print "n is not"
```    
<p style="page-break-before: always;"></p>
<br>

* Make sure both functions return their values rather than printing them.

* Both branches of the `if/else` statement in `by_three` need to have return statements in them (that's three returns total, two for `by_three` and one for `cube`).

**설명:** [ Hint ]    
• 연산자 ( % ) 를 사용하여 함수의 기능을 처리하라.    
• if, else 문의 끝에는 항상 ( : ) 가 있어야 한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def cube(number):
  return number * number * number

def by_three(number):
  if number % 3 == 0:
    return cube(number)
  else:
    return False
```

**설명:** [ Solution ]   
• 함수 by_three(number) 는 다음과 같이 처리한다.        
• if 문에서는 number 에 전달된 값이 3 으로 나누어 떨어지면, 함수 cube()를 호출한다.    
• 그리고, 그 결과값을 반환한다.    
• else 문에선 number 에 전달된 값이 3으로 나누어 떨어지지 않으면 False 를 반환한다.
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
<font size="3"  face="돋움">FUNCTIONS</font> 

### 7. I Know Kung Fu    

Remember `import` this from the first exercise in this course? That was an example of importing a module. A module is a file that contains definitions—including variables and functions—that you can use once it is imported.



**설명:** [ Learn ]      
• Ch7. I Know Kung Fu 에서는 import 모듈을 학습한다.    
• 모듈 import 는 미리 만들어진 변수, 함수들을 묶어둔 것이다.    
• 명령어 import 는 이것들을 호출하여 사용하는 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Before we try any fancy importing, let's see what **Python** already knows about square roots. On line 3 in the editor, ask Python to

```python
print sqrt(25)
```
* which we would expect to equal five.

* Instead, it throws an error.


**설명:** [ Instruction ]    
• Python에서는 미리 만들어 놓은 함수들을 묶어서 정의해 둔 것이 있다.     
• 그 중 예를 하나 들면, 함수 sqrt() 이다.     
• e.g. 함수 sqrt(5), argument 값 5 의 루트 값을 구하는 함수이다.    
• Editor 화면 3 라인에서 함수 sqrt(25) 를 호출해보자.    
• 예상한대로, 값 루트 5가 계산되어 반환되는가?    
• 예상과 달리, error 가 발생한다.     
• Editor 화면에서 시도해 보라.   
{: .notice--info}


<p style="page-break-before: always;"></p>
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
# Ask Python to print sqrt(25) on line 3.

print sqrt(25)
```

**설명:** [ Solution ]    
• 함수 sqrt(25)의 결과 값을 출력하면 Error 가 발생한다.    
• 이유는 함수 sqrt() 를 사용할수 있게 해주는 import 가 선언되지 않았기 때문이다.
{: .notice--info}



**결과** 
``` 
Traceback (most recent call last):
  File "python", line 3, in <module>
NameError: name 'sqrt' is not defined
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 8. Generic Imports     

Did you see that? Python said: **NameError: name 'sqrt' is not defined**. Python doesn't know what square roots are—yet.

There is a Python module named math that includes a number of useful variables and functions, and `sqrt()` is one of those functions. In order to access math, all you need is the import keyword. When you simply import a module this way, it's called a generic `import`.


**설명:** [ Learn ]      
• Ch8. Generic Imports 에서는 Import 를 계속 학습한다.    
• 다음 Error 는 해당 함수를 본문에서 사용했지만, 그 함수를 찾지 못했을 경우 발생한다.    
• e.g. NameError: name 'sqrt' is not defined    
• Python 은 각종 수학 관련 함수들을 모아 놓은 모듈들의 묶음이 있다.    
• 이 모듈에는 함수 sqrt() 도 속해 있다.    
• 함수 sqrt() 와 같은 함수들을 우리는 직접 구현하지 않고 사용할 수 있다.    
• import 문을 사용하여, 정의해 놓으면 사용할 수 있다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* You'll need to do two things here:

  * Type `import math` on line 2 in the editor.    
  * Insert `math`. before `sqrt()` so that it has the form `math.sqrt()`.     
  * This tells Python not only to `import math`, but to get the `sqrt()` function from within `math`.     
  * Then hit `Run` to see what Python now knows.

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]    
• 아래와 같이 2가지 작업을 실행하라.    
• 첫번째, 2번 라인에 import math 를 선언한다.    
• 함수 sqrt() 를 사용하기 위해선 다음과 같이 모듈 math의 sqrt()를 선언해야 한다.    
• e.g. import math.sqrt()    
• 그리고 함수 sqrt()를 사용해야 한다.    
• Run 실행하라. 
{: .notice--info}




<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Make sure you  `import math` (no colons or anything like that), and make sure you ask Python to print `math.sqrt(25)`.

**설명:** [ Hint ]   
• import math 를 선언하여 math 모듈을 불러온다.    
• 모듈 math 의 함수 sqrt()를 사용한다.    
• e.g. math.sqrt(25)
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Ask Python to print sqrt(25) on line 3.
import math
print math.sqrt(25)

```

**설명:** [ Solution ]    
• 수학 관련 내장된 함수를 사용하기 위해선, import math 를 선언한다.    
• 사용 방법은 아래 예와 같다.    
• e.g. math.sqrt(25) 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>

**결과** 
``` 
5.0
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 9. Function Imports    

Nice work! Now Python knows how to take the square root of a number.

However, we only really needed the sqrt function, and it can be frustrating to have to keep typing `math.sqrt()`.

It's possible to import only certain variables or functions from a given module. Pulling in just a single function from a module is called a function import, and it's done with the `from` keyword:

```python
from module import function
```
Now you can just type `sqrt()` to get the square root of a number.     no more `math.sqrt()`!





**설명:** [ Learn ]     
• Ch9. Function Imports 에서는 함수명을 Imports 하는것을 학습한다.     
• 함수 sqrt()를 사용하기 위해선, import math 를 선언해줘야 한다고 이미 배웠다.    
• 그리고 math.sqrt() 를 사용했다.    
• math.sqrt() 를 사용할 수도 있지만, 다른 방법도 있다.    
• import 선언시 좀더 구체적으로 math 모듈에 대하여 자세히 선언해 주면 된다.    
• e.g. from moudle import sqrt     
• 이렇게 선언하면, math.sqrt() 라고 쓰지않고 단순히 sqrt() 만 사용할 수 있다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Let's import only the `sqrt` function from `math` this time. (You don't need the `()` after `sqrt` in the `from math import sqrt` bit.)


**설명:** [ Instruction ]    
• from math import sqrt 에서 함수 sqrt 뒤에 '()'를 안붙여 줘도 된다.     
• 함수 sqrt 를 선언해 보자. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Remember: from module import function! (Don't include the parentheses here—just the function name, e.g. sqrt.)

**설명:** [ Hint ]    
• from moudle import sqrt 로 선언한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from math import sqrt
```

**설명:** [ Solution ]    
• 모듈 math 에서 함수 sqrt 를 사용 하겠다는 것을 명확하게 선언해 준다. 
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
<font size="3"  face="돋움">FUNCTIONS</font> 

### 10. Universal Imports    

Great! We've found a way to handpick the variables and functions we want from modules.

What if we still want all of the variables and functions in a module but don't want to have to constantly type math.?

Universal import can handle this for you. The syntax for this is:

```python
from module import *
```

**설명:** [ Learnn ]      
• Ch10. Universal Imports 에서는 함수 선언을 * 로 활용하는 법을 학습한다.    
• 우리는 from 명령어를 사용하여 원하는 모듈을 콕 찝어서 사용할 수 있다.    
• 반대로, 여러 함수를 다양하게 사용할 수 있도록 선언도 할 수 있다.    
• math. 의 ( . ) 도 필요 없고, 다양하게 사용하려면 다음 예와 같이 하면 된다.    
• ( * ) 를 활용하여 다음과 같이 선언하면 된다.    
• e.g. from module import *
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Use the power of `from module import *` to import everything from the math module on line 3 of the editor.


**설명:** [ Instruction ]     
• from module import * 를 사용하여라.    
• 라인 3 에 모듈 math 를 사용할 수 있게 import 를 선언해라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

```python
Just like this: from math import *
```
**설명:** [ Hint ]    
• from math import *  를 사용하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Import *everything* from the math module on line 3!

from math import *
```

**설명:** [ Solution ]    
• math 모듈의 모든 함수/변수 기능을 사용하겠다고 선언하였다.
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
<font size="3"  face="돋움">FUNCTIONS</font> 

### 11. Here Be Dragons    

Universal imports may look great on the surface, **but they're not a good idea for one very important reason** : they fill your program with a ton of variable and function names without the safety of those names still being associated with the module(s) they came from.

If you have a function of your very own named `sqrt` and you `import math`, your function is safe: there is your sqrt and there is `math.sqrt`. If you do `from math import *`, however, you have a problem: namely, two different functions with the exact same name.

Even if your own definitions don't directly conflict with names from imported modules, if you import * from several modules at once, you won't be able to figure out which variable or function came from where.

For these reasons, it's best to stick with either import module and type module.name or just import specific variables and functions from various modules as needed.


<br>
<br>

**설명:** [ Learn ]      
• Ch11. Here Be Dragons 에서는 함수 모듈을 확인하는 함수 dir()을 학습한다.    
• ( * )를 사용하여 해당 모듈의 모든것을 가져오기에 정말 편리해 보인다.    
• 그러나 단점도 있다.     
• ( * ) 를 사용하면, 해당 모듈에 대한 모든것을 가져온다.    
• 만약, 내가 만든 모듈이 Python 내부에서 제공하는 모듈과 이름이 같으면 어떻게 될까?     
• Python은 혼돈이 올것이다.     
• 지금 실행되는 함수 sqrt() 가 내가 작성한 함수인지 ?  
• 아니면 모듈 math 에서 제공하는 함수 sqrt() 인지를 알수가 없다.     
• 이러한 이유로, 우리는 좀더 정확하게 선언을 해야 한다.    
• 내가 만든 함수는 me.sqrt() 로 표현한다.    
• Python 모듈 math 가 제공하는 함수는 math.sqrt() 로 표현한다.    
• 이렇게 하는것이 프로그램 오류를 줄일 수 있는 방법이다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* The code in the editor will show you everything available in the **math** module.

* Click `Run` to check it out (you'll see `sqrt`, along with some other useful things like `pi`, `factorial`, and `trigonometric` functions.

**설명:** [ Instruction ]   
• Editor 화면에 있는 소스를 실행 시켜보자.    
• Python 모듈 math 에는 어떤 함수들이 포함되어 있는지 확인해 보자. 
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
import math # Imports the math module
everything = dir(math) # Sets everything to a list of things from math
print everything # Prints 'em all!
```

**설명:** [ Solution ]    
• Python 모듈 math 에 속해 있는 모든 함수들을 보여준다.    
• 함수 dir(math) 를 사용하면 볼 수 있다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>


**결과** 
``` 
['__doc__', '__name__', '__package__', 'acos', 'acosh', 'asin', 'asinh', 'atan', 'atan2', 'atanh', 'ceil', 'copysign', 'cos', 'cosh', 'degrees', 'e', 'erf', 'erfc', 'exp', 'expm1', 'fabs', 'factorial', 'floor', 'fmod', 'frexp', 'fsum', 'gamma', 'hypot', 'isinf', 'isnan', 'ldexp', 'lgamma', 'log', 'log10', 'log1p', 'modf', 'pi', 'pow', 'radians', 'sin', 'sinh', 'sqrt', 'tan', 'tanh', 'trunc']

```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 12. On Beyond Strings     

Now that you understand what functions are and how to `import` modules, let's look at some of the functions that are **built** in to Python (no modules required!).

You already know about some of the **built-in functions** we've used with strings, such as `.upper()`, `.lower()`, `str()`, and `len()`. These are great for doing work with strings, but what about something a little more analytic?


**설명:** [ Learn ]       
• Ch12. On Beyond Strings 에서는 Built-in 함수를 학습한다.    
• Python 내장함수(built-in function) 에 대하여 알아보자.    
• 내장함수는 import 을 선언하지 않고도 자유롭게 사용할수 있게 해준다.    
• 대표적인 내장 함수는 다음과 예와 같다.    
• e.g. .upper() , .lower() 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* What do you think the code in the editor will do? Click `Run` when you think you have an idea.


**설명:** [ Instruction ]   
• Run 을 실행 후, 어떻게 동작 되는지를 설명해 보라. 
{: .notice--info}


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
def biggest_number(*args):
  print max(args)
  return max(args)
    
def smallest_number(*args):
  print min(args)
  return min(args)

def distance_from_zero(arg):
  print abs(arg)
  return abs(arg)

biggest_number(-10, -5, 5, 10)
smallest_number(-10, -5, 5, 10)
distance_from_zero(-10)
```

**설명:** [ Solution ]    
• 함수 biggest_number()는 입력된 argument 최대값을 반환한다.     
• 함수 smallest_number()는 입력된 argument 최소값을 반환한다.    
• 함수 distance_from_zero()는 입력된 argument 절대값을 반환한다.
{: .notice--info}



**결과** 
``` 
10
-10
10
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 13. max()    

The `max()` function takes any number of arguments and returns the largest one. ("Largest" can have odd definitions here, so it's best to use `max()` on **integers** and **floats**, where the results are straightforward, and not on other objects, like **strings**.)

For example, max(1,2,3) will return 3 (the largest number in the set of arguments).


**설명:** [ Learn ]     
• Ch13. max() 에서는 함수 max()를 학습한다.       
• Python 내장 함수 max() 는 arguments 중 가장 큰 값을 반환한다.    
• 단, arguments 값이 integer와 floats 만 있다는 조건이다.    
• 만약 arguments 값이 문자열이면, 문자열 값을 계산해서 더 큰 값을 반환한다.    
• 이 장에서는 숫자만 입력 된다는 조건에서 이야기 한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Try out the `max()` function on line `3` of the editor. You can provide any number of **integer** or **float** arguments to `max()`.


**설명:** [ Instruction ]    
• Editor 화면의 라인 3 에서 함수 max()를 사용하라.    
• 숫자만 입력된다는 조건에서 가장 큰수를 반환한다.  
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

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Set maximum to the max value of any set of numbers on line 3!

maximum = max(4, 8, 15)

print maximum
```

**설명:** [ Solution]    
• Arguments 4, 8, 15 중 가장 큰 값을 반환한다. 
{: .notice--info}


**결과** 
``` 
15
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 14. min()    

`min()` then returns the smallest of a given series of arguments.



**설명:** [ Learn ]     
• Ch14. min() 에서는 함수 min() 을 학습한다.    
• Python 내장 함수 min() 는 arguments 중 가장 작은 값을 반환한다.    
• 단, arguments 값이 integer와 floats 만 있다는 조건이다.    
• 만약 arguments 값이 문자열이면, 문자열 값을 계산해서 더 작은 값을 반환한다.    
• 이 장에서는 숫자만 입력 된다는 조건에서 이야기 한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Go ahead and set minimum equal to the `min()` of any set of integers or floats you'd like.


**설명:** [ Instruction ]   
• 함수 min()를 사용하여라.    
• Arguments 로 어떤값을 넣어도 가장 작은 값을 반환한다.    
• 단, arguments는 숫자만 입력한다.
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
# Set minimum to the min value of any set of numbers on line 3!

minimum = min(4, 8, 15)

print minimum
```

**설명:** [ Solution ]   
• 함수 min()를 사용하여, 입력값 4, 8, 15 중 가장 작은 값을 반환한다.
{: .notice--info}


**결과** 
``` 
4
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 15. abs()    

The `abs()` function returns the absolute value of the number it takes as an argument—that is, that **number's distance from 0** on an imagined number line. For instance, 3 and -3 both have the same absolute value: 3. The `abs()` function **always returns a positive value**, and unlike `max()` and `min()`, it only takes a **single number**.


**설명:** [ Learn ]     
• Ch15. abs() 에서는 함수 abs() 를 학습한다.    
• 함수 abs() 는 절대값을 구하는 함수이다.    
• 절대값이란? 입력값이 0 에서 얼마나 떨어져 있는지를 구하는 것이다.    
• -3 과 3 은 절대값이 같다. 같은 값이 반환된다.     
• 함수 abs() 는 argument 를 1개 만 입력할 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Set absolute equal to the absolute value of -42 on line 1.


**설명:** [ Instruction ]   
• Argument 값으로 -42 를 입력하고, -42 의 절대값을 구하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* skip

<p style="page-break-before: always;"></p>
<br>

**설명:**    
• skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
absolute = abs(-42)

print absolute
```

**설명:** [ Solution ]    
• abs(-42) 는 절대값 42 를 반환한다.
{: .notice--info}


**결과** 
``` 
42
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 16. type()    

Finally, the `type()` function returns the type of the data it receives as an argument. If you ask Python to do the following:

```python
print type(42)
print type(4.2)
print type('spam')
```

Python will output:
```
<type 'int'>
<type 'float'>
<type 'str'>
```



**설명:** [ Learn ]      
• Ch16. type() 에서는 함수 type() 를 학습한다.    
• 함수 type() 는 입력값 arguments의 type 이 무엇인지 알려준다.    
• type(42) 를 호출하면, arguments 42 가 integer type 임을 알려준다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Have Python print out the type of an **int**, a **float**, and a **str** string in the editor.     
* You can pick any values on which to call `type()`, so long as they produce one of each.


**설명:** [ Instruction ]    
• 함수 type() 을 사용하여라.     
• 입력된 argumetns 값이 integer, float, string type 이 출력 되도록 하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Here's a freebie if you're a bit stuck:     
  * print type('I have to push the pram a lot')     
* will cover your str string requirement.    

**설명:** [ Hint ]    
• type('i am a boy') 은 argument 값 i am a boy 의 값이 string 임을 알려준다.    
• 이것을 출력하면, <type 'str'>  라고 출력된다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Print out the types of an integer, a float,
# and a string on separate lines below.

print type(108)
print type(3.14)
print type('hello')
```

**설명:** [ Solution ]   
• 함수 type() 은 argument의 값이 어떤 type 인지를 알려준다.    
• type(108) 은 argument 가 integer 이므로 <type 'int'> 를 출력한다.    
• type(3.14) 은 argument 가 float 이므로 <type 'float'> 를 출력한다.    
• type('hello') 은 argument 가 string 이므로 <type 'str'> 를 출력한다.
{: .notice--info}


**결과** 
``` 
<type 'int'>
<type 'float'>
<type 'str'>
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 17. Review: Functions    

Okay! Let's review functions.

```python
def speak(message):
  return message

if happy():
  speak("I'm happy!")
elif sad():
  speak("I'm sad.")
else:
  speak("I don't know what I'm feeling.")
```

Again, the example code above is just there for your reference!


**설명:** [ Learn ]      
• Ch17. Review: Functions 에서는 함수를 복습한다.     
• 위 함수를 설명해 보자.    
• 함수 speak()는 arguments 의 값을 반환한다.    
• 조건문 if/elif/else의 조건절에 따라 함수 speak()가 호출된다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* First, def a function, `shut_down`, that takes one argument `s`. Don't forget the parentheses or the colon!

* Then, if the `shut_down` function receives an s equal to "yes", it should return "Shutting down"

<p style="page-break-before: always;"></p>
<br>

* Alternatively, elif s is equal to "no", then the function should return "Shutdown aborted".

* Finally, if `shut_down` gets anything other than those inputs, the function should return "Sorry"



**설명:** [ Instruction ]    
• 함수 shut_down(s) 을 정의한다.    
• 이 함수는 arguments 로 s 를 가진다.    
• 함수 뒤에는 ( : ) 가 있어야 하는것을 잊지 말자.    
• 함수 shut_down() 는 argument가 "yes"가 입력시, "Shuttingdown"을 출력한다.    
• 만약 "no"가 입력되면, "Shutdown aborted" 가 출력된다.    
• 마지막으로, "yes"도 "no"도 아닌 값이면 "Sorry"를 출력한다.
{: .notice--info}



<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Ensure your function outputs appear exactly as shown!

* Also, ensure your function returns the above values rather than printing them.

**설명:** [ Hint ]    
• return 문을 실행하기 전에 먼저 출력을 하라. ( e.g. print )    
• 그렇게 하면, 입력된 값이 무엇인지를 정확히 알 수 있다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def shut_down(s):
  if s == "yes":
    return "Shutting down"
  elif s == "no":
    return "Shutdown aborted"
  else:
    return "Sorry"
```

**설명:** [ Solution ]    
• 함수 shut_down(s) 는 arguments 값 s 를 가진다.   
• 입력값 s 가 "yes" 이면, 문자열 "Shutting down"    를 반환한다.    
• 입력값 s 가 "no"  이면, 문자열 "Shutting aborted" 를 반환한다.    
• 입력값 s 가 "yes" 도 "no" 도 아니면, 문자열 "Sorry" 를 반환한다.    
• 조건문 if/elif/else 뒤에 ( : ) 가 오는것을 주의하자.
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
<font size="3"  face="돋움">FUNCTIONS</font> 

### 18. Review: Modules    

Good work! Now let's see what you remember about importing modules (and, specifically, what's available in the `math` module).


**설명:** [ Learn ]      
• Ch18. Review: Modules 에서는 import 모듈을 복습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Import the `math` module in whatever way you prefer.    
* Call its `sqrt` function on the number `13689` and `print` that value to the console.


**설명:** [ Instruction ]    
• 모듈 math 를 import 선언하라.    
• 함수 sqrt() 를 사용하라.    
• Arguments 값을 13689 를 입력하라.     
• 그 결과를 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* There are three ways you can import the `sqrt()` function, but we'd probably go with    

```python
from math import sqrt
```    
<p style="page-break-before: always;"></p>
<br>

* You can figure out the rest. We believe in you!

**설명:** [ Hint ]    
• 함수 sqrt() 를 사용하는 방법은 3가지 이다.    
• 첫째, 직접 함수 sqrt()를 만든다.   
• 둘째, 모듈 math 를 import 한다.    
• 셋째, 모듈 math 를 구체적으로 import 한다.    
• e.g. from math import sqrt    
• 3가지 방법중 하나를 사용하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
import math
print math.sqrt(13689)
```

**설명:** [ Solution ]     
• 모듈 math 를 import 하였다.    
• 모듈 math 의 함수 sqrt(13689)를 호출후, 출력하였다.
{: .notice--info}


**결과** 
``` 
117.0
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FUNCTIONS</font> 

### 19. Review: Built-In Functions    

Perfect! Last but not least, let's review the `built-in functions` you've learned about in this lesson.

```python
def is_numeric(num):
  return type(num) == int or type(num) == float:

max(2, 3, 4) # 4
min(2, 3, 4) # 2

abs(2) # 2
abs(-2) # 2
```

**설명:** [ Learn ]       
• Ch19. Review: Built-In Functions 에서는 빌트인 함수를 복습한다.    
• 함수 is_numeric(num) 은 arguments 값 num 을 받는다.    
• 함수 type(num)을 사용하여, 입력값 num 의 type 값을 반환한다.    
• 입력값 num 의 type 이 int 이거나, float 이면 해당 type 값을 반환한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* First, def a function called `distance_from_zero`, with one **argument** (choose any argument name you like).

* If the type of the argument is either **int** or **float**, the function should return the **absolute value** of the function input.

* Otherwise, the function should return **"Nope"**

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]    
• 함수 distance_from_zero() 를 작성하라.    
• Arguments 명은 자신이 좋아하는 이름으로 짓는다.    
• Arguments 의 type 이 int or float 이면, 입력된 값의 절대값을 출력한다.    
• 그렇지 않으면 "Nope"가 출력되게 한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* You can check to see if a value is of type int just as shown in the instructions:    

```python
if type(thing) == int or type(thing) == float:
  # do something with the number
```    

* Make sure your capitalization and punctuation are exactly as shown!

**설명:** [ Hint ]    
• Arguments 의 type을 알려주는 함수 type() 를 사용하라.    
• 함수 type() 를 사용하여 입력값이 int or floast 인지를 파악한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def distance_from_zero(num):
  if type(num) == int or type(num) == float:
    return abs(num)
  else:
    return "Nope"
```

**설명:** [ Solution ]    
• 함수 distance_from_zero(num) 은 arguments 값 num 을 가진다.    
• 입력값 num 의 type 이 int 이거나 float 이면 절대값 abs(num)을 반환한다.    
• 그 외에는 문자열 "Nope"가 반환된다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**결과** 
``` 
#skip
```