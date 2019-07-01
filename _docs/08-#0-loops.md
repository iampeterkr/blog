---
# layout : rchive
title: "Loops"
permalink: /loops/
excerpt: "We learn about loops Syntax."
# last_modified_at: 2019-02-20T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    


<hr style="border: solid 1px #dddddd ;">    

LESSON    

Loops allow you to quickly iterate over information in Python. In this lesson, we'll cover two types of loop: 'while' and 'for'.

**설명:** [ 학습방향 ]     
이 장에서는 while 문과, for 문을 학습한다.     
반복문을 활용하여 데이타를 신속하게 처리하는 방법을 학습한다.
{: .notice--info}     
     


<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 1. While you're here    

The `while` loop is similar to an if statement: it executes the code inside of it if some condition is true. The difference is that the while loop will continue to execute as long as the condition is true. In other words, instead of executing if something is true, it executes while that thing is true.

Line 6 decides when the loop will be executed. So, "as long as count is less than 5," the loop will continue to execute. Line 8 increases count by 1. This happens over and over until count equals 5. 



**설명:** [ Learn ]     
• Ch1. While you're here 에서는 while 문을 학습한다.    
• while 문은 if 문과 비슷하다.     
• while 문의 조건절이 True 이면, while 문 내부 구간이 실행 되는 구조이다.    
• if 문과 다른점은 while 문은 조건절 값이 True 이면, 계속 실행된다.    
• if 문은 조건절 값이 완료되면 끝난다.    
• e.g. 3번 실행하라고 하면 3번만 실행하고 종료    
• while 문은 조건절 상태가 Ture(예를 들면, 0 < 5 )가 되면 무한대로 실행한다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Change the loop so that it counts **from 0 up to 9** (inclusive).

* Be careful not to alter or remove the count += 1 statement. If your program has no way to increase count, your loop could go on forever and become an infinite loop which could crash your computer/browser!    


**설명:** [ Instruction ]          
• 반복문을 9(포함)까지 세는 프로그램으로 변경하라. (현재는 4까지 셈)   
• 변수 count 가 증가하지 않으면, 무한대로 반복되는 프로그램이 될 수 있다.    
• 이럴 경우 컴퓨터에 문제가 발생할 수 있으니 주의하라.  
{: .notice--info}



<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* To make sure your loop counts up to 9, your condition should be 'count < 10' (or count <= 9).


**설명:** [ Hint ]         
• 9 까지만 실행되는 조건문을 만든다. ( count < 10 또는 count <= 9 )
{: .notice--info}


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
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• if 문은 1 번 출력한다.(조건문이 변수 count 가 10 보다 작은지만 비교)    
• while 문은 9 번 출력한다.(조건문이 변수 count 가 9 일때 까지, True 이다.)
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
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>    

### 2. Condition    

The condition is the expression that decides whether the loop is going to continue being executed or not. There are 5 steps to this program:

1. The loop_condition variable is set to True

2. The while loop checks to see if loop_condition is True. It is, so the loop is entered.

3. The print statement is executed.

4. The variable loop_condition is set to False.

5. The while loop again checks to see if loop_condition is True. It is not, so the loop is not executed a second time.    


**설명:** [ Learn ]     
• Ch2. Condition 에서는 조건절을 학습한다.    
• 조건절(loop_condition)은 반복(loop)을 계속할지 그만 할지를 결정하는 표현이다.     
• 다음 5단계로 진행된다.     
• ① 조건절의 변수값을 True 로 설정한다.       
• ② 조건절의 상태가 True 이면, 반복문 안으로 들어간다.    
• ③ print문을 출력한다.     
• ④ 조건절의 상태를 False 로 설정한다.    
• ⑤ while 문의 조건절을 다시 True 인지 확인한다.(True가 아니면 반복 종료 )
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* See how the loop checks its condition, and when it stops executing? When you think you've got the hang of it, click Run to continue.

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]          
• 실행이 멈췄을때, 반복문의 상태를 어떻게 확인 하는지 살펴보라.    
• 예상 한대로 실행되는지 Run 을 실행해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* See how the source works.



**설명:** [ Hint ]          
• 소스가 어떻게 동작하는지 확인하라. 
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

**설명:** [ Solution ]          
• 변수 loop_condition 을 True 로 설정한다.    
• 조건문이 True 이기에 while 문에 진입한다.    
• ( print "I am a loop" ) 를 출력한다.    
• 변수 loop_condition 을 강제로 False 로 변경한다.    
• 다시 while 문의 조건절 loop_condition 이 True 인지 확인한다.    
• 조건문이 True 이면, while 문의 블럭문이 실행된다.    
• 조건문이 False 이면, while 문을 빠져나간다.
{: .notice--info}


