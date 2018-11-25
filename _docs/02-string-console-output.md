---
# layout : rchive
title: "String & Console Output"
permalink: /string-console-output/
excerpt: "We learn about String, Console, and Output Syntax."
last_modified_at: 2018-11-21T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    
    
<hr/>


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



**설명:** 문자열(string)은 문자와, 숫자와, 기호도 사용할 수 있다. 스트링인데, 숫자도 사용할수 있다는 의미는 int()로 변화하여 사용할수 있다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a new variable `brian` and assign it the string `"Hello life!"`.


**설명:** ① 변수 `brian`를 만들고 `"Hellow life!"`를 대입하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Do you remember how to declare and assign variables in Python? If not, refresh your memory here!

There is no difference between using single quotes ' and double quotes ". However, sometimes it is helpful to use one or the other. If we want to include an apostrophe in our string, it would be smart to use double quotes to create the string like "I'm a string". If we want to use quotes in the string, we might want to create the string with single quote like 'The man screamed "I love Python!" so that everyone could hear.'


**설명:** 문자열을 대입할때, 양 끝을 `" "`or `' '`를 만들면 된다. 아래 소스를 실행시켜 보면 아래와 같은 결과를 얻는다.
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

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
brian = "Hello life!"
```

**설명:** 문자열을 대입할때, 양 끝을 `" "`or `' '`를 사용한다. 
{: .notice--info}

**결과**
```
```


<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 2. Practice 

Excellent! Let's get a little practice in with strings.


**설명:** 문자열 연습을 해보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Set the following variables to their respective phrases:

1 Set caesar to "Graham"
2 Set praline to "John"
3 Set viking to "Teresa"


**설명:** ① 변수 `caesar`, `praline`, `viking`에 각각 해당 문자열 `Graham`, `John`, `Teresa`를 대입하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Make sure you use exactly the capitalization shown! Python takes things very literally.


**설명:** Python은 문자열의 대/소문자를 구별한다. 정확하게 사용하라.
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

**결과**
```
Graham
John
Teresa
```
<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
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


**설명:** 우리는 문자열을 `' '`을 사용한다고 했다. 가령 **There's** 라는 문자열을 만들때 Python은 `'`를 쿼터로 인식하게 된다. 이런 경우는 `'`가 쿼터가 아님을 표시해주는 `\`를 앞에 두어 Python에게 `'`가 단순 문자임을 알게 해준다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    
Fix the string in the editor!
**①** 본문의 문자열을 바르게 수정해라. 
```python
# The string below is broken. Fix it using the escape backslash!

'This isn't flying, this is falling with style!'
```

**설명:** ① **ist't** 를 수정하여 정상적인 문자열을 만들어라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

You can escape the ' just by adding a ' before it: \'.

There's another way to fix this problem. Can you think of it?

You cannot pass this exercise with the other methods.

**설명:**  `\'` 를 참조하라. 
{: .notice--info}

<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# The string below is broken. Fix it using the escape backslash!

'This isn\'t flying, this is falling with style!'
```

**설명:** **isn't**' 를 **isn\'t** 로 수정 한다. 또다른 방법으로 가장 바깥쪽 문자열 쿼터 `' '` 를 `" "` 로 바꾸어 준다.   
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

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
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
① In the above example, we create a new variable called `c` and set it to `"c"`, the character at index **zero** of the string `"cats"`.

② Next, we create a new variable called `n` and set it to `"n"`, the character at index **three** of the string `"Ryan"`.

Notice that in the first `"cat"` example we are calling the 0th letter of `"cat"` and getting `"c"` in return. This is because in Python indices begin counting at **0**. Therefore, in the string `"cats"`, the first letter, `"c"`, is at the **0th** index and the last letter, `"s"`, is at the **3rd** index.

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


**설명:** 문자열은 위와 같이 메모리에 저장되며, 그 메모리에는 0번부터 주소(index)가 매겨진다.  
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

**①** On line **13**, assign the variable `fifth_letter` equal to the **fifth** letter of the string **"MONTY"**.

Remember that the fifth letter is not at index 5. Start counting your indices from zero.


**설명:** ① 변수 `fifth_letter`에 "MONTY" 중 5번째 글자만 대입하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
The letter you want is **"Y"**.


**설명:** 문자열 "MONTY" 에서 "Y" 만 출력 할려면 변수에 "Y" 만 대입해야 한다.
{: .notice--info}

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
**설명:** 문자열 "MONTY" 에서 "Y" 만 출력 할려면 "Y"가 다섯번째에 있는 글자이지만, 실제 인덱스 주소에는 4번에 저장되어 있으므로, **"MONTY"[4]** 즉, 4번째 주소에 있는 글자만 변수에 대입해야 한다. 
{: .notice--info}

**결과**
```
Y
```


<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 5. String methods


Great work! Now that we know how to store strings, let's see how we can change them using **string methods**.

**String methods** let you perform specific tasks for strings.

We'll focus on four string methods:

1 `len()`    
2 `lower()`    
3 `upper()`    
4 `str()`    


Let's start with `len()`, which gets the length (the number of characters) of a string!


**설명:** 함수 `len()` 는 문자의 갯수를 알려주는 함수 이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** On line 1, create a variable named parrot and set it to the string "Norwegian Blue".

On line 2, type len(parrot) after the word print, like so: print len(parrot). The output will be the number of characters in "Norwegian Blue"!


**설명:** ① 1번 라인엣 변수 `parrot`를 만들고 "Norwegian Blue" 를 대입하라. 2번 라인에서는 `print len(parrot)` 라고 작성하자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
let() 함수를 사용하자 


**설명:** len() 함수에 변수를 삽입하여 해당 변수에 들어 있는 문자의 갯수를 셀 수 있다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
parrot = "Norwegian Blue"
print len(parrot)
```

