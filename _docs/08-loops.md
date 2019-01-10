---
# layout : rchive
title: "Loops"
permalink: /loops/
excerpt: "We learn about loops Syntax."
last_modified_at: 2019-01-08T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    
 <hr style="border: solid 1px #dddddd ;">

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 1. While you're here    

The **`while`** loop is similar to an if statement: it executes the code inside of it if some condition is true. The difference is that the while loop will continue to execute as long as the condition is true. In other words, instead of executing if something is true, it executes while that thing is true.

Line 6 decides when the loop will be executed. So, "as long as count is less than 5," the loop will continue to execute. Line 8 increases count by 1. This happens over and over until count equals 5. 



**설명:**     
while 문은 if 문과 비슷하다.  while안의 조건절이 True 이면, 실행 되는 구조이다.    
if문과 다른점은 조건절 안 값이 True 이면, 계속 실행된다는 것이다. if문은 조건절, 예를 들어 3번 실행하라고 조건을 주면 3번 실행하고 완료되지만, while문은 조건문 안의 값이 Ture(예를 들면, 0 < 5 )가 되면 무한대로 실행한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Change the loop so that it counts **from 0 up to 9** (inclusive).

Be careful not to alter or remove the count += 1 statement. If your program has no way to increase count, your loop could go on forever and become an infinite loop which could crash your computer/browser!    


**설명:**     
① 반복문을 9(포함)까지 세는 프로그램으로 바꾸어라. (현재는 4까지 셈)   
변수 `count` 가 증가하지 않으면, 무한대로 반복되는 프로그램이 될 수 있다. 이럴 경우 컴퓨터에 문제가 발생할 수 있으니 주의하자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
To make sure your loop counts up to 9, your condition should be count < 10 (or count <= 9).


**설명:**    
9까지만 실행되는 조건문을 만들어라. ( `count < 10 or count <= 9` )  