**결과** 
``` 
I am a loop
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>     

### 3. While you're at it    

Inside a while loop, you can do anything you could do elsewhere, including arithmetic operations. 



**설명:** [ Learn ]         
• Ch3. While you're at it 에서는 while 문의 조건문을 추가 학습한다.    
• while 조건문 에는 사칙연산을 비롯하여 다른 곳에서 사용했던 어떤 것이든 들어갈수 있다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a while loop that prints out all the numbers from 1 to 10 squared (1, 4, 9, 16, ... , 100), each on their own line.    
* Fill in the blank space so that our while loop goes from 1 to 10 inclusive.    
* Inside the loop, print the value of num squared. The syntax for squaring a number is num ** 2.    
* Increment num.



**설명:** [ Instruction ]          
• while 문을 사용하여 1 부터 10 까지 값의 제곱 값을 출력하라.    
• while 문의 조건문을 넣는 곳에 1 부터 10 까지 반복적으로 실행하도록 작성하라.       
• while 문의 내부실행 블럭에서는 ( num ** 2 ) 제곱 값을 출력하라.       
• 변수 num 을 1 씩 증가 시켜라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>

* Your condition will have to be num <= 10 (or num < 11) so that the loop will always print until num is 11.


**설명:** [ Hint ]          
• 조건문 num <= 10 또는 num < 11 로 10 이하 인지를 확인한다. 
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

**설명:** [ Solution ]          
• 변수 num 에 값 1 로 초기화 한다.    
• while 문에서 조건문 num <= 10 으로 정의 하였다.    
• while 문 조건은 변수 num 이 10 이하 일때까지 실행한다(True).      
• while 실행 블럭에서는 num ** 2 하여 제곱을 구하고 출력한다.     
• 마지막으로 변수 num 을 값 1 을 증가 시킨다.     
• 다시, while 조건문에서 변수 num 이 10 보다 같거나 작으면 실행블럭이 동작한다(True).
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
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>     

### 4. Simple errors    

A common application of a while loop is to check user input to see if it is valid. For example, if you ask the user to enter y or n and they instead enter 7, then you should re-prompt them for input.



**설명:** [ Learn ]         
• Ch4. Simple errors 에서는 연산자 같다( == ), 틀리다( != ) 를 학습한다.    
• 주로 while 조건문에서 사용한다.   
• 사용자가 입력한 값이 유효 한지를 체크하는 기능이다.    
• 예를들면, 당신은 사용자가 y 또는 n 을 입력하길 기대하고 있다.    
• 그런데, 사용자가 7 을 입력하면, 당신은 다시 입력하는 단계로 되돌아 갈 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Fill in the loop condition so the user will be prompted for a choice over and over while choice does not equal 'y' and choice does not equal 'n'.


**설명:** [ Instruction ]          
• Prompt 창에서 입력값이 y 또는 n 만 입력 되도록 하라.    
• while 조건문에서 통제 하도록 하라.    
• 만약 y 또는 n 이외의 값이 입력되면 다시 입력하도록 반복하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>

* Remember, use the != operator to test if two things are different, such as choice != "y", and the and operator to check more than one thing, such as A and B.


**설명:** [ Hint ]         
• 조건문에 연산자 ( != ) 를 사용한다.   
• y 또는 n 이외에는 True(참) 가 되지 않도록 한다.    
• 입력받은 비교 변수가 y 와 같지 않는지를 비교하는 것은 (e.g. !="y" ) 이다.    
• 연산자 ( and ) 는 A, B 모두 True(참) 이어야 한다(e.g. A and B ).
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
choice = raw_input('Enjoying the course? (y/n)')

while choice != 'y' and choice != 'n':  # Fill in the condition (before the colon)
  choice = raw_input("Sorry, I didn't catch that. Enter again: ")
```

**설명:** [ Solution ]          
• 변수 choice 에 입력값을 받아 저장한다.    
• while 문에서 변수 choice 가 y 도 아니고, n 도 아니다 를 비교한다.    
• 조건문이 True(참) 이면, 다시 입력문을 받는다.    
• 조건문이 False(거짓) 이면, while 문을 실행하지 않고 빠져나간다.
{: .notice--info}



