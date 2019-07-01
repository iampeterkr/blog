---
# layout : rchive
title: "String & Console Output"
permalink: /string-console-output/
excerpt: "We learn about String, Console, and Output Syntax."
# last_modified_at: 2019-01-30T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    
<hr style="border: solid 1px #dddddd ;">    
LESSON    

This lesson will introduce you to strings and console output in Python, including creating string literals, calling a variety of string methods, and using the "print" keyword.    

**설명:** [ 학습방향 ]     
이 장에서는 문자열의 콘솔 출력, 생성, 함수 등 콘솔에 출력하는 방법을 학습한다.
{: .notice--info}     
     
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 1. Strings     

Another useful data type is the **string**. A **string** can contain letters, numbers, and symbols.

```python
name = "Ryan"
age = "19"
food = "cheese"
```
In the above example, we create a variable `name` and set it to the string value `"Ryan"`.
We also set `age` to `"19"` and `food` to `"cheese"`.
Strings need to be within quotes.



**설명:** [ Learn ]      
• Ch1. Strings 에서는 문자열을 학습한다.    
• 문자열(string)은 문자와, 숫자와, 기호도 사용할 수 있다.     
• 문자열인데, 숫자도 사용할수 있다는 의미는 함수 int()를 활용하여 변환후 사용할수 있다.  
{: .notice--info}


<p style="page-break-before: always;"></p>     
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a new variable `brian` and assign it the string `"Hello life!"`.    

**설명:** [ Instruction ]    
• 변수 brian 를 만들고 *Hello life!* 를 대입하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Do you remember how to declare and assign variables in Python? If not, refresh your memory here!


**설명:** [ Hint ]     
• 문자열을 대입할때, 문자열의 양끝을 따옴표 ( " " ) or ( ' ' ) 를 사용하면 된다.     
• 아래 소스를 실행시켜 보면 아래와 같은 결과를 얻는다.
{: .notice--info}

```python
brian = "Hello life!"
brian1 = 'The man screamed "I love Python!" so that everyone could hear.'
brian2 = "The man screamed 'I love Python!' so that everyone could hear."

print (brian)
print (brian1)
print (brian2)
```

**결과**
```
Hello life!
The man screamed "I love Python!" so that everyone could hear.
The man screamed 'I love Python!' so that everyone could hear.
```

<p style="page-break-before: always;"></p>     
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
brian = "Hello life!"
```

**설명:** [ Solution ]    
• 문자열을 대입할때, 문자열 양 끝에 따옴표 ( " " ) or ( ' ' )를 사용한다. 
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

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 2. Practice     

Excellent! Let's get a little practice in with strings.


**설명:** [ Learn ]     
• Ch2. Practice 에서는 문자열 연습을 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Set the following variables to their respective phrases:

  *  Set `caesar` to "Graham"    
  *  Set `praline` to "John"    
  *  Set `viking` to "Teresa"    


**설명:** [ Instruction ]    
• 변수 caesar = "Graham" 을 대입    
• 변수 praline = "John"  을 대입  
• 변수 viking = "Teresa" 을 대입
{: .notice--info}


<p style="page-break-before: always;"></p>     
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Make sure you use exactly the capitalization shown! Python takes things very literally.


**설명:** [ Hint ]    
• Python은 문자열의 대/소문자를 구별한다. 정확하게 사용해야 한다.
{: .notice--info}

<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Assign your variables below, each on its own line!

caesar = "Graham"
praline = "John"
viking = "Teresa"

# Put your variables above this line

print caesar
print praline
print viking
```    

**설명:** [ Solution ]    
• 각 변수에 문자열을 대입한다. 
{: .notice--info}



**결과**
```
Graham
John
Teresa
```    
<p style="page-break-before: always;"></p>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)   
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 3. Escaping characters     

There are some characters that cause problems. For example:

```python
'There's a snake in my boot!'
```

This code breaks because Python thinks the apostrophe in 'There's' ends the string. We can use the backslash to fix the problem, like this:

```python
'There\'s a snake in my boot!'
```


