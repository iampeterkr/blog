---
layout: posts
title:  "[conditionals-control-flow] 파이썬 조건절에 대한 설명!!"    
---

[#Python #Codecademy(코드카데미) #한글설명 가이드 #프로젝트 (03-#1)]
    
    
<hr style="border: solid 1px #dddddd ;">    

LESSON    

In this lesson, we'll learn how to create programs that generate different outcomes based on user input!    


**설명:** [ 학습방향 ]     
이 장에서는 사용자의 의도에 따라 다른 결과 값을 생성하는 프로그램을 만드는 연습을 한다. 
{: .notice--info}     
     
    
  
<hr style="border: solid 1px #dddddd ;">


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 
### 1. Go With the Flow    

Just like in real life, sometimes we'd like our code to be able to make decisions.

The Python programs we've written so far have had one-track minds: they can add two numbers or print something, but they don't have the ability to pick one of these outcomes over the other.

**Control flow** gives us this ability to choose among outcomes based on what else is happening in the program.


**설명:** [ Learn ]     
• Ch1. Go With the Flow 에서는 상황에 따른 선택을 할수 있는 방법을 학습한다.    
• Control flow 기능을 사용하여 다중 선택 방법을 학습한다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the code in the editor.     
* You'll see the type of program you'll be able to write once you've mastered control flow.     
* Click `Run` to see what happens!


**설명:** [ Instruction ]    
• Run 클릭 후, 프로그램이 어떻게 동작 되는지 확인하라. 
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
def clinic():
    print "You've just entered the clinic!"
    print "Do you take the door on the left or the right?"
    answer = raw_input("Type left or right and hit 'Enter'.").lower()
    if answer == "left" or answer == "l":
        print "This is the Verbal Abuse Room, you heap of parrot droppings!"
    elif answer == "right" or answer == "r":
        print "Of course this is the Argument Room, I've told you that already!"
    else:
        print "You didn't pick left or right! Try again."
        clinic()

clinic()
```

**설명:** [ Solution ]     
• Console 창에서, *right* 또는 *r*, *left* 또는 *l*, 또는 Enter 를 입력한다.    
• 입력값에 따라 결과물이 출력된다.
{: .notice--info}


**결과**
```
You've just entered the clinic!
Do you take the door on the left or the right?
Type left or right and hit 'Enter'.
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 2.  Compare Closely!    

Let's start with the simplest aspect of control flow: comparators. There are six:

Equal to (`==`)

```python
>>> 2 == 2
True
>>> 2 == 5
False
```


Not equal to (`!=`)

```python
>>> 2 != 5
True
>>> 2 != 2
False
```


Less than (`<`)

```python
>>> 2 < 5
True
>>> 5 < 2
False
```


Less than or equal to (`<=`)

```python
>>> 2 <= 2
True
>>> 5 <= 2
False
```


Greater than (`>`)

```python
>>> 5 > 2
True
>>> 2 > 5
False
```

Greater than or equal to (`>=`)

```python
>>> 5 >= 5
True
>>> 2 >= 5
False
```

Comparators check if a value is (or **is not**) **equal** to, **greater than** (or **equal** to), or **less than** (or **equal** to) another value.

Note that `==` compares whether two things are **equal**, and `=` assigns a value to a variable.



**설명:** [ Learn ]   
• Ch2.  Compare Closely! 에서는 비교 연산자를 학습한다.     
• `==` 같다, `!=` 같지 않다.    
• `>`  크다, `>=` 크거나 같다.    
• `<`  작다, `<=` 작거나 같다.    
• `==`와 `=`는 다른 표현이다.    
• `==`는 ex) A == B, A와 B가 같은지를 비교한다.     
• `=` 는 ex) A = 3, 변수 A 에 값 3을 대입한다.  
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Set each variable to `True` or `False` depending on what you think the result will be.    
* For example, `1 < 2` will be `True`, because **one** is **less than two**.