**결과** 
``` 
Enjoying the course? (y/n)x
Sorry, I didn't catch that. Enter again: z
Sorry, I didn't catch that. Enter again: y
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>     

### 5. Infinite loops    

An infinite loop is a loop that never exits. This can happen for a few reasons:

1. The loop condition cannot possibly be false (e.g. while 1 != 2)

2. The logic of the loop prevents the loop condition from becoming false.

Example:    
```python
count = 10
while count > 0:
  count += 1 # Instead of count -= 1
```



**설명:** [ Learn ]          
• Ch5. Infinite loops 에서는 무한반복(loop)을 방지하는 방법을 학습한다.    
• 무한 loop 는 프로그램을 빠져 나가지 않고 계속 반복되는 것이다.    
• 문한 loop 가 발생하는 원인은 다음과 같이 여러가지 이유가 있다.    
• ① 조건문 결과가 무조건 True 일때 ( while 1 !=2 )    
• ② 프로그램 로직상 false 가 발생할 수 없는 경우 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* The loop in the editor has **two problems**: it's missing a colon (a syntax error) and count is never incremented (logical error). The latter will result in an infinite loop, so be sure to **fix** both before running!

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]          
• while 반복문에 2 개의 문제가 있다.    
• 첫째는 문법적으로 ( : ) 이 빠져 있다.    
• 둘째는 로직적으로 무한 반복이 되는 것이다.    
• 프로그램을 실행하기 전에 수정하라.  
{: .notice--info}


<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Since count is never incremented (count += 1), count is always 0, and since zero is less than ten, 0 will be printed over and over again forever.


**설명:** [ Hint ]          
• 변수 count 가 증가하지 않으면 count 값은 항상 0 이다.   
• while 조건문이 항상 10 보다 작게 되며, 이경우는 조건문이 무조건 True 가 된다. 
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

**설명:** [ Solution ]          
• 변수 count 가 0 부터 10 보다 작을때까지 변수 count를 출력하는 프로그램이다.    
• 변수 count 에 값 1 을 증가 시켜준다.   
• 변수 count 가 10 이 되면 while 조건문을 빠져 나간다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>

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
<p style="page-break-before: always;"></p>
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





**설명:** [ Learn ]          
• Ch6. Break 에서는 break 문을 학습한다.    
• 반복문에서는 break 문을 만나면 현재 loop 를 빠져나간다.    
• while 문은 조건문에서 항상 True 인지를 확인한다. True가 아니면 loop 를 빠져나간다.    
• while 문 내부블럭에서 if 문을 사용해서 빠져나가도 된다.    
• if 문에 조건을 걸어서 해당 조건이 되면 break 사용하여 해당 loop 를 빠져나간다.     
• while 문과 if 문의 break 차이점은, while 문은 내부블럭이 1 번은 실행된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* See what the break does? Feel free to mess around with it (but make sure you don't cause an infinite loop)! Click Run when you're ready to continue.


**설명:** [ Instruction ]          
• break 문이 무슨일을 하는지 살펴보라.    
• 가볍게 살펴보고, 실행 시켜라.   
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ Hint ]          
• skip
{: .notice--info}


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

**설명:** [ Solution ]          
• While 문의 조건문이 항상 True 이다.    
• 변수 count 를 출력한다.    
• 변수 count 를 값 1 을 증가한다.    
• 변수 count 가 10 보다 같거나 크면 break 문이 동작된다. while 문을 빠져나간다.    
• 변수 count 가 10 보다 작으면 while 문이 다시 반복 실행된다.
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
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>     

### 7. While / else    

Something completely different about Python is the `while/else` construction. `while/else` is similar to `if/else`, but there is a difference: the **else** block will execute anytime the loop condition is evaluated to False. This means that it will execute if the loop is never entered or if the loop exits normally. If the loop exits as the result of a break, the else will not be executed.

In this example, the loop will break if a 5 is generated, and the else will not execute. Otherwise, after 3 numbers are generated, the loop condition will become false and the else will execute.





**설명:** [ Learn ]          
• Ch7. While / else 에서는 while/else 문을 학습한다.   
• while/else 문은 python에 사용되는 독특한 구조이다.    
• if/else 의 else 와 비슷하다.    
• 차이는, if/else 는 if 문이 실행되면 else 문은 실행되지 않는다.    
• while/else 는  while 문이 flase 되어 빠져 나오면 반드시 else 문이 동작된다.    
• 실습을 통해서 이해하자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Click Run to see while/else in action!


**설명:** [ Instruction ]          
• Run 실행후, 소스가 어떻게 동작 되는지를 확인하라.
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

**설명:** [ Solution ]          
• while 문은 변수 count 가 3 보다 작을 때까지 내부블럭이 실행된다.    
• 변수 count 가 3보다 크면 while 문을 빠져나온다. 그리고 else 문이 실행된다.    
• else 문의 *You win!* 이 출력된다.
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
<p style="page-break-before: always;"></p>
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
Remember, `raw_input` turns user input into a **string**, so we use `int()` to make it a number again.    





**설명:** [ Learn ]          
• Ch8. Your own while / else 에서는 while/else 의 사용법을 학습한다.    
• while/else 문이 어떤 경우에 사용 되는지는 살펴보자.     
• 참고로, 함수 raw_input() 는 return 값이 문자열(string)이다.    
• 즉, 입력을 숫자로 입력해도 내부적으로는 문자열로 취급된다.    
• 함수 int() 를 사용하여, int(raw_input("Your guess: ")) 숫자로 바꿔줘야 한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

* Use a while loop to let the user keep guessing so long as guesses_left is greater than zero.    
* Ask the user for their guess, just like the second example above.    
* If they guess correctly, print "You win!" and break.    
* Decrement guesses_left by one.    
* Use an else: case after your while loop to print "You lose.".    



**설명:** [ Instruction ]          
• 사용자가 계속 질문하는 while 문을 만들어라.    
• 조건문은 변수 guesses_left > 0 큰 경우다.    
• Learn 단계에서 설명하였던 내용을 참조하여 질문하는 문장을 만들어라.        
• 질문한 값이 맞으면 *You win!* 이라고 출력하고, break 문으로 빠져나온다.        
• 변수 guess_left 를 값 1 씩 줄여 나간다. (e.g. guess_left -= 1 )    
• else 문을 사용하여 while 문을 빠져나오면 *You lose.* 라고 출력한다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* This game will have a very similar structure to the example, but instead of losing right before the break, the user should win.

* The if should check if guess == random_number. If it does, then it's the winning guess!


**설명:** [ Hint ]          
• 앞의 예제와 비슷하지만, break 문이 걸리는게 승리 했을때 이다.    
• 승리의 조건은 다음과 같다.    
• e.g. if guess == random_number    
• Random 값은 while 문 시작 하기전에 산출된다.     
• break 문이 실행되어 while 문을 빠져나갈때, else 문은 실행되지 않는다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>

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

**설명:** [ Solution ]          
• 미리 변수 random_number 에 임의의 값을 생성한다.     
• while 문이 True (변수 guess_left > 0) 인경우 진행된다.     
• Prompt 창에서  Your guess: 로 임의의 숫자를 입력 받는다.    
• 입력받은 값은 변수 guess 에 저장된다.      
• 변수 guess 값이 미리 산출한 변수 random_number 와 같은지 비교한다.    
• 같으면, *You win!* 을 출력한다. 그리고 break 문이 작동되어 loop를 빠져나온다.    
• 틀리면 변수 guess_left 에 1 을 차감한다. 다시 while 문을 돈다.    
• 변수 guesses_left 의 값이 0 이 되면    
• while 문의 조건문은 False 가 된다. 그리고 while 문을 빠져나온다.    
• 이때, else 문이 실행되고, ( print "You lose" ) 가 출력된다.    
• 강제로 break 문이 실행되어 while 문을 빠져나오면 else 문이 실행 안된다.    
• while 문의 조건문이 True 에서 False 로 변경되어 while 문을 빠져나오면 else 문이 실행된다.
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
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>     

### 9. For your health    

An alternative way to loop is the for loop. The syntax is as shown in the code editor. This example means "for each number i in the range 0 - 9, print i".



**설명:** [ Learn ]          
• Ch9. For your health 에서는 for 문을 학습한다.    
• Editor 화면에 있는 소스는, 0 부터 9 까지 산출하여 반복적으로 돌면서 산출하는 소스이다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Make the loop print the numbers from 0 to 19 instead of 0 to 9.


**설명:** [ Instruction ]          
• 0 부터 19 까지 숫자를 출력하는 반복문으로 변경하라.    
• ( 기존 0 부터 9 까지 산출하는 소스를 변경한다. ) 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

• Make sure to change the number inside of `range`.


**설명:** [ Hint ]          
• 내부 함수 range() 를 사용한다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print "Counting..."

for i in range(20):
  print i
  
  
```