**설명:** [ Learn ]       
• Ch3. Escaping characters 에서는 `\` 사용법을 학습한다.    
• 우리는 문자열을 만들때, 따옴표( ' ' )를 사용해야 한다고 앞에서 배웠다.    
• 가령 'There's' 라는 문자열을 만들때 Python은 따옴표 ( ' )를 쿼터로 인식한다.     
• 이런 경우는 ( ' ) 가 쿼터가 아님을 표시해주는 `\` 를 앞에 둔다.    
• Python 은 `\` 이면 다음 문자를 단순 문자로 인식한다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    
* Fix the string in the editor!

```python
# The string below is broken. Fix it using the escape backslash!

'This isn't flying, this is falling with style!'
```

**설명:** [ Instruction ]     
• 문자열 *ist't* 를 수정하여 정상적인 문자열로 만들어라.  
{: .notice--info}


<p style="page-break-before: always;"></p>     
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* You can escape the ' just by adding a ' before it: \'.

* There's another way to fix this problem. Can you think of it?

* You cannot pass this exercise with the other methods.

**설명:** [ Hint ]    
• `\` 를 사용하라. 
{: .notice--info}


<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# The string below is broken. Fix it using the escape backslash!

'This isn\'t flying, this is falling with style!'
```

**설명:** [ Solution ]    
• 문자열 *isn't'* 를 *isn\'t* 로 수정 한다.     
• 또다른 방법은 가장 바깥쪽 문자열 쿼터 ( ' ' ) 를 ( " " ) 로 바꾸어 준다.   
{: .notice--info}

```python
# The string below is broken. Fix it using the escape backslash!

a = 'This isn\'t flying, this is falling with style!'

b = "This isn\'t flying, this is falling with style!"

print (a)
print (b)

```

**결과**
```
This isn't flying, this is falling with style!
This isn't flying, this is falling with style!
```    

<p style="page-break-before: always;"></p>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)   
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 4. Access by Index    

Great work!

Each character in a string is assigned a number. This number is called the index. Check out the diagram in the editor.
```python
c = "cats"[0]
n = "Ryan"[3]
```
1. In the above example, we create a new variable called `c` and set it to `"c"`, the character at index zero of the string `"cats"`.

2. Next, we create a new variable called `n` and set it to `"n"`, the character at index three of the string `"Ryan"`.

Notice that in the first `"cat"` example we are calling the 0th letter of `"cat"` and getting `"c"` in return. This is because in Python indices begin counting at 0. Therefore, in the string `"cats"`, the first letter, `"c"`, is at the 0th index and the last letter, `"s"`, is at the 3rd index.

```
+---+---+---+---+
| c | a | t | s |
+---+---+---+---+
  0   1   2   3  

+---+---+---+---+
| R | y | a | n |
+---+---+---+---+
  0   1   2   3  
```


**설명:** [ Learn ]       
• Ch4. Access by Index 에서는 문자열 주소 접근법을 학습한다.    
• 문자열은 위와 같이 메모리에 저장된다.    
• 그 메모리에는 0 번 부터 주소(index)가 매겨진다.  
{: .notice--info}

```python
"""
The string "PYTHON" has six characters,
numbered 0 to 5, as shown below:

+---+---+---+---+---+---+
| P | Y | T | H | O | N |
+---+---+---+---+---+---+
  0   1   2   3   4   5

So if you wanted "Y", you could just type
"PYTHON"[1] (always start counting from 0!)
"""
```

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On line 13, assign the variable `fifth_letter` equal to the fifth letter of the string "MONTY".

* Remember that the fifth letter is not at index `5`.    
* Start counting your indices from zero.


**설명:** [ Instruction ]     
• 변수 fifth_letter 에 *MONTY* 중 5 번째 글자만 대입하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* The letter you want is *Y*.


**설명:** [ Hint ]    
• 문자열 *MONTY* 에서 *Y* 만 출력 할려면 변수에 *Y* 만 대입해야 한다.
{: .notice--info}