* Set `bool_one`   equal to the result of `17 < 328`
* Set `bool_two`   equal to the result of `100 == (2 * 50)`
* Set `bool_three` equal to the result of `19 <= 19`
* Set `bool_four`  equal to the result of `-22 >= -18`
* Set `bool_five`  equal to the result of `99 != (98 + 1)`



**설명:** [ Instruction ]    
• 아래 계산값의 결과를 True 또는 Fasle 로 각 변수에 대입하라.    
• 변수 bool_one   에  17 < 238         의 결과 값을 저장하라.   
• 변수 bool_two   에  100 == ( 2 * 50) 의 결과 값을 저장하라.   
• 변수 bool_three 에  19 <= 19         의 결과 값을 저장하라.   
• 변수 bool_four  에  -22 >= -18       의 결과 값을 저장하라.   
• 변수 bool_five  에  99 != (98 + 1)   의 결과 값을 저장하라.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, you set variables like this:    

```python
bool_one = True
```    

* Keep in mind that checking for equality uses a double equals sign:    

```python
True == True
```


**설명:** [ Hint ]    
• 변수 bool_one 에  True 또는 False 값을 대입하라. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
# Assign True or False as appropriate on the lines below!

# Set this to True if 17 < 328 or to False if it is not.
bool_one = True   # We did this one for you!

# Set this to True if 100 == (2 * 50) or to False otherwise.
bool_two = True

# Set this to True if 19 <= 19 or to False if it is not.
bool_three = True

# Set this to True if -22 >= -18 or to False if it is not.
bool_four = False

# Set this to True if 99 != (98 + 1) or to False otherwise.
bool_five = False
```

**설명:** [ Solution ]    
• 각 변수에 결과값이 맞으면 True, 틀리면 False를 대입한다. 
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
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 3. Compare... Closelier!    

Excellent! It looks like you're comfortable with **basic expressions** and **comparators**.

But what about extreme expressions and comparators?



**설명:** [ Learn ]    
• ( = ) 과 ( == ) 는 완전히 다르다.    
• ( = ) 는 대입할때 사용한다.    
• ( == )는 비교할때 사용한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Let's run through the comparators again with more complex expressions. Set each variable to `True` or `False` depending on what you think the result will be.

* Set `bool_one`   to the result of `(20 - 10) > 15`
* Set `bool_two`   to the result of `(10 + 17) == 3**16`
* Set `bool_three` to the result of `1**2 <= -1`
* Set `bool_four`  to the result of `40 * 4 >= -4`
* Set `bool_five`  to the result of `100 != 10**2`


**설명:** [ Instruction ]    
• 각 변수에 계산시 예상되는 결과값이 맞으면 : True , 틀리면 : False 를 대입하라. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* An Expression `(20-10) > 15` is `False`     

```python
bool_one = False
```

**설명:** [ Hint ]    
• 수식 (20-10) >  15 , 10 > 15라는 표현은 틀린 표현이다.    
• 즉, False 이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Assign True or False as appropriate on the lines below!

# (20 - 10) > 15
bool_one = False    # We did this one for you!

# (10 + 17) == 3 ** 16
# Remember that ** can be read as 'to the power of'. 3 ** 16 is about 43 million.
bool_two = False

# 1**2 <= -1
bool_three = False

# 40 * 4 >= -4
bool_four = True

# 100 != 10**2
bool_five = False
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]    
• 각 주석의 계산 값이 True  이면, 변수에 True  를 입력하라.    
• 각 주석의 계산 값이 False 이면, 변수에 False 를 입력하라.  
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
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 4. How the Tables Have Turned    

Comparisons result in either `True` or `False`, which are **booleans** as we learned before in this exercise.    

```python
# Make me true!
bool_one = 3 < 5
```    

Let's switch it up: we'll give the boolean, and you'll write the expression, just like the example above.




**설명:** [ Learn ]     
• 이전에 우리는 boolean 에 대하여 잠시 공부한적이 있다.     
• Python은 수식을 변수에 대입 하면(e.g. bool_one = 3 < 5)    
• 그 결과 값이 참(True)이면 참(True) 값이 대입된다.    
• 그 결과 값이 거짓(False)이면 거짓(True) 값이 대입된다.   
• 변수 bool_one 에 어떤 값이 대입될지 생각해 보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* For each boolean value in the editor, write an expression that evaluates to that value.     
* Remember, comparators are: `==`, `!=`, `>`, `>=`, `<`, and `<=`.

* Use at least three different ones!

* Don't just use `True` and `False`! That's cheating!

 


**설명:** [ Instruction ]    
• 각 주석문에서 지시하는 사항을 보고, 그 지시 사항에 맞게끔 대입하라.    
• 비교 연산자를 서로 겹치지 않게 3종류 이상 사용하라.    
• 직접 True, False 를 대입하지 마라.     
• e.g. ( bool_one = 3 < 5 ) 같이 참(True)이 되게 만든다.         
• 각 비교수식을 사용하여 작성하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* `bool_two` should store a false expression, so you could try:

```python
bool_two = 8 < 7
```

**설명:** [ Hint ]    
• 변수 bool_two 에 Fasle 값이 들어가게 오른쪽 비교문( 8 < 7 )을 만들어라.
{: .notice--info}


<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
# Create comparative statements as appropriate on the lines below!

# Make me true!
bool_one = 3 < 5  # We already did this one for you!

# Make me false!
bool_two = 99 == "lettuce"

# Make me true!
bool_three = 44 / 2 <= 43

# Make me false!
bool_four = "potato" != "potato"

# Make me true!
bool_five = "tomato" == "tomato"
```