**설명:** [ Solution ]          
• 함수 range(20) 는 20 미만의 숫자를 0 부터 20 개 산출한다.
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
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>     

### 10. For your hobbies    

This kind of loop is useful when you want to do something a **certain number of times**, such as append something to the end of a list.



**설명:** [ Learn ]          
• for 문은 내가 몇번 loop 를 돌려야 하는지를 정확히 알때 사용한다.     
• 예를 들면, 리스트의 끝에 항목값을 추가할때 사용한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a `for` loop that prompts the user for a **hobby 3 times**.    
* Save the result of each prompt in a `hobby` variable    

* append each one to `hobbies[]`.    

* print hobbies after your for loop    

* Make sure to answer the prompts in the terminal when testing your code!    



**설명:** [ Instruction ]          
• for 문을 사용하여 취미를 3 번 묻는 프로그램을 작성하라.    
• 변수 hobby 에 prompt 에서 입력받은 값을 저장하라.      
• 변수 hobby 의 값을 리스트 hobbies 에 추가하라.    
• for 문을 빠져나온다.    
• 리스트 hobbies 값을 출력하라. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Your for loop should use range(3). You should use the `raw_input()` function to get info from the user and `hobbies.append(hobby)` to add the `hobby` to the list.


**설명:** [ Hint ]          
• 함수 raw_input() 를 사용하라.     
• 리스트에 추가하는 방법은 다음과 같다.    
• e.g. hobbies.append(hobby)
{: .notice--info}


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