**설명:** `len()` 함수에 인자로 `parrot`변수를 넣고 `print`문으로 `len(parrot)`를 출력하면 변수 `parrot`에 들어있는 "Norwegian Blue"의 문자 갯수가 출력된다.
그런데, 문자갯수가 13개가 아니라, 14개인 이유는 공백(space)도 하나의 문자로 계산한다.
(중간에 공백을 몇개 넣고 RUN 해보면 바로 알수 있다.) 
{: .notice--info}


**결과**
```
14
```

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 6. lower()

Well done!

You can use the `lower()` method to get rid of all the capitalization in your strings. You call `lower()` like so:

```python
"Ryan".lower()
which will return "ryan".
```


**설명:**  lower() 함수는 문자열중 대문자를 모두 소문자로 변경 해 준다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Call `lower()` on parrot (after print) on line 3 in the editor.


**설명:** ① 변수 `parrot`의 담긴 문자열을 `lower()` 함수를 사용하고, 라인 3에서 출력 해라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Your code should look something like this:
```python
print parrot.lower()
```

**설명:**  변수 parrot.lower() 사용하라.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
parrot = "Norwegian Blue"

print parrot.lower()
```

**설명:** 문자열에 `.`을 붙이고 `lower()`를 사용할수도 있지만, 변수에도 동일하게 `.` 을 붙이고 `lower()`함수를 사용할수 있다. 
{: .notice--info}


**결과**
```
norwegian blue
```
<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 7. upper()
 
Now your **string** is 100% lower case! A similar method exists to make a string completely upper case.

**설명:** 함수 `upper()` 는 문자열을 모두 대문자로 바꿔 주는 함수이다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Call `upper()` on parrot (after print on line 3) in order to capitalize all the characters in the string!


**설명:** ① 변수 `parrot`를 `upper()` 함수를 사용하여 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Use the same syntax as the previous exercise! Last time, you used:
```python
print parrot.lower()
```

**설명:** 사전에 연습한 `lower()` 함수와 사용법을 참조하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
parrot = "norwegian blue"

print parrot.upper()
```

**설명:** 문자열에 `.`을 붙이고 `upper()`를 사용할수도 있지만, 변수에도 동일하게 `.` 을 붙이고 `upper()`함수를 사용할수 있다.  
{: .notice--info}


**결과**
```
NORWEGIAN BLUE
```
<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 8. str()

Now let's look at `str()`, which is a little less straightforward. The `str()` method turns non-strings into strings! For example:
```python
str(2)
```
would turn `2` into `"2"`.




**설명:** `str()` 함수는 문자열이 아닌것을(ex. integer, float)문자열로 바꿔주는 함수이다. ex) integer `2` 를 string `"2"`로 바꿔 준다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a variable `pi` and set it to `3.14` on line 4.

Call `str(pi)` on line 5, after print.


**설명:** ① 변수 `pi`를 만ㄷ르고, 값 `3.14`를 대입하라. 그리고, 라인 5에서, `str(pi)`를 사용하고, 출력하여라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
The str() syntax is like the len() syntax:

str(pi)The str() syntax is like the len() syntax:
```python
str(pi)
```

**설명:** `str()`사용법은 `len()` 함수 사용법과 같다. 
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

**설명:** **float** 변수 `pi`에 실수 `3.14`가 들어가 있다. 이를 출력할때는 **string** 으로 바꿔어서 출력 해야 한다.  
{: .notice--info}


**결과**
```
3.14
```
<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 9. Dot Notation

Let's take a closer look at why you use len(string) and str(object), but dot notation (such as "String".upper()) for the rest.

lion = "roar"
len(lion)
lion.upper()
Methods that use dot notation only work with strings.

On the other hand, len() and str() can work on other data types.

**설명:** `.`은 같은 테이타 형에서 대문자, 소문자로 바꿀때 사용을 하고, `len()`, `str()`은 다른 테이타 형태의 변환을 시킬때 사용된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** On line 3, call the `len()` function with the argument `ministry`.

On line 4, invoke the `ministry's .upper()` function.


**설명:** ① 라인 3에서는 `len()` 함수를 사용하여, 출력하고, 라인 4에서는 `.upper()`를 사용하여 출력하여라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

**No answer**

**설명:** 힌트 없음 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
ministry = "The Ministry of Silly Walks"

print len(ministry)
print ministry.upper()
```

**설명:** `len(변수명)`, `변수명.upper()`를 사용하여  각 함수의 기능을 안다.
{: .notice--info}

<

**결과**
```
27
THE MINISTRY OF SILLY WALKS
```
<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 10. Printing Strings

The area where we've been writing our code is called the editor.

The console (the window to the right of the editor) is where the results of your code is shown.

`print` simply displays your code in the console.



**설명:** `print`는 Coding 창에서 작성한 프로그래밍 소스를 `console` 창에 보여주는 역할을 한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Print "Monty Python" to the console.


**설명:** ① "Monty Python" 을 콘솔에 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
The syntax looks like this:
```python
print "Your string goes here"
```

**설명:** `print`문을 사용하여 문자열을 출력한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
"""Tell Python to print "Monty Python"
to the console on line 4!"""

print "Monty Python"
```

**설명:** `print` 문을 사용하여 문자열을 출력한다. 
{: .notice--info}



**결과**
```
Monty Python
```
<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 11. Printing Variables

Great! Now that we've printed strings, let's print variables


**설명:** 이미 앞에서 사용해 봤지만, `print`문은 변수도 출력 할 수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Declare a variable called `the_machine_goes` and assign it the string value "Ping!" on line 5.

Go ahead and print `the_machine_goes` in line 6.


**설명:** ① 변수 `the_machine_goes`에 **"Ping"**을 대입하고, 변수 `the_machine_goes`를 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Make sure you're setting your variable like this:
```python
the_machine_goes = "Ping!"
```
**설명:** 우선 변수 `the_machine_goes`부터 만들고 대입하자.
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

**설명:** 변수 `the_machine_goes`를 만들고, 그 변수를 `print`문으로 출력한다.
{: .notice--info}


**결과**
```
Ping!
```
<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
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


**설명:** 각각의 문자열을 `+` 연산자를 사용하여 연결 할수 있다. 이를 **concatenations** 이라고 한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Let's give it a try. Print the concatenated strings **"Spam ", "and ", "eggs"** on line 3, just like the example above.

Make sure you include the spaces at the end of **"Spam " and "and ".


**설명:** ① "Spam ", "and ", "eggs"를 연결 시키는데, 주의할 점은 "Spam" 과 "and" 다음에 공백이 있어야 한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Make sure you include the spaces and use the correct capitalization.

**설명:** "Spam"과 "and" 다음에 공백이 있도록 주의 한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Print the concatenation of "Spam and eggs" on line 3!

print "Spam " + "and " + "eggs"
```

**설명:** `+`는 문자를 문자 그대로 연결 시키므로 임의로 공백을 주지 않으면 `Spamandeggs`로 출력된다. 문자열 `" "` 사이에 공백을 적절히 넣어 줘야 한다. 
{: .notice--info}


**결과**
```
Spam and eggs
```
<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
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


**설명:** 문자열과 숫자를 연결 시킬때는 숫자를 문자열 형태로 바꿔 줘야 한다. 그렇지 않으면 Python은 Error를 발생시킨다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Run the code as-is. You get an error!

Use `str()` to turn `3.14` into a string. Then run the code again.


**설명:** ① Coding 창의 소스를 `Run`시키면 Error가 발생한다. 우리는 실수 `3.14`를 `str()` 함수를 사용하여 문자열 형태로 바꿔 주고 `Run` 시켜라.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
The code to turn the number 2 into a string is str(2).

Can you convert the number 3.14 into a string?


**설명:** 숫자를 문자로 바꿔 주기 위해선 `str()`를 사용해야 한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Turn 3.14 into a string on line 3!

print "The value of pi is around " + str(3.14)
```