**설명:** [ Solution ]    
• 주석에서 지시하는 조건을 만족하도록, 참(True), 거짓(False)값이 되도록 만든다.    
• 대입값은 비교 수식을 작성하여 대입하였다.
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
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 5. To Be and/or Not to Be    

**Boolean** operators compare statements and result in boolean values. There are three boolean operators:

1 **and**, which checks if both the statements are True;
2 **or**, which checks if at least one of the statements is True;
3 **not**, which gives the opposite of the statement.
We'll go through the operators one by one.


**설명:** [ Learn ]     
• Ch5. To Be and/or Not to Be 에서는 Boolean을 학습한다.     
• Boolean 에는 and , or , not 이 있다.     
• 아래의 boolean 표를 참조하자. 
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/03-boolean-00.svg)    

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)  

* Check out the truth tables to the right.     
* They show the results of using `AND`, `OR`, and `NOT` boolean operators given the boolean inputs `A` and `B`.    

* Click next to continue. 

**설명:** [ Instruction ]    
• Boolean 표를 보고, boolean이 어떻게 동작 되는지를 이해하자. 
{: .notice--info}



<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ Hint ]    
• skip
{: .notice--info}


<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
skip
```

**설명:** [ Solution ]    
• skip
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
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 6. AND     

The boolean operator and returns `True` when the expressions on both sides of `and` are `true`. For instance:     

* 1 < 2 and 2 < 3 is True;    
* 1 < 2 and 2 > 3 is False.     


**설명:** [ Learn ]     
• Ch6. AND 에서는 AND 연산자를 학습한다.    
• AND 연산자는 양 쪽 A, B의 값이 모두 참(True)이면, 참(True)이다.    
• A 또는 B 둘 중 하나라도 거짓(False)이면 거짓(False)이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png) 

* Let's practice with `and`.     
* Assign each variable to the appropriate `boolean` value.


* Set `bool_one` equal to the result of    

``` python
`False` and `False` 
```    

* Set `bool_two` equal to the result of    

```python
 `-(-(-(-2))) == -2` and `4 >= 16 ** 0.5`
```    

* Set `bool_three` equal to the result of     

```python
`19 % 4 != 300 / 10 / 10` and `False`
```   
<p style="page-break-before: always;"></p>
<br>


* Set `bool_four` equal to the result of    

```python
`-(1 ** 2) < 2 ** 0` and `10 % 10 <= 20 - 10 * 2`
```    

* Set `bool_five` equal to the result of     

```python
`True` and `True`
```    

   

**설명:** [ Instruction ]    
• AND 연산자 양변 A, B를 계산하여라.    
• 각 변수에, 계산 결과값이 참이면, 참(True) or 거짓이면, 거짓(False)을 대입하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
bool_one = False and False
```


