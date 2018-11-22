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

You can use the lower() method to get rid of all the capitalization in your strings. You call lower() like so:

"Ryan".lower()
which will return "ryan".



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


**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 7. 



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

<

**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 8. 



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

<

**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 9. 



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

<

**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 10. 



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

<

**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 11. 



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

<

**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

### 12. 



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



**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

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

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}



**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

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

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

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


**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

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


**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

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


**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

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


**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    

<font size="3"  face="돋움">STRING & CONSOLE OUTPUT</font> 

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


**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