<p style="page-break-before: always;"></p>     
<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
"""
The string "PYTHON" has six characters,
numbered 0 to 5, as shown below:

+---+---+---+---+---+---+
| P | Y | T | H | O | N |
+---+---+---+---+---+---+
  0   1   2   3   4   5

So if you wanted "Y", you could just type
"PYTHON"[1] (always start counting from 0!)
"""
fifth_letter = "MONTY"[4]

print fifth_letter
```    

**설명:** [ Solution ]    
• 문자열 *MONTY* 에서 *Y* 만 출력 할려면 *Y*가 다섯번째에 있는 글자 이다.    
• 하지만, 실제 인덱스 주소에는 4 번에 저장되어 있다.    
• "MONTY"[4] 즉, 4 번째 주소에 있는 글자만 변수에 대입해야 한다. 
{: .notice--info}

**결과**
```
Y
```
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 5. String methods    

Great work! Now that we know how to store strings, let's see how we can change them using string methods.

String methods let you perform specific tasks for strings.

We'll focus on four string methods:

*  `len()`    
*  `lower()`    
*  `upper()`    
*  `str()`    


Let's start with `len()`, which gets the length (the number of characters) of a string!


**설명:** [ Learn ]       
• Ch5. String methods 에서는 문자열 관련 함수를 학습한다.    
• 함수 len() 는 문자의 갯수를 알려주는 함수이다. 
{: .notice--info}



<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On line 1, create a variable named `parrot` and set it to the string "Norwegian Blue".

* On line 2, type `len(parrot)` after the word print, like so: `print len(parrot)`.    
* The output will be the number of characters in "Norwegian Blue"!


**설명:** [ Instruction ]    
• 1번 라인에, 변수 parrot 를 만들어라.    
• 변수 parrot 에 문자열 "Norwegian Blue" 를 대입하라.    
• 2번 라인에, print len(parrot) 라고 작성하자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the function `len()`.  


**설명:** [ Hint ]    
• 함수 len() 에 변수를 삽입하여 해당 변수에 들어 있는 문자의 갯수를 셀 수 있다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
parrot = "Norwegian Blue"
print len(parrot)
```

**설명:** [ Solution ]    
• 함수 len()의 Parameter로 parrot 변수를 넣었다.    
• print 문으로 len(parrot) 를 출력하였다.    
• 변수 parrot 에 들어있는 문자열 *Norwegian Blue* 의 문자 갯수가 출력된다.    
• 그런데, 예상된 문자 갯수가 13개가 아니라, 14개가 출력 된다.    
• 이유는 공백(space)도 하나의 문자로 계산한다.    
• 중간에 공백을 몇개 넣고 RUN 해보면 바로 알수 있다.
{: .notice--info}


**결과**
```
14
```
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)     
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 6. lower()    

Well done!

You can use the `lower()` method to get rid of all the capitalization in your strings. You call `lower()` like so:

```python
"Ryan".lower()
```    
which will return "ryan".



**설명:** [ Learn ]     
• Ch6. lower() 에서는 메서드 lower()를 학습한다.    
• 함수 lower() 는 대문자를 모두 소문자로 변경하여 반환한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Call `lower()` on parrot (after print) on line 3 in the editor.


**설명:** [ Instruction ]    
• 변수 parrot 의 담긴 문자열을 함수 lower() 를 사용하여, 라인 3에서 출력하라. 
{: .notice--info}


<p style="page-break-before: always;"></p>     
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Your code should look something like this:    

```python
print parrot.lower()
```    


**설명:** [ Hint ]    
• 함수 parrot.lower() 사용하라.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
parrot = "Norwegian Blue"

print parrot.lower()
```     

**설명:** [ Solution ]    
• 문자열에 ( . ) 을 붙이고 lower() 를 사용할 수 있다.    
• 변수에도 동일하게 ( . ) 을 붙이고 함수 lower() 를 사용할 수 있다. 
{: .notice--info}


**결과**
```
norwegian blue
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 7. upper()    
 
Now your **string** is 100% lower case! A similar method exists to make a string completely upper case.