**설명:** [ Hint ]    
• False(거짓) and False(거짓) 은 False(거짓) 이다.     
• 변수 bool_one 에 결과값 거짓(False)을 대입한다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
bool_one = False and False

bool_two = -(-(-(-2))) == -2 and 4 >= 16 ** 0.5

bool_three = 19 % 4 != 300 / 10 / 10 and False

bool_four = -(1 ** 2) < 2 ** 0 and 10 % 10 <= 20 - 10 * 2

bool_five = True and True
```

**설명:** [ Solution ]    
• 오른쪽의 계산 결과 값이 참(True) or 거짓(False) 인지를 계산한다.    
• 그 결과가 각 변수에 저장된다.     
• And 연산자는 양 변이 모두 참(True)일 때만, 참(Ture)을 반환한다. 
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
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 7. OR    

The **boolean** operator or returns `True` when at least one expression on either side of or is true. For example:

```python
1 < 2 or 2 > 3 is True;
1 > 2 or 2 > 3 is False.
```


**설명:** [ Learn ]     
• Ch7. OR 에서는 OR 연산자를 학습한다.     
• OR 연산자는 양 변이 하나라도 참(True)이면, 참(True)을 반환한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Time to practice with or!

* Set `bool_one` equal to the result of    

```python
2 ** 3 == 108 % 100 or 'Cleese' == 'King Arthur'
```    
* Set `bool_two` equal to the result of    

```python
True or False
```    

* Set `bool_three` equal to the result of    

```python
100 ** 0.5 >= 50 or False
```    

* Set `bool_four` equal to the result of    

<p style="page-break-before: always;"></p>
<br>

```python
True or True
```    

* Set `bool_five` equal to the result of    

```python
1 ** 100 == 100 ** 1 or 3 * 2 * 1 != 3 + 2 + 1
```   


**설명:** [ Instruction ]     
• 각 변수에 OR 연산자를 한 결과 값( True 또는 False ) 을 대입하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, or is True when either (or both!) of the expressions involved are true.

**설명:** [ Hint ]    
• OR 의 경우 양변 A , B 중 하나라도 참(True)이면 참(True)이 된다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
bool_one = 2**3 == 108 % 100 or 'Cleese' == 'King Arthur'

bool_two = True or False

bool_three = 100**0.5 >= 50 or False

bool_four = True or True

bool_five = 1**100 == 100**1 or 3 * 2 * 1 != 3 + 2 + 1
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• OR 연산자 양 변의 A , B 값이 계산된다.    
• 계산된 값 참(True), 거짓(False)값이 자동으로 변수에 대입된다. 
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
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 8. Not    

The **boolean** operator `not` returns `True` for `false` statements and `False` for `true` statements.

For example:

not `False` will evaluate to `True`, while not `41 > 40` will return `False`.



**설명:** [ Learn ]     
• Ch8. Not 에서는 NOT 연산자를 학습한다.    
• Not 은 다음과 같이 동작한다.    
• True 는 False 를 반환한다.    
• False 는 True 를 반환한다.    
• 41 > 40 은 계산 결과는 True 이다.    
• 하지만, 앞에  NOT(!) 연산자가 있으므로, False 를 반환한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Let's get some practice with not.

* Set `bool_one` equal to the result of    

```python
not True
```    

* Set `bool_two` equal to the result of    

```python
not 3 ** 4 < 4 ** 3
```    

* Set `bool_three` equal to the result of    

```python
not 10 % 3 <= 10 % 2
```    

* Set `bool_four` equal to the result of    

```python
not 3 ** 2 + 4 ** 2 != 5 ** 2
```    

* Set `bool_five` equal to the result of    

```python
not not False
```    



**설명:** [ Instruction ]    
• 각 변수에 양변의 계산 결과 값을 True 또는 False 를 대입하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, not True is False and not False is True. So, for example, bool_one should be:   

```python
bool_one = False
```

**설명:** [ Hint ]    
• NOT ( ! ) 연산자는 양 변의 최종 결과값의 반대를 반환한다.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
bool_one = not True

bool_two = not 3**4 < 4**3

bool_three = not 10 % 3 <= 10 % 2

bool_four = not 3**2 + 4**2 != 5**2

bool_five = not not False
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]    
• 각 변수의 반환값이 무엇일지 생각해 보자. 
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
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 9. This and That (or This, But Not That!)

**Boolean** operators aren't just evaluated from **left** to **right**. Just like with **arithmetic operators**, there's an order of operations for boolean operators:

1. `not` is evaluated **first**;
2. `and` is evaluated **next**;
3. `or`  is evaluated **last**.
For example, `True` or not `False` and `False` returns `True`. If this isn't clear, look at the Hint.

Parentheses `()` ensure your expressions are evaluated in the order you want. Anything in parentheses is evaluated as its own unit.


**설명:** [ Learn ]    
• Ch9. This and That 에서는 Boolean 의 우선 순위를 학습한다.    
• boolean 의 계산 순서는 수학의 우선 순위와 같다.    
• 1st : NOT     
• 2nd : AND    
• 3rd : OR    
• () 는 NOT 보다 순서가 빠르다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Assign `True` or `False` as appropriate for `bool_one` through `bool_five`.

* Set `bool_one` equal to the result of    

```python
False or not True and True
```    

* Set `bool_two` equal to the result of   

```python
False and not True or True
```   

* Set `bool_three` equal to the result of    

```python
True and not (False or False)
```    

* Set `bool_four` equal to the result of    

```python
not not True or False and not True
```    

* Set `bool_five` equal to the result of    

```python
False or not (True and True)
```


**설명:** [ Instruction ]    
• 각 변수에 True 또는 False 를 대입하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* True or not False and False.     

1. `not` gets evaluated **first**, 
2. so we have `True or True and False`. 
3. `and` goes next, 
4. so we get `True or False`. 
5. As we've seen, `True or False` is `True`, 
6. so the value finally returned is `True`!


**설명:** [ Hint ]    
• NOT -> AND -> OR 순으로 계산한다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
bool_one = False or not True and True

bool_two = False and not True or True

bool_three = True and not (False or False)

bool_four = not not True or False and not True

bool_five = False or not (True and True)
```