**설명:** [ Solution ]          
• for 문에서 3 번 돌도록 산출된다.(e.g. range(3))    
• 함수 raw_input() 으로 입력값을 받아서, 변수 hobby 에 저장한다.    
• 리스트 hobbies 에 변수 hobby 의 값을 추가한다.    
• 3번 입력이 끝나고, for 문을 빠져나온다.    
• 리스트 hobbies 를 출력한다. 
{: .notice--info}



**결과** 
``` 
Tell me one of your favorite hobbies: swim
Tell me one of your favorite hobbies: ski
Tell me one of your favorite hobbies: cycle
[u'swim', u'ski', u'cycle']
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>     

### 11. For your strings    

Using a for loop, you can print out each individual character in a string.

The example in the editor is almost plain English: "for each character c in thing, print c". 



**설명:** [ Learn ]          
• Ch11. For your strings 에서는 반복문으로 문자열을 관리하는 방법을 학습한다.    
• loop 반복을 통하여 문자열을 문자 단위로 나눌수 있다.     
• Editor 화면에 있는 소스는 문자열 단어를 스펠링으로 나누는 소스이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Add a second for loop so that each character in `word` is printed one at a time.


**설명:** [ Instruction ]          
• for 문을 추가하여, 변수 word 에 담겨 있는 문자열 eggs 를 문자 하나씩 출력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the example on lines 3 - 4 as a model.


**설명:** [ Hint ]          
• 3, 4 라인에 있는 for 문을 참조하라. 
{: .notice--info}

<p style="page-break-before: always;"></p>
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

**설명:** [ Solution ]          
• 변수 word 에 있는 문자열 *eggs!* 를 알파벳 하나씩 읽어서 출력한다.     
• 문자열도 문자별 index 를 가지고 있다. 
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
<p style="page-break-before: always;"></p>
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



**설명:** [ Learn ]          
• Ch12. For your A 에서는 문자열의 문자를 비교하는 방법을 학습한다.    
• for 문은 문자열을 조작하기 편리하다.    
• 예제에서 Marble 가 M a r b l e 로 출력된다.    
• 문자열이 새로운 줄에서 출력되는 것이 아니라,     
• 같은 라인에서 출력되게는 다음과 같이 한다.    
• e.g. print char ,   --> ( , ) comma 를 해준다.  
{: .notice--info}


**설명:** [ Python3 ]          
• Python2 에서는 줄을 바꾸지 않고 출력하려면 comma ( , )를 사용한다.    
• Python3 에서는 다음과 같이 키워드 인자 end="" 사용해야 한다.    
• e.g print("Hello", end="")    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

* Let's filter out the letter "A" from our string.

* Do the following for each character in the `phrase`.
* If char is an "A" or char is an "a", print "X", instead of char. Make sure to include the trailing comma.
* Otherwise (else:), please print char, with the trailing comma.



**설명:** [ Hint ]          
• 문자열 중 A 를 걸러내자.         
• 변수 phrase 에 들어있는 문자열을 이용한다.    
• 문자열 중 A 또는 a 는 해당 문자를 X 로 출력 되도록 수정한다.    
• ( , ) 를 사용하여 한 줄에 출력하라.        
• 그 외 문자는 는 ( , ) 를 사용하여, 문자열 그대로 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can use the same for syntax, for c in s, as before. Use an if to compare c to 'a' and 'A'. Print an 'X' in that case, and use an else to print the character otherwise.

* Include a comma after the character to be printed in order to ensure it's not printed on its own line, like so:

```python
if c == "A" or c == "a":
  print "X",