{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
count = 0

if count < 10:
  print "Hello, I am an if statement and count is", count

while count < 10:
  print "Hello, I am a while and count is", count
  count += 1
```

**설명:**     
if 문은 1번 출력할 것이다. 그리고 while 문은 `count`가 9일때 까지 9번 출력될 것이다.  
{: .notice--info}


**결과** 
``` 
Hello, I am an if statement and count is 0
Hello, I am a while and count is 0
Hello, I am a while and count is 1
Hello, I am a while and count is 2
Hello, I am a while and count is 3
Hello, I am a while and count is 4
Hello, I am a while and count is 5
Hello, I am a while and count is 6
Hello, I am a while and count is 7
Hello, I am a while and count is 8
Hello, I am a while and count is 9
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 2. Condition    

The **condition** is the expression that decides whether the loop is going to continue being executed or not. There are 5 steps to this program:

1. The loop_condition variable is set to True

2. The while loop checks to see if loop_condition is True. It is, so the loop is entered.

3. The print statement is executed.

4. The variable loop_condition is set to False.

5. The while loop again checks to see if loop_condition is True. It is not, so the loop is not executed a second time.

 



**설명:**     
조건절(loop_condition)은 반복(loop)을 계속 실행할지 그만 둘지를 결정하는 표현이다. 다음 5단계로 진행된다.     
① 조건절의 변수값을 True 로 설정한다.       
② 조건절의 상태가 True 이면, 반복문 안으로 들어간다.    
③ print문을 출력한다.     
④ 조건절의 상태를 False 로 설정한다.    
⑤ while문의 조건절을 다시 True 인지 확인한다. True가 아니면 더이상 반복문을 실행하지 않는다.       
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** See how the loop checks its condition, and when it stops executing? When you think you've got the hang of it, click Run to continue.


**설명:**     
① 실행이 멈췄을때, 반복문의 상태를 어떻게 확인 하는지 살펴보라. 예상한대로 실행되는지 Run을 실행해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
See how the source works.



**설명:**     
소스가 어떻게 동작하는지를 확인 하세요. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
loop_condition = True

while loop_condition:
  print "I am a loop"
  loop_condition = False
```

**설명:**     
변수 `loop_condition`을 True로 설정한다. 이후, while 문에 진입하고, `print "I am a loop"`를 출력하고, 변수 `loop_condition`을 False로 변경한다. 그리고 다시 while의 조건절 `loop_condition`이 True인지를 확인하고, 맞으면 while 의 블럭문이 실행되고, 아니면 while 문을 빠져나간다.  
{: .notice--info}


**결과** 
``` 
I am a loop
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 3. While you're at it    

Inside a while loop, you can do anything you could do elsewhere, including arithmetic operations. 



**설명:**    
while 조건문 에서는 사칙 연산을 비롯하여 다른 곳에서 사용했던 어떤 것이든 들어갈수 있다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a while loop that prints out all the numbers from 1 to 10 squared (1, 4, 9, 16, ... , 100), each on their own line.

* Fill in the blank space so that our while loop goes from 1 to 10 inclusive.
* Inside the loop, print the value of num squared. The syntax for squaring a number is num ** 2.
* Increment num.



**설명:**     
① while 문을 사용하여 1부터 10까지의 값의 제곱근 값을 출력 되도록 하라.    
• while문의 조건을 넣는 공간에 1부터 10까지 돌도록 채우라.       
• while문 내부 실행 블럭에서는 `num ** 2`값을 출력 하여라.       
• 변수 `num`을 증가 시켜라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Your condition will have to be num <= 10 (or num < 11) so that the loop will always print until num is 11.


**설명:**     
조건절 `num <= 10` or `num < 11` 로 10 이하 인지를 확인한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
num = 1

while (num <= 10):  # Fill in the condition
  # Print num squared
  	print (num ** 2)
  # Increment num (make sure to do this!)
  	num += 1
```

**설명:**     
• `num <= 10` 은 변수 `num`이 10이하 일때까지 실행하겠다는 의미이다.     
• while 실행 블럭 안에 `num ** 2`는 제곱근을 구하는 방법이다.     
• 마지막으로 `num +=1`은 변수 `num`을 증가시켜, while문 조건이 맞으면 while을 빠져 나가도록 한다.
{: .notice--info}



**결과** 
``` 
1
4
9
16
25
36
49
64
81
100
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 4. Simple errors    

A common application of a while loop is to check user input to see if it is valid. For example, if you ask the user to enter y or n and they instead enter 7, then you should re-prompt them for input.



**설명:**    
주로 while 조건문은, 사용자가 입력한 값이 유효한지를 체크 하는 기능을 한다. 예를 들면, 당신은 사용자가 `y` or `n`를 입력하길 기대하는데, 사용자가 `7`을 입력하면, 당신은 다시 입력하는 단계로 되돌아 갈 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Fill in the loop condition so the user will be prompted for a choice over and over while choice does not equal 'y' and choice does not equal 'n'.


**설명:**     
① rompt에서 입력값이 y 또느 n 만 입력되도록 하는 조건문을 되도록 조건절을 채워라. 만약 y, n 이외의 값이 입력되면 다시 입력하도록 반복되어야 한다.      
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember, use the != operator to test if two things are different, such as choice != "y", and the and operator to check more than one thing, such as A and B.


**설명:**    
`!=`를 사용하여 두 값 이외에는 True 가 되지 않도록 해야 한다. `!="y"`는 비교값이 "y"가 같지 않는지를 비교하는 것이다. `and` 연산자는 앞에서 배운 바와 같이 `A and B`는 A, B 모두 True 이어야 한다.    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
choice = raw_input('Enjoying the course? (y/n)')

while choice != 'y' and choice != 'n':  # Fill in the condition (before the colon)
  choice = raw_input("Sorry, I didn't catch that. Enter again: ")
```

**설명:**     
`choice != 'y' and choice !='n'`는 `choice`값이 'y`도 아니고, 'n'도 아닌경우다.
{: .notice--info}



**결과** 
``` 
Enjoying the course? (y/n)x
Sorry, I didn't catch that. Enter again: z
Sorry, I didn't catch that. Enter again: y
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 5. Infinite loops    

An **infinite loop** is a loop that **never exits**. This can happen for a few reasons:

1. The loop condition cannot possibly be false (e.g. while 1 != 2)

2. The logic of the loop prevents the loop condition from becoming false.

Example:
```python
count = 10
while count > 0:
  count += 1 # Instead of count -= 1
```



**설명:**     
무한 loop는 프로그램을 빠져나가지 않고 계속 반복되는 것이다. 이렇게 되는데는 여러가지 이유가 있다.    
① 조건문 이 무조건 참일때 (`while 1 !=2 `)    
② 프로그램 로직상 false가 발생할수 없는 경우 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** The loop in the editor has **two problems**: it's missing a colon (a syntax error) and count is never incremented (logical error). The latter will result in an infinite loop, so be sure to **fix** both before running!


**설명:**     
① 반복문이 2개의 문제가 있다. 하나는 문법적으로 `:`이 빠져 있고, 하나는 로직적으로 무한 반복이 되는 것이다. 프로그램을 실행하기 전에 고쳐라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Since count is never incremented (count += 1), count is always 0, and since zero is less than ten, 0 will be printed over and over again forever.


**설명:**     
변수 count가 증가하지 않으면 count 값은 0 이기에 항상 10보다 작게 되며, 이는 조건문이 True가 된다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
count = 0

while count < 10: # Add a colon
  print count
  # Increment count
  count += 1
```

**설명:**     
변수 `count`가 0부터 시작되어 10보다 작을 때 까지 변수 `count`값을 출력되는 프로그램 이다. 변수 `count`값을 증가시켜줘서, 10번을 출력하고 프로그램을 빠져나온다. 
{: .notice--info}



**결과** 
``` 
0
1
2
3
4
5
6
7
8
9
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 6. Break    

The **break** is a one-line statement that means "exit the current loop." An alternate way to make our counting loop exit and stop executing is with the `break` statement.

* First, create a while with a condition that is always **true**. The simplest way is shown.

* Using an `if` statement, you define the stopping condition. Inside the if, you write break, meaning "exit the loop."

The difference here is that this loop is guaranteed to run at least once.





**설명:**     
`break`문을 만나면 현재 loop를 빠져나간다.    
• while문의 조건절을 항상 True 인 경우에만 진행 되도록 지정한다. Ture가 아닐때 그 loop를 빠져나간다.    

• while문의 내부 블럭에서 if문을 사용해서 멈춰도 된다. if 문에 조건을 걸어서 해당 조건이 되면 break 사용하여 해당 loop를 빠져나간다.     
이런 경우, 무조건 while 내부 내용이 1번은 실행된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** See what the break does? Feel free to mess around with it (but make sure you don't cause an infinite loop)! Click Run when you're ready to continue.


**설명:**     
① `break` 가 무슨일을 하는지 살펴보라. 가볍게 살펴보고, 실행 시켜 보아라.   
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
count = 0

while True:
  print count
  count += 1
  if count >= 10:
    break

```

**설명:**     
변수 `count`가 10이 되면 강제로 break 문이 발동되어 loop를 빠져 나간다. 
{: .notice--info}



**결과** 
``` 
0
1
2
3
4
5
6
7
8
9
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 7. While / else    

Something completely different about Python is the **`while/else`** construction. **`while/else`** is similar to **`if/else`**, but there is a difference: the **else** block will execute anytime the loop condition is evaluated to False. This means that it will execute if the loop is never entered or if the loop exits normally. If the loop exits as the result of a break, the else will not be executed.

In this example, the loop will break if a 5 is generated, and the else will not execute. Otherwise, after 3 numbers are generated, the loop condition will become false and the else will execute.





**설명:**     
`while/else`는 python에 사용되는 독특한 구조이다.    
`if/else` 의 `else`와 비슷하지만, `if/else`는 `if`문이 실행되면 `else`문이 실행되지 않지만, `while/else`는 `while`문이 flase 되어 빠져 나오면 반드시 `else`문이 동작된다.  실습을 통해서 알아보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Click Run to see while/else in action!


**설명:**     
① 실행해서, 소스가 어떻게 동작되는지를 확인해 보자.  
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
import random

print "Lucky Numbers! 3 numbers will be generated."
print "If one of them is a '5', you lose!"

count = 0
while count < 3:
  num = random.randint(1, 6)
  print num
  if num == 5:
    print "Sorry, you lose!"
    break
  count += 1
else:
  print "You win!"
```

**설명:**     
while문은 변수 `count`가 3보다 작을때까지 내부 블럭이 동작한다. 더불어 내부 블럭에는 변수 `num`이 5가 될때까지 실행된다.     
while문을 빠져나오면, `else`문의 `print "You win!"`이 출력된다. 
{: .notice--info}



**결과** 
``` 
Lucky Numbers! 3 numbers will be generated.
If one of them is a '5', you lose!
1
6
1
You win!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 8. Your own while / else    

Now you should be able to make a game similar to the one in the last exercise. The code from the last exercise is below:
```python
count = 0
while count < 3:
  num = random.randint(1, 6)
  print num
  if num == 5:
    print "Sorry, you lose!"
    break
  count += 1
else:
  print "You win!"
```
In this exercise, allow the user to guess what the number is 3 times.
```python
guess = int(raw_input("Your guess: "))
```
Remember, **`raw_input`** turns user input into a **string**, so we use **`int()`** to make it a number again.





**설명:**     
`while/else`문이 어떻게 사용되는지는 살펴 보자.     
참고로, `raw_input()`내재 함수는 return 값이 문자열(string)이다. 즉, 입력을 숫자로 입력해도 내부적으로는 문자열로 취급된다. 그러므로 `int(raw_input("Your guess: "))`로 숫자로 바꿔 줘야 한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Use a while loop to let the user keep guessing so long as guesses_left is greater than zero.

* Ask the user for their guess, just like the second example above.

* If they guess correctly, print "You win!" and break.

* Decrement guesses_left by one.

* Use an else: case after your while loop to print "You lose.".




**설명:**     
① 변수 `guesses_left`가 0 보다 클 동안 사용자가 계속 질문하는 while 문을 만든다.    
• 상단 처럼 질문하는 문을 만들자.    
• 만약, 질문한 값이 맞으면 "You win!" 이라고 출력하고, break문으로 빠져나오자.     
• 변수 `guess_left`를 1씩 줄여 나가자 `guess_left -=1`    
• `else`문을 사용하여 while 문을 빠져나오면 "You lose."라고 출력하자.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
This game will have a very similar structure to the example, but instead of losing right before the break, the user should win.

The if should check if guess == random_number. If it does, then it's the winning guess!


**설명:**     
앞의 예제와 비슷하지만, break 문이 걸리는게 이겼을때 이다.     
`if guess == random_number`인 경우가 승리하는 조건이다. 
random값은 while 문 시작 하기전에 산출된다.  
break문이 실행되어 while문을 빠져나갈때, else문은 실행되지 않는다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint

# Generates a number from 1 through 10 inclusive
random_number = randint(1, 10)

guesses_left = 3
# Start your game!
while guesses_left > 0:
  guess = int(raw_input("Your guess: "))
  if guess == random_number:
    print "You win!"
    break
  guesses_left -= 1
else:
  print "You lose."

```

**설명:**     
미리 `random_number`값을 가진다.    
변수 `guess_left`가 0보다 클동안 while문이 진행된다.     
prompt 에서 `"Your guess: "`로 임의의 숫자를 입력 받는다. 입력받은 값은 변수 `guess`에 저장된다.      
`guess`값이 미리 산출한 `random_number`과 같으면 "You win!"을 출력한다.그리고 break 문이 작동되어 loop를 빠져나온다. 그렇지 않으면 변수 `guess_left`를 -1 하도 다시 loop를 돈다.     
`guesses_left` 값이 0이 되면 while문을 빠져나오고, `else`문이 실행되어 `print "You lose"`가 동작된다.  
{: .notice--info}



**결과**
`#` case : fail    
``` 
Your guess: 2
Your guess: 2
Your guess: 2
You lose.
```
`#` case : correct   
```
Your guess: 2
Your guess: 1
Your guess: 3
You win!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 9. For your health    

An alternative way to loop is the for loop. The syntax is as shown in the code editor. This example means "for each number i in the range 0 - 9, print i".



**설명:**     
앞에서 배운 for 문은 또다른 반복문이다. 즉, while문을 대체할 수 있다. edit 창에 있는 소스는  0부터 9까지 반복적으로 돌면서 산출하는 소스이다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Make the loop print the numbers from 0 to 19 instead of 0 to 9.


**설명:**     
① 0부터 19까지 숫자를 출력하는 반복문으로 변경하라. (기존 0부터 9까지 산출하는 소스를 이용) 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Make sure to change the number inside of **`range`**.


**설명:**     
`rang()` 함수를 사용하자. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print "Counting..."

for i in range(20):
  print i
  
  
```

**설명:**     
`range(20)` 함수는 20 미만의 숫자를 0부터 20개 출력하는 것이다. 
{: .notice--info}



**결과** 
``` 
Counting...
0
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 10. For your hobbies    

This kind of loop is useful when you want to do something a **certain number of times**, such as append something to the end of a list.



**설명:**     
for문은 내가 몇번 loop를 둘려야 하는지를 정확히 알때 사용한다. 예를 들면,
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a **`for`** loop that prompts the user for a **hobby 3 times**.

* Save the result of each prompt in a **`hobby`** variable

* append each one to `hobbies[]`.

* print hobbies after your for loop

Make sure to answer the prompts in the terminal when testing your code!


**설명:**     
① for문을 사용하여 취미를 3번 묻는 것을 만들어라.     
• 변수 `hobby`에 prompt에서 입력 받은 값을 저장하라.      
• 입력 받은 `hobby`를 리스트 `hobbies`리스트에 추가하라.    
• for 문을 빠져나오고 `hobbies`리스트 값을 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Your for loop should use range(3). You should use the **`raw_input()`** function to get info from the user and **`hobbies.append(hobby)`** to add the **`hobby`** to the list.


**설명:**     
• `raw_input()`함수를 사용하라.     
• 리스트에 추가하는것은 `hobbies.append(hobby)`이다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
hobbies = []

# Add your code below!

for num in range(3):
  hobby =  raw_input("Tell me one of your favorite hobbies: ")
  hobbies.append(hobby)

print hobbies
```

**설명:**     
`for num in range(3):`로 3번 입력 받는다.     
입력받은 값은 리스트 hobbies에 추가한다.    
for 문을 빠져나오면, 리스트 hobbies를 출력한다. 
{: .notice--info}



**결과** 
``` 
Tell me one of your favorite hobbies: swim
Tell me one of your favorite hobbies: ski
Tell me one of your favorite hobbies: cycle
[u'swim', u'ski', u'cycle']
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 11. For your strings    

Using a for loop, you can print out each individual character in a string.

The example in the editor is almost plain English: "for each character c in thing, print c". 



**설명:**     
loop 반복을 통하여 문자열을 문자 단위로 나눌수 있다.     
edit 창에 있는 소스는 문자열 단어를 스펠링으로 나누는 소스이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Add a second for loop so that each character in **`word`** is printed one at a time.


**설명:**     
① for 문을 추가하여, 변수 `word`에 담겨 있는 "eggs"를 하나씩 출력 되게 하여라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Use the example on lines 3 - 4 as a model.


**설명:**     
3,4라인에 있는 for문을 참조하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
thing = "spam!"

for c in thing:
  print c

word = "eggs!"

# Your code here!
for character in word:
  print character
```

**설명:**     
변수 `word`에 있는 문자열 "eggs!"를 알파벳 하나씩 읽어서 출력한다. 
{: .notice--info}



**결과** 
``` 
s
p
a
m
!
e
g
g
s
!
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 12. For your A    

String manipulation is useful in for loops if you want to modify some content in a string.
```python
word = "Marble"
for char in word:
  print char,
```  
The example above iterates through each character in word and, in the end, prints out M a r b l e.

The `,` character after our print statement means that our next print statement **keeps** printing on **the same line**.





**설명:**     
for 문은 문자열 조작을 하기에 편리하다.    
예제에서 "Marble"가 M a r b l e 로 출력된다.    
여기에서 `print char ,` `,`는 문자열이 새로운 줄에서 출력되는 것이 아니라, 같은 라인에서 출력되는 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Let's filter out the letter "A" from our string.

* Do the following for each character in the **`phrase`**.
* If char is an "A" or char is an "a", print "X", instead of char. Make sure to include the trailing comma.
* Otherwise (else:), please print char, with the trailing comma.



**설명:**     
① 문자열에서 "A"를 걸러내는 것을 해 보자.    
• 변수 `phrase`에 들어있는 문자열을 이용한다.    
• 문자 중 "A" or "a"는 해당 문자를 "X"로 출력되게끔 바꿔라. `,`를 사용하여 한줄에 출력되게 하라.        
• 그외는 `,`를 사용하여, 문자열을 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can use the same for syntax, for c in s, as before. Use an if to compare c to 'a' and 'A'. Print an 'X' in that case, and use an else to print the character otherwise.

Include a comma after the character to be printed in order to ensure it's not printed on its own line, like so:

```python
if c == "A" or c == "a":
  print "X",
```


**설명:**     
for 문을 돌면서 문자를 추출하고, 해당 문자가 "A" or "a"이면 "X"를 출력한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
phrase = "A bird in the hand..."

# Add your for loop
for char in phrase:
  if char == "A" or char == 'a':
    print 'X',
  else:
    print char,

#Don't delete this print statement!
print
```

**설명:** 
{: .notice--info}



**결과** 
``` 
X   b i r d   i n   t h e   h X n d . . .
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
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
<font size="3"  face="돋움">LOOPS</font> 
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
<font size="3"  face="돋움">LOOPS</font> 
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
<font size="3"  face="돋움">LOOPS</font> 
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
<font size="3"  face="돋움">LOOPS</font> 
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
<font size="3"  face="돋움">LOOPS</font> 
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
<font size="3"  face="돋움">LOOPS</font> 
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