**설명:** [ Solution ]    
• 각 변수에 NOT , AND , OR 순으로 계산한다.    
• 그 결과값 True 또는 False 가 대입된다.     
• 각 변수를 출력해 보면, 계산 결과값을 알수 있다.
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
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 10. Mix 'n' Match    

Great work! We're almost done with **boolean** operators.

```python
# Make me false
bool_one = (2 <= 2) and "Alpha" == "Bravo"
```

**설명:** [ Learn ]     
• Ch10. Mix 'n' Match 에서는 boolean을 학습한다.  
• 변수 bool_one 에는 False 값이 반환된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* This time we'll give the expected result, and you'll use some combination of **boolean** operators to achieve that result.

* Remember, the **boolean** operators are `and`, `or`, and `not`. Use each one at least once!


**설명:** [ Instruction ]     
• Editor 화면의 소스에서 주석을 읽고 이해하라.    
• 주석에서 지시하는대로 결과 값을 만들어라.    
• Boolean 은 연산자 ( NOT , AND , OR ) 를 활용하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Make sure to use at least one `and`, `or`, or `not`.

**설명:** [ Hint ]    
• Boolean 연산자 NOT , AND , OR 사용하여 만들라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Use boolean expressions as appropriate on the lines below!

# Make me false!
bool_one = (2 <= 2) and "Alpha" == "Bravo"  # We did this one for you!

# Make me true!
bool_two = True and True

# Make me false!
bool_three = False and True

# Make me true!
bool_four = not False