```


**설명:** [ Hint ]          
• for 문을 돌면서 문자를 하나씩 추출한다.   
• 해당 문자가 A 또는 a 이면 문자열 X 를 출력한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>

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

**설명:** [ Solution ]      
• 변수 phrase 에 문자열 *A bird in the hand...* 가 저장되어 있다.    
• for 문으로 변수 phrase 의 문자를 하나씩 추출하여 변수 char 에 저장한다.    
• 변수 char 에 A 또는 a 가 들어 있으면 문자 X 를 출력한다.    
• 그렇지 않으면 변수 char 를 출력한다.    
• 출력할때, ( , )를 사용하여 한줄에 출력된다. 
{: .notice--info}



**결과** 
``` 
X   b i r d   i n   t h e   h X n d . . .
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>     

### 13. For your lists    

Perhaps the most useful (and most common) use of for loops is to go through a list.

On each iteration, the variable `num` will be the next value in the list. So, the first time through, it will be 7, the second time it will be 9, then 12, 54, 99, and then the loop will exit when there are no more values in the list.

 



**설명:** [ Learn ]         
• Ch13. For your lists 에서는 리스트의 활용을 학습한다.    
• 리스트를 사용할때 for 문이 많이 유용하다.     
• for 문으로 리스트 numbers 의 값들을 하나식 추출할 수 있다.    
• 변수 num 에는 그 추출된 값들이 하나씩 들어 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write a second for loop that goes through the numbers list and prints each element squared, each on its own line.




**설명:** [ Instruction ]          
• 두번째 for 문을 통하여, numbers 의 값들을 꺼내어 그 값의 제곱을 구하여 출력하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the `**` operator for exponentiation.    

<p style="page-break-before: always;"></p>
<br>

* The rest of the loop should be very similar to the first one.


**설명:** [ Hint ]          
• ( ** ) 를 사용하여 제곱을 구하라.     
• for 문 사용법은 첫번째 for 문과 비슷하다. 
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
numbers  = [7, 9, 12, 54, 99]

print "This list contains: "

for num in numbers:
  print num

# Add your loop below!
for num in numbers:
  print num ** 2
```

**설명:** [ Solution ]          
• 변수 numbers 에 있는 값을 변수 num 에 대입하라.    
• 변수 num 의 제곱을 구하여 출력한다. 
{: .notice--info}


**결과** 
``` 
This list contains: 
7
9
12
54
99
49
81
144
2916
9801
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>    

### 14. Looping over a dictionary    

You may be wondering how looping over a dictionary would work. Would you get the key or the value?

The short answer is: you get the key which you can use to get the value.    

```python
d = {'x': 9, 'y': 10, 'z': 20}
for key in d:
  if d[key] == 10:
    print "This dictionary has the value 10!"
```    

1. First, we create a dictionary with strings as the keys and numbers as the values.
2. Then, we iterate through the dictionary, each time storing the key in key.
3. Next, we check if that key's value is equal to 10.
4. If so, we print "This dictionary has the value 10!"




**설명:** [ Learn ]          
• Ch14. Looping over a dictionary 에서는 딕셔너리 반복을 학습한다.    
• 딕셔너리의 경우 반복문을 어떻게 사용하는지를 알아보자.     
• 먼저 간단하게 이야기하면, key 로 값을 얻어 낼수 있다.  
• 먼저, key 와 value 로 구성된 딕셔너리를 만든다.      
• 딕셔너리의 key 를 반복적으로 꺼낸다.    
• 꺼낸 key 의 value 값이 10 인지를 비교한다.    
• value 값이 10 이면 *This dictionary has the value 10!* 을 출력한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On line 5, print the **key**, followed by a space, followed by the value associated with that key.

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]          
• 5 라인에서, key 를 출력하고, 공백을 하나 뛰고 key 의 value 를 출력하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* An easy way to print in the requested format is to use the , character, like so:     

```python
greeting = "Hello"
name = "World"

print greeting, name
# prints "Hello World"
```    