**설명:** [ Learn ]     
• Ch7. upper() 에서는 메서드 upper()를 학습한다.     
• 함수 upper() 는 문자열을 모두 대문자로 바꿔주는 함수이다.  
{: .notice--info}



<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Call `upper()` on parrot (after print on line 3) in order to capitalize all the characters in the string!


**설명:** [ Instruction ]     
• 변수 parrot 을  함수 upper() 를 사용하여 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Use the same syntax as the previous exercise! Last time, you used:    

```python
print parrot.lower()
```    


**설명:** [ Hint ]    
• 이전에 연습한 함수 lower() 사용법을 참조하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
parrot = "norwegian blue"

print parrot.upper()
```     


**설명:** [ Solution ]     
• 문자열에 ( . ) 을 붙이고 함수 upper() 를 사용할 수 있다.     
• 변수에도 ( . ) 을 붙이고 함수 upper() 를 사용할 수 있다.  
{: .notice--info}


**결과**
```
NORWEGIAN BLUE
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 8. str()    

Now let's look at `str()`, which is a little less straightforward. The `str()` method turns non-strings into strings! For example:    

```python
str(2)
```    

would turn `2` into `"2"`.




**설명:** [ Learn ]     
• Ch8. str() 에서는 메서드 str()를 학습한다.     
• 함수 str() 는 문자열이 아닌것을 문자열로 변환해 준다.    
• e.g. integer 2 를 string "2" 로 변환해 준다.     
• e.g. float 2.0 를 string "2.0" 로 변환해 준다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a variable `pi` and set it to `3.14` on line 4.

* Call `str(pi)` on line 5, after print.    


**설명:** [ Instruction ]    
• 변수 pi 를 만들고, 3.14 를 대입하라.    
• 라인 5 에서, str(pi) 를 사용하고, 출력하라. 
{: .notice--info}


<p style="page-break-before: always;"></p>     
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* The `str()` syntax is like the `len()` syntax:    

```python
str(pi)
```

**설명:** [ Hint ]    
• 함수 str() 사용법은 함수 len() 사용법과 같다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
"""Declare and assign your variable on line 4,
then call your method on line 5!"""

pi = 3.14
print str(pi)
```

**설명:** [ Solution ]    
• float 변수 pi 에 실수 3.14 를 대입한다.    
• 변수 pi 를 출력 할때는 str() 을 사용하여 문자열로 변환하여 출력 해야한다.  
{: .notice--info}


**결과**
```
3.14
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 9. Dot Notation    

Let's take a closer look at why you use `len(string)` and `str(object)`, but dot notation (such as `"String".upper()`) for the rest.    

```python
lion = "roar"
len(lion)
lion.upper()
```    
Methods that use dot notation only work with strings.

On the other hand, `len()` and `str()` can work on other data types.    

**설명:** [ Learn ]       
• Ch9. Dot Notation 에서는 메서드 접근법을 학습한다.    
• 문자열(대문자, 소문자)을 변환 할때는 ( . ) 을 사용한다.    
• 데이타 type 을 변환 할때는 함수 len() , str() 을 사용한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On line 3, call the `len()` function with the argument `ministry`.

* On line 4, invoke the `ministry's .upper()` function.


**설명:** [ Instruction ]     
• 라인 3에서는 함수 len() 를 사용하여 출력하라.    
• 라인 4에서는 함수 .upper() 를 사용하여 출력하라.
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
ministry = "The Ministry of Silly Walks"

print len(ministry)
print ministry.upper()
```

**설명:** [ Solution ]     
• 함수 len(ministry) 는 변수 ministry 의 길이를 반환한다.    
• ministry.upper() 는 변수 ministry 의 문자열을 대문자로 변환한다.    
• *주의)* 변수 ministry 의 저장되어 있는 내용은 변하지 않는다. 
{: .notice--info}



**결과**
```
27
THE MINISTRY OF SILLY WALKS
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)   
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 10. Printing Strings    

The area where we've been writing our code is called the **editor**.

The **console** (the window to the right of the editor) is where the results of your code is shown.

`print` simply displays your code in the console.