# Make me true!
bool_five = True or True
```

**설명:** [ Solution ]    
• 주석에서 True 를 만들려면, 우변의 값을 True로 만들어 대입한다.
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
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 11. Conditional Statement Syntax    

`if` is a **conditional statement** that executes some specified code after checking if its expression is `True`.

Here's an example of `if` statement syntax:    

```python
if 8 < 9:
  print "Eight is less than nine!"
```    

In this example, `8 < 9` is the checked expression and print **"Eight is less than nine!"** is the specified code.

Pay **attention** to the **indentation** before the `print` statement. This space, called white space, is how Python knows we are entering a **new block** of code. Python accepts many different kinds of **indentation to indicate blocks**. In this lesson, we use four **spaces** but elsewhere you might encounter **two-space** indentation or tabs (which Python will see as different from spaces).

If the **indentation** from one line to the next is different and there is no command (like if) that indicates an incoming block then Python will raise an `IndentationError`. These errors could mean, for example, that one line had two spaces but the next one had three. Python tries to indicate where this error happened by printing the line of code it couldn't parse and using a `^` to point to where the indentation was different from what it expected.




**설명:** [ Learn ]    
• Ch11. Conditional Statement Syntax 에서는 조건문을 학습한다.      
• if 문은 조건문 이다.     
• 조건이 True 이면, if 절 내부에 정의된 내용을 실행한다.    
• if 문 사용시 주의 사항은 다음과 같다.    
• if 문 조건 뒤에 항상 ( : )을 붙여줘야 한다.      
• 이것은 if 문 조건이 끝났음을 의미한다.    
• if 문 내부를 정의할때, if 문 보다 안쪽으로 Space 2칸이 들어간 상태에서 시작한다.    
• if 문은 자신보다 안쪽에 위치한 내용을 자신의 처리 범위로 여긴다.    
• 들여쓰기가 정상적이지 않으면 Python 해석기는 Error 를 발생시킨다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* If you think the `print` statement will print to the console, set `response` equal to 'Y'; otherwise, set response equal to 'N'.


**설명:** [ Instruction ]    
• 출력되는 문장의 내용이 맞으면 변수 response 에 'Y' 를 대입한다.    
• 그렇지 않으면 변수 response 에 'N'를 대입한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Make sure to set response to "Y" or "N"!


**설명:** [ Hint ]    
• 변수 response 에 'Y' 또는 'N' 를 대입한다.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
response = 'N'

answer = "Left"
if answer == "Left":
    print "This is the Verbal Abuse Room, you heap of parrot droppings!"
    
# Will the above print statement print to the console?
# Set response to 'Y' if you think so, and 'N' if you think not.
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]    
• 출력문의 내용이 마음에 들지 않으므로 변수 response 에 'N' 를 대입한다. 
{: .notice--info}



**결과** 
``` 
This is the Verbal Abuse Room, you heap of parrot droppings!
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 12. If You're Having...    

Let's get some practice with `if` statements. Remember, the syntax looks like this:

```python
if some_function():
  # block line one
  # block line two
  # et cetera
```    

Looking at the example above, in the event that `some_function()` returns `True,` then the indented block of code after it will be executed. In the event that it returns False, then the indented block will be skipped.

Also, make sure you notice the `colons` at the end of the `if` statement. We've added them for you, but they're important.


**설명:** [ Learn ]     
• Ch12. If You're Having... 에서는 조건에 따라 결과값을 결정하는 학습을 한다.    
• if 문 은 some_function()을 호출하여 받은 결과값이 True 인지를 비교한다.    
• if 문의 결과값이 True 이면, if 문 블럭안에 다음 정의문이 실행된다.     
• e.g.  # block line one,    
• e.g.  # block line two,     
• e.g.  # et cetera     
• 결과값이 False 이면 정의문 들은 실행되지 않는다.    
• if 문의 끝에는 ( : ) 이 항상 있어야 한다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* In the editor you'll see two functions.    
* Don't worry about anything unfamiliar.     
* We'll explain soon enough.    
* Replace the underline on line 2 with an expression that returns `True`.    
* Replace the underline on line 6 with an expression that returns `True`.    
* If you do it successfully, then both "Success #1" and "Success #2" are printed.