**설명:** [ Hint ]          
• ( , ) 를 사용하면, 같은 줄에 출력할 수 있다.
{: .notice--info}    



<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
d = {'a': 'apple', 'b': 'berry', 'c': 'cherry'}

for key in d:
  # Your code here!
  print key, d[key]
```

**설명:** [ Solution ]          
• key 는 문자열 'a' 이고, 그 값은 d[key] 로 나타낼 수 있다.  
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**결과** 
``` 
a apple
c cherry
b berry
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>     

### 15. Counting as you go    

A weakness of using this for-each style of iteration is that **you don't know the index** of the thing you're looking at. Generally this isn't an issue, but at times it is useful to know how far into the list you are. Thankfully the built-in `enumerate` function helps with this.

`enumerate` works by supplying a corresponding index to each element in the list that you pass it. Each time you go through the loop, index will be one greater, and item will be the next item in the sequence. It's very similar to using a normal for loop with a list, except this gives us an easy way to count how many items we've seen so far.



**설명:** [ Learn ]       
• Ch15. Counting as you go 에서는 리스트의 인덱스 값을 관리하는 방법을 학습한다.     
• for 문을 돌려 리스트의 항목을 추출하더라도, 그 항목의 인덱스는 알려주지 않는다.    
• 다만 그 값만 추출한다.    
• 이러한 약점은 함수 enumerate 를 사용하면 해당 값의 인덱스 값을 알수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* We don't want the user to see things listed from index 0, since this looks unnatural. Instead, the items should appear to start at index 1. Modify the print statement to reflect this behavior. See the Hint for help. 


**설명:** [ Instruction ]          
• 리스트의 index 를 출력하면 0 부터 출력된다.    
• 우리는 리스트 번호를 1 번 부터 번호를 매기는게 더 자연스럽다.    
• 비록 index 값이 0 부터 출력되지만, print 할때는 1 부터 하는것처럼 보이게 하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Instead of just printing index, print index + 1 !


**설명:** [ Hint ]          
• 출력할때, index 값에 +1 을 하여라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
choices = ['pizza', 'pasta', 'salad', 'nachos']

print 'Your choices are:'
for index, item in enumerate(choices):
  print index + 1, item
```

**설명:** [ Solution ]          
• index 값에 +1 을 하여 1 부터 보이게 한다. 
{: .notice--info}


**결과** 
``` 
Your choices are:
1 pizza
2 pasta
3 salad
4 nachos
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>     

### 16. Multiple lists    

It's also common to need to iterate over **two lists at once**. This is where the built-in `zip` function comes in handy.

`zip` will create pairs of elements when passed two lists, and will **stop at the end of the shorter list**.

`zip` can handle three or more lists as well!




**설명:** [ Learn ]          
• Ch16. Multiple lists 에서는 리스트 끼리 곱하는것을 학습한다.    
• 한번에 두개의 리스트를 반복적으로 사용해야 할 경우에,    
• 우리는 함수 zip() 를 이용할수 있다.     
• 함수 zip() 은 2개의 리스트를 쌍으로 만들어주고, 잛은 리스트의 기준에 맞춰진다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Compare each pair of elements and print the larger of the two.


**설명:** [ Instruction ]          
• 각 원소들의 쌍을 비교하고, 두개중 더 큰것을 출력하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>

`a` is an element from `list_a` and `b`is an element of `list_b`.

You have two options: Use an `if/else` statement to compare the two and print whichever is larger. Alternatively, you can use the `max` function that you learned in unit 4.


**설명:** [ Hint ]          
• list_a를 변수 a로 받고, list_b를 변수 b로 값을 받는다.    
• 그리고 각각의 변수를 if/else 를 사용하여 어느것이 더 큰지를 비교한다.     
• 또는 내장함수 max() 를 활용해도 된다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
list_a = [3, 9, 17, 15, 19]
list_b = [2, 4, 8, 10, 30, 40, 50, 60, 70, 80, 90]

for a, b in zip(list_a, list_b):
  # Add your code here!
    print max(a, b)
```

**설명:** [ Solution ]          
• 각각의 리스트를 변수 a, b로 받아서, 함수 max(a,b) 를 비교하여 큰값을 출력한다.
{: .notice--info}


**결과** 
``` 
3
9
17
15
30
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>     

### 17. For / else    

Just like with `while`, `for` loops may have an else associated with them.

In this case, the `else` statement is executed after the `for`, but only `if` the `for` ends normally—that is, not with a `break`. This code will break when it hits 'tomato', so the `else` block won't be executed.