**설명:** 실수 `3.14`를 문자열로 바꿔주는 `str()`함수를 사용하여 `str(3.14)`로 변경 해줘야 한다. 
{: .notice--info}



**결과**
```
The value of pi is around 3.14
```
<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
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

**설명:** 문자열을 표현할때 `%` 옵션을 사용하여 해당 변수를 치환 할 수 가 있다. 
상기 Pytho 코드에서 보면, `%s` 문자열 변수를 치환해 주는 역할을 한다. 또다른 `%` 옵션으로 `%d`가 있다. 이것은 문자열 양수만 치환해 주는 역할을 한다. `%d`는 옵션을 추가 할수 있는데, 수자의 앞 부분을 `0` 채워주는 역할을 한다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Take a look at the code in the editor. What do you think it'll do? Click Run when you think you know.


**설명:** ① Edit 창에 있는 소스를 실행 시키고, 당신이 예상한대로 출력 되는지 검토하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Think about `%` and `%()`
**설명:** `%`와 `%()` 관계를 생각해 보라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    
string_1 = "Camelot"
string_2 = "place"

print "Let's not go to %s. 'Tis a silly %s." % (string_1, string_2)

```python
```

**설명:** 1번째 `%s`에는 변수 `string_1`값이 , 2번째 `%s`에는 변수 `string_2`의 값이 출력된다.  
{: .notice--info}


**결과**
```
Let's not go to Camelot. 'Tis a silly place.
```
<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
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

**설명:** `%s` 옵션에 직접 문자열도 치환 할 수 있다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**** Now it's your turn! We have ___ in the code to show you what you need to change!
**①** Inside the string, replace the three ___ with %s.
**②** After the string but before the three variables, replace the final ___ with a %.
**③** Hit Run.
**④** Answer the questions in the console as they pop up! Type in your answer and hit Enter.



**설명:** ① ___ 에 `%s`를 넣고, ② 치환할 변수에는 `%`를 넣는다. ③ `Run`한다.  ④ 콘솔에 질문이 나오면, 입력하고, `Enter`를 친다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Remember, the syntax is:
```python
print "%s" % (string_variable)
```
The `\` character on line 5 is a continuation marker. It simply tells Python that line 5 continues onto line 6.

**설명:**  앞전에서 배운 `%s` 를 사용한다. 그리고 `\`는 Python에게 문자열이 계속 된다는 것을 알려주는 것이다. 
{: .notice--info}

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

**설명:** `%s`, `%`로 치환한다. 그리고 **Console** 창에서 질문에 답을 입력하고 **Enter**를 입력한다. 
{: .notice--info}


**결과**
```
What is your name? iampeter
What is your quest? earth
What is your favorite color? yellow
Ah, so your name is iampeter, your quest is earth, and your favorite color is yellow.

```
<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
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

**설명:** 2장에서 배운 내용들이다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

Let's wrap it all up!

**①** On line 3, create the variable `my_string` and set it to **any string** you'd like.
**②** On line 4, use `len()` to print the length of `my_string`.
**③** On line 5, print the `.upper()` case version of `my_string`.


**설명:** ① 변수 `my_string`를 만들고 당신이 원하는 문자를 대입하라. ② 라이 4에서 `len()`함수를 사용하여 `my_string` 변수에 들어있는 길이를 출력하고 ③ 라인 5에서는 `.upper()`함수를 사용하여 `my_string`에 대입되어 있는 문자열을 모두 대문자로 변환하여 출력하여라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

You can `print` a variable with a method all on one line, like so: 
``` python
print my_variable.upper()
```
**설명:** `print`함수를 사용하고, `.upper()`를 사용하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    
```python
# Write your code below, starting on line 3!

my_string = "hey"
print len(my_string)
print my_string.upper()
```

**설명:** `len()`과 `.upper()`를 사용한다. 
{: .notice--info}


**결과**
```
3
HEY
```
<br>
<br>    
<br>   