**설명:** [ Instruction ]     
• 2 라인과 6 라인에 각 True 가 되도록 계산식을 수정하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Here's an example to remind you of the syntax:

```python
def true_function():
  if 1 < 2:
    return True
```    

* Don't forget the colon at the end of the line!


**설명:** [ Hint ]    
• if 문 다음의 조건절에 True 값이 되도록 계산식을 만든다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def using_control_once():
    if 2 < 3:
        return "Success #1"

def using_control_again():
    if 3 == 3:
        return "Success #2"

print using_control_once()
print using_control_again()
```

**설명:** [ Solution ]     
• if 2 <  3:  이 True 가 되도록 조건문을 만들었다.    
• if 3 == 3:  이 True 가 되도록 조건문을 만들었다.
{: .notice--info}



**결과** 
```
Success #1
Success #2
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 13. Else Problems, I Feel Bad for You, Son...    

The `else` statement complements the if statement. An `if/else` pair says: "If this expression is true, run this indented code block; otherwise, run this code after the else statement."

Unlike if, else doesn't depend on an expression. For example:

```python
if 8 > 9:
  print "I don't printed!"
else:
  print "I get printed!"
```

**설명:** [ Learn ]     
• Ch13. Else Problems, ... 에서는 else 문을 학습한다.    
• else 문은 if 문과 함께 사용한다.     
• if 문 조건을 체크하고, 조건에 맞지 않으면, else 문이 실행된다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Complete the `else` statements to the right. Note the indentation for each line!


**설명:** [ Instruction ]     
• Coding 창에 있는 소스중, else 문을 완성하라. (단, 들여 쓰기를 주의하라.)
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* To complete your `else` statement lines, the only thing you need to do is add `False` after the returns on lines 7 and 13.

**설명:** [ Hint ]    
• else 문 부분을 False 로 수정하라.
{: .notice--info}

<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
answer = "'Tis but aa scratch!"

def black_knight():
    if answer == "'Tis but a scratch!":
        return True
    else:
      	print ("else call")
        return False        # Make sure this returns False

black_knight()


def french_soldier():
    if answer == "Go away, or I shall taunt you a second time!":
        return True
    else:             
        return False        # Make sure this returns False
      
```

**설명:** [ Solution ]    
• 함수 black_knight() 에서는 다음과 같이 동작한다.    
• if 문이 변수 answer 과 문자열을 비교한다.    
• 비교한 결과가 참이면 True 를 반환한다.    
• 비교한 결과가 거짓이면 else 문이 작동된다.    
• e.g. print ("else call")     
• else 문의 블럭내용이 출력된다.    
• 그리고 False 가 반환(return)된다.    
• # 각 line 에 print 문을 작성해 보면, 그 결과를 알 수 있다.
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
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 14. I Got 99 Problems, But a Switch Ain't One    

`elif` is short for **"else if."** It means exactly what it sounds like: "otherwise, if the following expression is true, do this!"

```python
if 8 > 9:
  print "I don't get printed!"
elif 8 < 9:
  print "I get printed!"
else:
  print "I also don't get printed!"
```    

In the example above, the `elif` statement is only checked if the original if statement is `False`.


**설명:** [ Learn ]    
• Ch14. I Got 99 Problems, 에서는 elif 를 학습한다.     
• elif 는 *else if* 의 줄인 말이다.    
• elif 는 if 조건절이 아니고 그다음에 다른 조건을 체크 하고 싶을때 사용한다.    
• 비슷한 else 와의 차이는 else 는 조건을 만들수 없지만, elif 문은 조건문을 만들수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On line 2, fill in the `if` statement to check if answer is greater than `5`.

* On line 4, fill in the `elif` so that the function outputs `-1` if answer is less than `5`.


**설명:** [ Instruction ]    
• 2 라인에서 if 문을 사용한다.    
• 조건은 변수 answer 값이 5 보다 크면 1 을 반환한다.    
• 4 라인에서 elif 문을 사용한다.    
• 조건은 변수 answer 값이 5 보다 작으면 -1 을 반환하라.  
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Make sure the `if` and `elif` statements end with colons :

* Your code should look something like:

```python
if EXPRESSION:
  # do something