**설명:**  [ Learn ]      
•Ch10. Printing Strings 에서는 문자열 출력방법을 학습한다.    
• print 는 editor 화면에서 작성한 프로그래밍을 console 창에 보여준다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Print "Monty Python" to the console.


**설명:** [ Instruction ]    
• 문자열 "Monty Python" 을 console 에 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* The syntax looks like this:

```python
print "Your string goes here"
```

**설명:** [ Hint ]     
• print 문을 사용하여 문자열을 출력한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
"""Tell Python to print "Monty Python"
to the console on line 4!"""

print "Monty Python"
```

**설명:** [ Solution ]     
• print 문을 사용하여 문자열 "Monty Python" 을 출력한다. 
{: .notice--info}



**결과**
```
Monty Python
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)     
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 11. Printing Variables    

Great! Now that we've printed strings, let's print variables


**설명:** [ Learn ]      
• Ch11. Printing Variables 에서는 변수 출력을 학습한다.     
• print 문은 변수도 출력한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Declare a variable called `the_machine_goes` and assign it the string value "Ping!" on line 5.

* Go ahead and print `the_machine_goes` in line 6.


**설명:** [ Instruction ]     
• 라인 5에서, 변수 the_machine_goes 에 "Ping" 을 대입하라.    
• 라인 6에서, 변수 the_machine_goes 를 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Make sure you're setting your variable like this:

```python
the_machine_goes = "Ping!"
```
**설명:** [ Hint ]    
• 변수 the_machine_goes = "Ping!" 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
"""Assign the string "Ping!" to
the variable the_machine_goes on
line 5, then print it out on line 6!"""

the_machine_goes = "Ping!"
print the_machine_goes
```

**설명:** [ Solution ]    
• 변수 the_machine_goes 를 만들어라.    
• 변수 the_machine_goes 를 print 문을 사용하여 출력한다.
{: .notice--info}


**결과**
```
Ping!
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 12. String Concatenation    

You know about **strings**, and you know about arithmetic operators. Now let's combine the two!

```python
print "Life " + "of " + "Brian"
This will print out the phrase Life of Brian.
```

The `+` operator between strings will **'add'** them together, one after the other. Notice that there are spaces inside the quotation marks after Life and of so that we can make the combined **string** look like 3 words.

Combining strings together like this is called **concatenation**. Let's try concatenating a few strings together now!


**설명:** [ Learn ]      
• Ch12. String Concatenation 에서는 문자열 연결을 학습한다.     
• 문자열은 ( + ) 연산자를 사용하여 연결할수 있다.    
• 문자열을 ( + ) 연산자를 사용하여 연결하는것을 concatenations 이라고 한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Let's give it a try. Print the concatenated strings "Spam ", "and ", "eggs" on line 3, just like the example above.

* Make sure you include the spaces at the end of "Spam " and "and ".


**설명:** [ Instruction ]    
• 라인 3 에서, "Spam ", "and ", "eggs"를 연결하라.        
• 주의할 점은 "Spam" 과 "and" 문자뒤에 공백이 있어야 한다.    
• e.g. "Spam ",   "and "
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Make sure you include the spaces and use the correct capitalization.

**설명:** [ Hint ]    
• 문자열 "Spam "과 "and " 다음에 공백이 있다는것을 주의한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Print the concatenation of "Spam and eggs" on line 3!

print "Spam " + "and " + "eggs"
```

**설명:** [ Solution ]     
• Concatenation( + ) 는 문자 그대로 연결시켜 준다.    
• 임의로 공백을 주지 않으면 "Spamandeggs" 로 출력된다.    
• 문자열 (" ") 사이에 공백을 적절히 넣어줘야 한다. 
{: .notice--info}


**결과**
```
Spam and eggs
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 13. Explicit String Conversion    

Sometimes you need to combine a **string** with something that isn't a string. In order to do that, you have to convert the **non-string** into a **string**.

```python
print "I have " + str(2) + " coconuts!"
This will print I have 2 coconuts!.
```

The `str()` method converts **non-strings** into strings. In the above example, you convert the number `2` into a **string** and then you concatenate the strings together just like in the previous exercise.