**설명:** [ Learn ]          
• Ch17. For / else 에서는 for 문에 else 문 사용을 학습한다.    
• for 반복문은 else 문을 가질수 있다.    
• for 문이 다 실행되고, 빠져 나오면 마지막으로 else 문이 실행된다.    
• 단, for 문에서 break 가 발생되면, else 문은 실행되지 않는다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Click Run to see how for and else work together.


**설명:** [ Instruction ]          
• Run 을 실행시켜, 소스가 어떻게 동작되는지 확인한다. 
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

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
fruits = ['banana', 'apple', 'orange', 'tomato', 'pear', 'grape']

print 'You have...'
for f in fruits:
  if f == 'tomato':
    print 'A tomato is not a fruit!' # (It actually is.)
    break
  print 'A', f
else:
  print 'A fine selection of fruits!'
```

**설명:** [ Solution ]          
• for 문을 돌면서, 리스트 fruits 의 값이 *tomato* 이면,    
• *A tomato is not a fruit!* 가 출력되고 break 가 실행된다.    
• 이 경우는 else 가 실행되지 않는다.    
• 만약에 for 문에서 break 가 안걸리고 정상적으로 다 돌게 되면,    
• else 문이 마지막에 실행된다.
{: .notice--info}



**결과 1** 
```
# break 문을 만난 경우 
You have...
A banana
A apple
A orange
A tomato is not a fruit!
```
<p style="page-break-before: always;"></p>
<br>

**결과 2** 
```
# break 문을 만나지 못한  경우 
You have...
A banana
A apple
A orange
A tomato
A pear
A grape
A fine selection of fruits!
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font> 
### 18. Change it up     

As mentioned, the `else` block won't run in this case, since break executes when it hits **'tomato'**.



**설명:** [ Learn ]          
• Ch18. Change it up 에서는 for/else 를 계속 학습한다.    
• break 문이 실행되면(즉, *tomato* 가 있으면),    
• for/else 문의 else 문은 실행되지 않는다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Modify the code in the editor such that the `for` loop's `else` statement is executed.


**설명:** [ Instruction ]          
• for 문의  else 문이 동작 되도록 소스를 수정하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can change the contents of fruits or the contents of the for statement such that the loop doesn't break on "tomato".

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]          
• else 문이 실행되게 하려면 다음과 같이 하면 된다.    
• 리스트 fruits 의 내용이 *tomato* 가 없게 하거나,    
• if 문에서 *tomato* 가 일치 하지 않게 만들어, break 문이 작동하지 않게 만들면,    
• else 문이 실행된다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
fruits = ['banana', 'apple', 'orange', 'tomato', 'pear', 'grape']

print 'You have...'
for f in fruits:
  if f == 'tomato':
    print 'A tomato is not a fruit!' # (It actually is.)
  print 'A', f
else:
  print 'A fine selection of fruits!'
```

**설명:** [ Solution ]          
• 이 경우엔, break 문을 삭제 했다.    
• for 문이 실행되고, else 문도 실행 된다.
{: .notice--info}


**결과** 
``` 
You have...
A banana
A apple
A orange
A tomato is not a fruit!
A tomato
A pear
A grape
A fine selection of fruits!
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LOOPS</font>     

### 19. Create your own    

To wrap up this lesson, let's create our own `for/else` statement from scratch.




**설명:** [ Learn ]          
• Ch19. Create your own 에서는 for/else 문을 활용하는 방법을 학습한다.    
• 지금까지 배운것을 종합하여, for/else 문을 활용하여 자신만의 소스를 만들어 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Build your `for/else` statement in the editor. Execution of the `else` branch is optional, but your code should print a string of your choice to the editor regardless.


**설명:** [ Instruction ]          
• for/else 문을 사용하여 프로그램을 작성하라.    
• else 문이 실행되고 안되고는 자유다.    
• 하지만, 당신이 원하는대로 출력이 되어야 한다.  
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
test = ["bleh", "blah", "bloh"]

for x in test:
    print x
else:
    print "ok"
```

**설명:** [ Solution ]          
• 리스트 test 에 3 개의 값을 넣고, for/else 문을 돌린다.     
• 변수 x 에 리스트 test 의 값을 하나씩 추출하여, 출력한다.    
• for 문이 다 돌고 나면, 마지막에 else 문이 실행된다.
{: .notice--info}


**결과** 
``` 
bleh
blah
bloh
ok
```


<br>
<br>    
<br>    
