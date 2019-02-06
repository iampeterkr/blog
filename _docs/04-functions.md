---
# layout : rchive
title: "Functions"
permalink: /functions/
excerpt: "We learn about Functions Syntax."
last_modified_at: 2018-12-04T09:00:00-04:00
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


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 1. What Good are Functions?    

You might have considered the situation where you would like to reuse a piece of code, just with a few different values. Instead of rewriting the whole code, it's much cleaner to define a *function*, which can then be used repeatedly.


**설명:**     
• 가끔식, 자주 사용되는 기능을 반복적으로 사용할 필요성이 있다.    
• 코딩을 할때마다, 반복적으로 만들것이 아니라, 해당 기능을 함수로 만들어 놓고 재 사용하자.   
• 코딩중 해당 기능이 필요 할때마다 불러서 사용하는 것이 현명하다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the code in the editor.     
* If you completed the Tip Calculator lesson, you'll remember going through and calculating `tax` and `tip` in one chunk of program.     
* Here you can see we've `def`ined two functions: `tax` to calculate the tax on a bill, and `tip` to compute the tip.

* See how much of the code you understand at first glance (we'll explain it all soon).     
* When you're ready, click Run to continue.



**설명:**     
• editor 창에 구현되어 있는 tax 함수와, tip 함수를 해석해 보자.    
• 참고로, tax 함수는 세금을 계산해 주고, tip 함수는 팁을 계산해주는 함수이다.    
• 각 함수가 어떻게 작동 되는지를 이해해 보자.    
• 그리고 실행해보고, 당신이 생각한대로 동작되는지 확인해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Remember how we used `%s` to print strings? We can use `%f` to print floats! (That is, numbers with decimals in them.)

**설명:**    
• %s 는 문자열을 출력할때, %f 는 실수를 출력할때 사용한다. 
{: .notice--info}

<br>
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

**설명:**     
• 변수 meal_cost 에 100 을 대입한다.    
• tax 함수에 변수 meal_cost 를 대입하여 호출한다.    
• 변수 meal_with_tex 에 tax 함수 호출한 결과값을 저장한다.    
• tip 함수에 변수 meal_with_tax 를 대입하여 호출한다.    
• 변수 meal_with_tip 에 tip 함수 호출한 결과값을 저장한다.
{: .notice--info}


**결과** 
``` 
With tax: 108.000000
With tip: 124.200000
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 2. Function Junction    

Functions are defined with three components:

* The header, which includes the def keyword, the name of the function, and any parameters the function requires. Here's an example:

```python
def hello_world(): # There are no parameters
```

**설명:**     
• 함수를 사용하기 위해선 다음 3가지 구성이 필요하다.     
• 첫째, 사용할 함수 이름을 선언한다. 함수를 선언할때는 인자가 없다.   
{: .notice--info}


* An optional comment that explains what the function does.

```python
"""Prints 'Hello World!' to the console."""
```

**설명:**     
• 둘째, 함수가 하는 기능을 문자열 주석( """ """ ) 처리한다.    
{: .notice--info}


* The body, which describes the procedures the function carries out. The body is indented, just like conditional statements.

```python
print "Hello World!"
```
* Here's the full function pieced together:

```python
def hello_world():
  """Prints 'Hello World!' to the console."""
  print "Hello World!"
```


**설명:**     
• 셋째, 함수가 처리할 기능을 구현한다.     
• 함수 'def hello_world()' 는 인자가 없으며, "Hello world"를 출력한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Go ahead and create a function, spam, that prints the string "Eggs!" to the console. Don't forget to include a comment of your own choosing (enclose it in triple quotes!).


**설명:**     
• 함수 spam 을 만들어라.    
• 함수 spam 은  "Eggs!" 를 출력하는 역할을 한다.    
• 함수 spam 이 무슨 기능을 하는지 주석( """ """ ) 을 단다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* If you're stuck, look closely at the example function syntax in the instructional text. Remember: whitespace counts in Python!


**설명:**     
• 앞장의 함수를 구성하는 3단계를 다시 학습해보자.     
• 함수를 선언할때, 함수 끝에 ( : ) 를 주의 하자. 
{: .notice--info}

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

**설명:**     
• 함수 spam(): 을 선언한다.    
• 함수 spam 내부에 어떤 기능을 처리 하는지를 문자열 주석 처리한다.    
• 함수 spam 기능, 즉 "Eggs!" 를 출력하는 기능을 구현한다. 
{: .notice--info}


**결과** 
```
Eggs!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 3. Call and Response
After defining a function, it must be *called* to be implemented. In the previous exercise, **spam()** in the last line told the program to look for the function called **spam** and execute the code inside it.

 
**설명:** 함수는 먼저 선언을 하고, 이후에 해당 함수를 호출 하면, 해당 함수가 호출되어 실행된다. 그리고 그 결과값을 처음 호출한 곳으로 반환된다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** We've set up a function, `square`. Call it on the number `10` (by putting 10 between the parentheses of `square()`) on line 10!


**설명:** ① 함수 `squar()`를 호출하라. 호출할때, 인자 값을 `10`을 준다.(ex. `square(10)`)
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember when we called spam in the previous exercise, like this: spam()? You can do the same here with square(), only you'll need to put 10 in between the parentheses so square knows what number to... well, square.  


**설명:** 앞에서 배운 함수 `spam()` 은 인자 값이 없이 함수를 호출했지만, 이번에는 인자값을 괄호 사이에 인자값을 주어야 한다. 
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

**설명:** 함수 `square(10)`를 호출하면, 정의된 `square()` 함수가 호출되어 입력된 `n`값 `10`이 계산되고, 해당 값이 출력되고, 마지막에 변수 `squared`값이 반환된다. 
{: .notice--info}



**결과** 
``` 
10 squared is 100.
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

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


**설명:** `square(n)`에서 `n`은 parameter라고 부르고, `square(10)`에서 `10`은 arugument라고 부른다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Check out the function in the editor, `power`. It should take two **arguments**, a base and an exponent, and raise the first to the power of the second. It's currently broken, however, because its **parameters** are missing.

Replace the `___s` with the **parameters** base and exponent and then call the `power` function with a base of `37` and an exponent of `4`.

**설명:** ① `power`함수를 호출하는데, 먼저 `square()`의 비어져 있는 parameter를  정의하고, 호출하는 함수 `power(37,4)`argument를 작성하여라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Make sure to include the parameters base and exponent between the parentheses on line 1, and the arguments 37 and 4 between the parentheses on line 5. Your parameters and arguments need to be separated by a comma, like this: (base, exponent).


**설명:** base:37, exponent:4 , power(base, exponent) 구조이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def power(base, exponent):  # Add your parameters here!
  result = base ** exponent
  print "%d to the power of %d is %d." % (base, exponent, result)

power(37, 4)  # Add your arguments here!
```

**설명:** 함수 `power(37,4)`에 arguments를 넣고, 호출하면, 함수에 정의된 parameter 즉, `base`, `exponent`에 값이 전달된다. 
{: .notice--info}



**결과** 
``` 
37 to the power of 4 is 1874161.
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 5. Functions Calling Functions

We've seen functions that can print text or do simple arithmetic, but functions can be much more powerful than that. For example, a function can call another function:

```python
def fun_one(n):
  return n * 5

def fun_two(m):
  return fun_one(m) + 7
```


**설명:** 함수는 단순히 계산하고, 출력하는것 외에, 함수가 함수를 호출 할수도 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Let's look at the two functions in the editor: `one_good_turn` (which adds `1` to the number it takes in as an argument) and `deserves_another` (which adds 2).

Change the body of deserves_another so that it always adds 2 to the output of one_good_turn.


**설명:** ① editor에 2개의 함수, `one_good_turn()`과 `deserves_another()`함수가 있다. `one_good_turn()`는 1개의 parameter `n`을 받아서 그 값에 `1`을 더하는 기능을 한다. `deservers_another()`는 1개의 parameter `n`을 받아서 그값에 `2`를 더하는 기능을 한다. 그럼 `deservers_another()`를 `one_good_turn()` 함수에 항상 `2`를 더하는 함수로 변경하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

The n in the body of deserves_another should be replaced by a call to the function `one_good_turn(n)`.

**설명:** `deserves_another()`함수의 body `n` 자리에 `one_good_turn(n)`이 오도록 수정한다.
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

**설명:** `deserves_another()`의 내부 `n` 자리에 `one_good_turn(n)`로 교체하여 함수가 함수를 호출하는 기능을 한다. 
{: .notice--info}



**결과** 
``` 
#No answer
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

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

**설명:** 함수를 어떻게 호출하고 처리 되는지 다시한번 상기하자. 함수 뒤에 `:`을 주의 하자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** First, def a function called `cube` that takes an **argument** called `number`. Don't forget the parentheses and the **colon**!

**설명:** ① 함수 `cube()`를 만들자. argument는 `number`를 가진다. 함수 끝에는 `:`을 빼먹지 말자.
{: .notice--info}

**②**Make that function return the `cube` of that `number` (i.e. that number multiplied by itself and multiplied by itself once again).

**설명:** ② 함수 `cube()`는 전달 받은 argument `number`를 두번 곱한 결과값(`number * number * number`)을 반환한다.  argument는 `number`를 가진다. 함수 끝에는 `:`을 빼먹지 말자.
{: .notice--info}

**③** Define a second function called `by_three` that takes an argument called `number`.

**설명:** ③ 함수 `by_three()`는 argument `number`를 가지는 함수를 만든다. 
{: .notice--info}

**④** if that number is divisible by `3`, `by_three` should call `cube(number)` and return its result. Otherwise, `by_three` should return **False**.

**설명:** ④ 함수 `by_three()`는 `3`으로 나누어 떨어지면 함수 `cube(number)`를 호출하고, 그 결과값을 출력한다. 만약, `3`으로 나누어 떨어지지 않으면, False를 반환한다. 
{: .notice--info}

Don't forget that if and else statements need a : at the end of that line!

**설명:** `else`문을 사용할때 `:`을 주의하라. 
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
Make sure both functions return their values rather than printing them.

Both branches of the `if/else` statement in by_three need to have return statements in them (that's three returns total, two for by_three and one for cube).

**설명:** `%` 연산자를 사용하여 함수의 기능을 처리하고, `if/else`문을 사용할때, `:`을 주의하라.
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

**설명:** 함수 `by_three()`에서 함수 `cube()`를 호출한다. 
{: .notice--info}



**결과** 
``` 
#No answer
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 7. I Know Kung Fu
Remember `import` this from the first exercise in this course? That was an example of importing a module. A module is a file that contains definitions—including variables and functions—that you can use once it is imported.



**설명:** `import`는 맨 첫 번째에서 사용한적이 있다. `import`는 미리 만들어진 변수, 함수들의 집합체로 묶어둔것을 호출하여 사용하는 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Before we try any fancy importing, let's see what **Python** already knows about square roots. On line 3 in the editor, ask Python to

```python
print sqrt(25)
```
which we would expect to equal five.

Instead, it throws an error.


**설명:** ① Python에서는 미리 만들어 놓은 함수들을 묶어서 정의해 둔 것이 있다. 그중 하나가 함수 `sqrt()` 이다. `sqrt(5)`는 argument `5`를 루트 값을 구하는 함수이다. editor 3라인에서 `sqrt(25)`를 사용하면 루트5가 계산되어지는것이 아니라, error가 발생할 것이다. editor 창에서 시도 해 보라.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

No answer !!

**설명:** No answer !!
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Ask Python to print sqrt(25) on line 3.

print sqrt(25)
```

**설명:** print sqrt(25)를 하면 Error 가 발생한다. 
{: .notice--info}



**결과** 
``` 
Traceback (most recent call last):
  File "python", line 3, in <module>
NameError: name 'sqrt' is not defined
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 8. Generic Imports
Did you see that? Python said: **NameError: name 'sqrt' is not defined**. Python doesn't know what square roots are—yet.

There is a Python module named math that includes a number of useful variables and functions, and sqrt() is one of those functions. In order to access math, all you need is the import keyword. When you simply import a module this way, it's called a generic import.


**설명:** "NameError: name 'sqrt' is not defined" 는 해당 함수를 사용했지만, 그 함수를 찾지 못했을 경우 나타내는 Error 메시지 이다. Python은 각종 수학 관련 함수들을 모아놓은 모듈들의 묶음이 있다. 이 모듈에는 `sqrt()` 함수도 속해 있다. 이런 각 종 함수들을 우리는 직접 구현하지 않고, 간단히 `import`만 하여도 사용 할 수 있다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** You'll need to do two things here:

• Type `import math` on line 2 in the editor.
• Insert `math`. before `sqrt()` so that it has the form `math.sqrt()`. This tells Python not only to `import math`, but to get the `sqrt()` function from within `math`. Then hit `Run` to see what Python now knows.


**설명:** ① 2가지 일들을 해줘야 하는데, 그중 한가지는 2번 라인에 `import math`를 선언해 주고, `sqrt()`함수를 사용하기 위해선 `math.sqrt()`라고 사용해야 한다. 이후, `Run` 실행을 시켜보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Make sure you  `import math` (no colons or anything like that), and make sure you ask Python to print `math.sqrt(25)`.

**설명:** `import math` `math` 모듈을 불러오고, 해당 모듈은 `math.sqrt(25)`로 사용한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Ask Python to print sqrt(25) on line 3.
import math
print math.sqrt(25)

```

**설명:** 수학 관련 내장된 함수 모듈을 사용할려면 `import math` 모듈을 불러놓고, `math` 함수는 `.`을 사용하여 `math.sqrt(25)` 로 사용해 한다. 
{: .notice--info}



**결과** 
``` 
5.0
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 9. Function Imports
Nice work! Now Python knows how to take the square root of a number.

However, we only really needed the sqrt function, and it can be frustrating to have to keep typing `math.sqrt()`.

It's possible to import only certain variables or functions from a given module. Pulling in just a single function from a module is called a function import, and it's done with the `from` keyword:

```python
from module import function
```
Now you can just type `sqrt()` to get the square root of a number—no more `math.sqrt()`!





**설명:** `math.sqrt()`를 사용할수도 있지만, `import` 선언시 좀더 구체적으로 `math`에 대하여 선언해주면 `math`함수의 `sqrt()`를 사용한다고 `math.sqrt()`라고 쓰지않고 단순히 `sqrt()`만 사용할수 있다. 그러기 위해선, `import`할때, `from moudle import function` 이라고 구체적으로 선언해 주면 된다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Let's import only the `sqrt` function from `math` this time. (You don't need the `()` after `sqrt` in the `from math import sqrt` bit.)


**설명:** ① `from math import sqrt`에서 `sqrt`뒤에 '`()`를 안붙여 줘도 된다. `sqrt` 한수를 선언해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Remember: from module import function! (Don't include the parentheses here—just the function name, e.g. sqrt.)

**설명:** `from moudle import function` 방식으로 선언한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from math import sqrt
```

**설명:** `math` 모듈에서 `sqrt`함수를 사용하겠다는 것을 명확하게 선언해 준다. 
{: .notice--info}



**결과** 
``` 
#No answer!!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 10. Universal Imports
Great! We've found a way to handpick the variables and functions we want from modules.

What if we still want all of the variables and functions in a module but don't want to have to constantly type math.?

Universal import can handle this for you. The syntax for this is:

```python
from module import *
```

**설명:** 우리는 `from`을 사용하여 원하는 모듈을 콕 찝어서 사용할 수 있다. 그런데, 만일 우리가 원하는 함수가 여러개일때는 해당 함수만 콕 찍을개 아니라, 두루두루 쓸수 있게 선언할수 있다. 그리고 `math.`도 필요 없다. `*` 를 활용하여  `from module import *` 라고 선언해 주면 된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Use the power of `from module import *` to import everything from the math module on line 3 of the editor.


**설명:** ① `from module import *`의 강력한 기능을 사용하여, 3라인에 `math`모듈을 사용할수 있는 `import`를 선언해라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

```python
Just like this: from math import *
```
**설명:** `from math import *`
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Import *everything* from the math module on line 3!

from math import *
```

**설명:** `math` 모듈의 모든 함수/변수 기능을 사용하겠다고 선언한다. 
{: .notice--info}



**결과** 
``` 
#No answer !!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 11. Here Be Dragons
Universal imports may look great on the surface, **but they're not a good idea for one very important reason** : they fill your program with a ton of variable and function names without the safety of those names still being associated with the module(s) they came from.

If you have a function of your very own named `sqrt` and you `import math`, your function is safe: there is your sqrt and there is `math.sqrt`. If you do `from math import *`, however, you have a problem: namely, two different functions with the exact same name.

Even if your own definitions don't directly conflict with names from imported modules, if you import * from several modules at once, you won't be able to figure out which variable or function came from where.

For these reasons, it's best to stick with either import module and type module.name or just import specific variables and functions from various modules as needed.



**설명:** `*`를 사용하여 해당 모듈의 모든것을 가져오면 참으로 편리해 보인다. 그런데, `*`는 묻지 않고 해당 모듈에 대한 모든것을 가져온다. 그런데, 내가 만든 모듈이 Python 내부에서 제공하는 모듈과 이름이 같으면 어떻게 될까? Python은 혼돈이 올것이다. 예를 들어 지금 실행되는 `sqrt()`함수가 내가 작성한 함수인지, 아니면 `math`모듈에서 제공하는 `sqrt()`인지를 알수가 없다. 그렇기에 향후, 우리는 
좀더 정확하게 표현해야 한다. 내가 만든 함수는 `me.sqrt()`로 표현하고, `math`가 제공하는 함수는 `math.sqrt()`로 표현하는것이 프로그램 오류를 줄일수 있는 방법이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** The code in the editor will show you everything available in the **math** module.

Click `Run` to check it out (you'll see `sqrt`, along with some other useful things like `pi`, `factorial`, and `trigonometric` functions.

**설명:** ① editor에 있는 소스를 실행시켜보자. `math` 모듈에는 어떤 함수들이 포함되어 있는지 확인해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

No answer

**설명:** `No answer`
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
import math # Imports the math module
everything = dir(math) # Sets everything to a list of things from math
print everything # Prints 'em all!
```

**설명:** `math` 모듈에 속해 있는 모든 함수들을 보여준다. `dir`명령어를 사용하면 볼수 있다. 
{: .notice--info}



**결과** 
``` 
['__doc__', '__name__', '__package__', 'acos', 'acosh', 'asin', 'asinh', 'atan', 'atan2', 'atanh', 'ceil', 'copysign', 'cos', 'cosh', 'degrees', 'e', 'erf', 'erfc', 'exp', 'expm1', 'fabs', 'factorial', 'floor', 'fmod', 'frexp', 'fsum', 'gamma', 'hypot', 'isinf', 'isnan', 'ldexp', 'lgamma', 'log', 'log10', 'log1p', 'modf', 'pi', 'pow', 'radians', 'sin', 'sinh', 'sqrt', 'tan', 'tanh', 'trunc']

```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 12. On Beyond Strings

Now that you understand what functions are and how to `import` modules, let's look at some of the functions that are **built** in to Python (no modules required!).

You already know about some of the **built-in functions** we've used with strings, such as `.upper()`, `.lower()`, `str()`, and `len()`. These are great for doing work with strings, but what about something a little more analytic?


**설명:** `built-in function`에 대하여 알아보자. 모듈을 선언하지 않고서도 우리가 자유롭게 사용하는 함수가 있었다. `.upper()`, `.lower()`등이 대표적인 `built-in function` 이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** What do you think the code in the editor will do? Click `Run` when you think you have an idea.


**설명:** ① `Run`을 실행 시켰을때, 어떻게 동작되는지를 설명해 보라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

No answer !!

**설명:** `No answer !!`
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

**설명:** 최대값, 최소값, 절대값 이 반환된다. 
{: .notice--info}



**결과** 
``` 
10
-10
10
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 13. max()
The `max()` function takes any number of arguments and returns the largest one. ("Largest" can have odd definitions here, so it's best to use `max()` on **integers** and **floats**, where the results are straightforward, and not on other objects, like **strings**.)

For example, max(1,2,3) will return 3 (the largest number in the set of arguments).


**설명:** `max()`함수는 arguments중 가장 큰 값을 반환한다. 여기서는 integer와 floats만 있다는 전제하에서 가장 큰 수를 반환한다. (만약 string이 있다면 문자열의 값을 계산해서 문자열이 더 큰 수일도 있다. 하지만 여기서는 숫자만 이라는 전제하에 이야기 한다. ) 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Try out the `max()` function on line `3` of the editor. You can provide any number of **integer** or **float** arguments to `max()`.


**설명:** ① 숫자만 있다는 전제하에서 가장 큰수를 말한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

No answer !!

**설명:** `No answer !!`
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Set maximum to the max value of any set of numbers on line 3!

maximum = max(4, 8, 15)

print maximum
```

**설명:** argument `4`, `8`, `15`중 가장 큰 값을 반환한다. 
{: .notice--info}


**결과** 
``` 
15
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 14. min()
`min()` then returns the smallest of a given series of arguments.



**설명:** `min()` 함수는 가장 작은 숫자를 반환한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Go ahead and set minimum equal to the `min()` of any set of integers or floats you'd like.


**설명:** ① `min()`함수에 아무 숫자를 넣어서 가장 작은 수가 반환되는것을 보여라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

No answer !!

**설명:** `No answer !!`
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Set minimum to the min value of any set of numbers on line 3!

minimum = min(4, 8, 15)

print minimum
```

**설명:** `min()`함수를 사용하여 가장 작은 값을 반환한다. 
{: .notice--info}


**결과** 
``` 
4
```



<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 15. abs()
The `abs()` function returns the absolute value of the number it takes as an argument—that is, that **number's distance from 0** on an imagined number line. For instance, 3 and -3 both have the same absolute value: 3. The `abs()` function **always returns a positive value**, and unlike `max()` and `min()`, it only takes a **single number**.


**설명:** `abs()`함수는 절대값을 구하는 함수이다. 쉽게 이야기 하면 `0`에서 멀이 떨어진 값을 구하는 것이다. `-3`과 `3`은 같은 값이 반환된다. `abs()`함수는 argument 가 1개만 쓸수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Set absolute equal to the absolute value of -42 on line 1.


**설명:** ① argument 값이 `-42`인 절대값을 구하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

No answer !!

**설명:** `No answer !!`
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
absolute = abs(-42)

print absolute
```

**설명:** argument `-42`의 절대값을 구한다. 
{: .notice--info}


**결과** 
``` 
42
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

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



**설명:** `type()`함수는 argument의 값의 type이 무엇인지 반환해 준다. `type(42)`는 `42`가 integer type임을 알려준다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Have Python print out the type of an **int**, a **float**, and a **str** string in the editor. You can pick any values on which to call `type()`, so long as they produce one of each.


**설명:** ① `type()`함수를 사용하여 interger, float, string type이 출력되도록 Python으로 작성하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Here's a freebie if you're a bit stuck: print type('I have to push the pram a lot') will cover your str string requirement.
**설명:** `print type('i am a boy`)라고 하면, `<type 'str'>`라고 출력된다.
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

**설명:** `type()`함수는 argument의 값이 어떤 type인이지를 알려준다.
{: .notice--info}


**결과** 
``` 
<type 'int'>
<type 'float'>
<type 'str'>
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

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


**설명:** 위 함수를 설명해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** First, def a function, `shut_down`, that takes one argument `s`. Don't forget the **parentheses** or the **colon**!

Then, if the `shut_down` function receives an s equal to **"yes"**, it should return **"Shutting down"**

Alternatively, elif s is equal to "no", then the function should return "Shutdown aborted".

Finally, if `shut_down` gets anything other than those inputs, the function should return "Sorry"



**설명:** ① 먼저, 함수 `shut_down`을 정의하고, argument는 `s`를 취한다. `(), :`을 주의하라. 그런다음, `shut_down` 함수는 argument가 "yes"가 입력되면, "Shuttingdown"을 출력한다. 그렇지 않고, 만약 "no"가 입력되면, "Shutdown aborted"가 출력된다. 마지막으로, "yes"도 "no"도 아닌 값이면 "Sorry"를 출력하라.
{: .notice--info}



<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Ensure your function outputs appear exactly as shown!

Also, ensure your function returns the above values rather than printing them.

**설명:** `return` 하기전에 먼저 출력(`print`)하여라. 
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

**설명:** 함수의 if/elif/else 뒤에 `:`가 오는것을 주의하자. 
{: .notice--info}


**결과** 
``` 
#No answer !!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 18. Review: Modules
Good work! Now let's see what you remember about importing modules (and, specifically, what's available in the `math` module).