Now try it yourself!


**설명:** [ Learn ]       
• Ch13. Explicit String Conversion 에서는 출력시 문자열 변환을 학습한다.     
• 문자열과 숫자를 concatenation 시킬때는 숫자를 문자열 형태로 바꿔 줘야한다.    
• 바꿔주지 않으면 Python 해석기(interpreter)는 Error를 발생시킨다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Run the code as-is. You get an error!

* Use `str()` to turn `3.14` into a string. Then run the code again.


**설명:** [ Instruction ]    
• Editor 화면의 소스를 Run 시키면 Error 가 발생한다.    
• 실수 3.14 를 함수 str() 를 사용하여 문자열 형태로 바꾸어라.    
• Run  시켜라.   
{: .notice--info}


<p style="page-break-before: always;"></p>     
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* The code to turn the number 2 into a string is `str(2)`.

* Can you convert the number `3.14` into a string?


**설명:** [ Hint ]    
• 숫자를 문자로 바꿔 주기 위해선, 함수 str() 를 사용한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Turn 3.14 into a string on line 3!

print "The value of pi is around " + str(3.14)
```

**설명:** [ Solution ]    
• 실수 3.14 를 문자열로 바꿔주는, 함수 str() 를 사용한다.    
• e.g. str(3.14) 로 변경 해야한다. 
{: .notice--info}



**결과**
```
The value of pi is around 3.14
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 14. String Formatting with %, Part 1    

When you want to print a variable with a **string**, there is a better method than **concatenating** strings together.

```python
name = "Mike"
print "Hello %s" % (name)
```

The `%` operator after the string is used to combine a string with variables. The `%` operator will replace the `%s` in the string with the string variable that comes after it.

If you'd like to print a variable that is an **integer**, you can **"pad"** it with zeros using **%02d**. The `0` means **"pad with zeros"**, the `2` means to pad to `2` characters wide, and the `d` means the **number** is a **signed integer** (can be positive or negative).

```python
day = 6
print "03 - %s - 2019" %  (day)
# 03 - 6 - 2019
print "03 - %02d - 2019" % (day)
# 03 - 06 - 2019
```

**설명:** [ Learn ]       
• Ch14. String Formatting with %, Part 1 에서는 문자열 치환을 학습한다.    
• 문자열을 출력 할때, % 옵션을 사용하여 해당 변수를 치환한다.     
• %s 는 문자 변수를 치환한다.    
• %d 는 정수 변수를 치환한다.    
• %d 는 옵션을 추가하면, 숫자 앞 부분을 0 으로 채운다.
{: .notice--info}    

**설명:** [ Python3 ]     
• python3 에서는 문자열 메서드 format() 을 사용한다.    
• %s 대신에, {0}, {1}, {2}, {3} 등 인자의 위치를 알려준다.    
• 사용은 다음과 같이 한다.    
• 'I am {0}, and i love {1}'.format('Peter', 'Python')    
• 출력은 다음과 같이 된다.    
• 'I am Peter, and i love Python
{: .notice--info}


<p style="page-break-before: always;"></p>     
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Take a look at the code in the editor.    
* What do you think it'll do? , Click Run when you think you know.


**설명:** [ Instruction ]     
• Editor 화면에 있는 소스를 실행하고, 당신이 예상한대로 출력 되는지 검토하라. 
{: .notice--info}



<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Think about `%` and `%()`    


**설명:** [ Hint ]     
• % 와  %() 를 어떻게 사용하는지를 생각하라.
{: .notice--info}


<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
string_1 = "Camelot"
string_2 = "place"

print "Let's not go to %s. 'Tis a silly %s." % (string_1, string_2)
```    

**설명:** [ Solution ]    
• 1 번째 %s 에는 변수 string_1 이 할당되어 출력된다.    
• 2 번째 %s 에는 변수 string_2 가 할당되어 출력된다.
{: .notice--info}


**결과**
```
Let's not go to Camelot. 'Tis a silly place.
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)   
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 15. String Formatting with %, Part 2    