elif OTHER EXPRESSION:
  # do something
else:
  # do something
```

**설명:** [ Hint ]    
• if , elif , else 문의 끝에 ( : ) 를 꼭 넣어야 한다.    
• 마지막에 각 함수를 출력해보면, 결과 값을 알수 있다.
{: .notice--info}    


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
def greater_less_equal_5(answer):
    if answer > 5:
        return 1
    elif answer < 5:          
        return -1
    else:
        return 0
        
print greater_less_equal_5(4)
print greater_less_equal_5(5)
print greater_less_equal_5(6)

```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 변수 answer 가 5 보다 큰지 or 작은지 or 같은지를 비교하여 그 결과값을 반환한다. 
{: .notice--info}


**결과** 
``` 
-1
0
1
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CONDITIONALS & CONTROL FLOW</font> 

### 15. The Big If    

Really great work! Here's what you've learned in this unit:

**Comparators**    
```python
3 < 4
5 >= 5
10 == 10
12 != 13
```

**Boolean operators**    
```python
True or False 
(3 < 4) and (5 >= 5)
this() and not that()
```

**Conditional statements**    
```python
if this_might_be_true():
  print "This really is true."
elif that_might_be_true():
  print "That is true."
else:
  print "None of the above."
Let's get to the grand finale.
```



**설명:** [ Learn ]     
• Ch15. The Big If 에서는 지금까지 배운 모든 연산자를 학습한다.    
• 지금까지 배운 비교문, Boolean 연산자, 조건문( if , elif , else )를 복습하자.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* In the workspace to your right, there is the outline of a function called `grade_converter()`.

* The purpose of this function is to take a number grade **(1-100)**, defined by the variable `grade`, and to return the appropriate letter **grade (A, B, C, D, or F)**.

* Your task is to complete the function by creating appropriate `if` and `elif` statements that will compare the input `grade` with a number and then return a letter `grade`.

* Your function should return the following letter grades:

  * 90 or higher should get an "A"
  * 80 - 89 should get a "B"
  * 70 - 79 should get a "C"
  * 65 - 69 should get a "D"
  * Anything below a 65 should receive an "F"


**설명:** [ Instruction ]    
• 함수 grade_converter() 를 만든다.    
• 함수의 동작은 비교문, 조건문을 사용하라.    
• 함수 조건은 점수 구간에 따라 A, B, C, D, F 등급을 준다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Be careful with your indentation—grade_converter() is a function (which we'll get to in the next unit), and as you can see from the comment, function blocks are indented the same way if, elif, and else blocks are.

* If you are having trouble creating the if and elif statements, here's the first one you can use as an example:    

```python
if grade >= 90:
     return "A"
```     

This will compare the variable grade with the value 90 and if it is greater than or equal to 90 it will return the letter A.

**설명:** [ Hint ]    
• 조건문 ( if grade >= 90: ) 은 변수 grade 값이 90 보다 크거나 같다는 표현이다.   
• 이 조건이 맞으면 if 문 내부에 A 가 반환되도록 작성한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
# Complete the if and elif statements!
def grade_converter(grade):
    if grade >= 90:
        return "A"
    elif grade >= 80:
        return "B"
    elif grade >= 70:
        return "C"
    elif grade >= 65:
        return "D"
    else:
        return "F"
      
# This should print an "A"      
print grade_converter(92)

# This should print a "C"
print grade_converter(70)

# This should print an "F"
print grade_converter(61)
```

**설명:** [ Solution ]    
• if , elif , else 를 사용하여 점수 구간별 A, B, C, D, F 등급을 반환한다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**결과** 
``` 
A
C
F
```