**설명:** 모듈에 대하여 정리한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Import the `math` module in whatever way you prefer. Call its `sqrt` function on the number `13689` and `print` that value to the console.


**설명:** ① `math`를 import 하고, `sqrt`함수를 사용하여 argument값을 `13689`를 입력하고 그 결과를 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

There are three ways you can import the `sqrt()` function, but we'd probably go with
```python
from math import sqrt
```
You can figure out the rest. We believe in you!

**설명:** `math.sqrt()`를 사용하려면 어떻게 선언해야 할지 고민하자.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
import math
print math.sqrt(13689)
```

**설명:** 
{: .notice--info}


**결과** 
``` 
117.0
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

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

**설명:** `built-in function` 사용 방법을 다시 생각해 보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** First, def a function called `distance_from_zero`, with one **argument** (choose any argument name you like).

If the type of the argument is either **int** or **float**, the function should return the **absolute value** of the function input.

Otherwise, the function should return **"Nope"**



**설명:** ① 함수 `distance_from_zero()`를 만들고, argument이름은 자신이 좋아하는 이름으로 짓는다. argument의 type이 int or float 이면, 입력된 값의 절대값을 출력하고, 그렇지 않으면 "Nope"가 출력되게 하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

You can check to see if a value is of type int just as shown in the instructions:
```python
if type(thing) == int or type(thing) == float:
  # do something with the number
```
Make sure your capitalization and punctuation are exactly as shown!

**설명:** `type()`를 사용하여 int or floast 인지를 알수 있다. 
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

**설명:** argument `num`입력값 type이 int or float 이면 해당 값의 절대값을 출력한다. 그렇지 않으면 "Nope"를 출력한다.
{: .notice--info}


**결과** 
``` 
#No answer
```


<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