Remember, we used the `%` operator to replace the `%s` placeholders with the variables in parentheses.

```python
name = "Mike"
print "Hello %s" % (name)
```

You need the same number of %s terms in a string as the number of variables in parentheses:

```python
print "The %s who %s %s!" % ("Knights", "say", "Ni")
# This will print "The Knights who say Ni!"
```

**설명:** [ Learn ]     
• Ch15. String Formatting with %, Part 2 에서는 문자열 치환을 학습한다.       
• %s 옵션으로 직접 문자열을 입력하여 치환한다.  
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Now it's your turn! We have ___ in the code to show you what you need to change!    

  * Inside the string, replace the three ___ with `%s`.    

  * After the string but before the three variables, replace the final ___ with a `%`.    

  * Hit Run.    

  * Answer the questions in the console as they pop up!     

  * Type in your answer and hit Enter.



**설명:** [ Instruction ]    
• ___ 에 %s 를 대입하라.    
• 치환 할 변수 앞에는 % 를 대입하라.    
• Run 클릭하라.    
• Console 에 질문이 나오면, 입력하고, Enter 키 를 누른다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Remember, the syntax is:

```python
print "%s" % (string_variable)
```
* The `\` character on line 5 is a continuation marker.     
* It simply tells Python that line 5 continues onto line 6.

**설명:**  [ Hint ]     
• %s 를 변수로 치환하는 문법을 사용한다.    
• `\` 는 문자열이 계속 된다는 것을 Python interpreter 에게 알려준다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
name = raw_input("What is your name? ")
quest = raw_input("What is your quest? ")
color = raw_input("What is your favorite color? ")

print "Ah, so your name is %s, your quest is %s, " \
"and your favorite color is %s." % (name, quest, color)
```    

**설명:** [ Solution ]    
• %s를 변수 치환 % 를 사용하여 치환한다.    
• Console 에서 질문에 답을 입력하고, Enter 키 를 누른다.    
• %s, %s, %s 에 %( name, quest, color) 값이 출력 된다.
{: .notice--info}


**결과**
```
What is your name? iampeter
What is your quest? earth
What is your favorite color? yellow
Ah, so your name is iampeter, your quest is earth, and your favorite color is yellow.
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 16. And Now, For Something Completely Familiar    

Great job! You've learned a lot in this unit, including:

Three ways to create strings

```python
'Alpha'
"Bravo"
str(3)
```
String methods

```python
len("Charlie")
"Delta".upper()
"Echo".lower()
```
Printing a string

```python
print "Foxtrot"
```
Advanced printing techniques

```python
g = "Golf"
h = "Hotel"
print "%s, %s" % (g, h)
```

**설명:** [ Learn ]       
• 이 장에서는 'String & Console Output' 에서 배운 내용들을 전체 복습한다.   
{: .notice--info}


<p style="page-break-before: always;"></p>     
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Let's wrap it all up!

  * On line 3, create the variable `my_string` and set it to **any string** you'd like.
  * On line 4, use `len()` to print the length of `my_string`.
  * On line 5, print the `.upper()` case version of `my_string`.


**설명:** [ Instruction ]    
• 변수 my_string 을 만들고, 당신이 원하는 문자를 대입하라.    
• 라인 4 에서 함수 len() 를 사용하여 변수 my_string 길이를 출력하라.    
• 라인 5 에서 함수 .upper() 를 사용하여 변수 my_string 의 문자열을 대문자로 모두 변환하라. 그리고 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* You can `print` a variable with a method all on one line, like so: 

``` python
print my_variable.upper()
```
**설명:** [ Hint ]    
• 함수 .upper() 를 사용하고, 출력하라. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    
```python
# Write your code below, starting on line 3!

my_string = "hey"
print len(my_string)
print my_string.upper()
```

**설명:** [ Solution ]    
• 변수 my_string 의 길이를 함수 len()를 사용하여 출력한다.    
• 변수 my_string 의 문자열을 함수 .upper() 를 사용하여 대문자로 출력한다. 
{: .notice--info}


**결과**
```
3
HEY
```