---
# layout : rchive
title: "Advanced Topics in Python"
permalink: /advanced-topics-python/
excerpt: "We learn about Data structure, list comprehension, slicing, lambda Syntax."
# last_modified_at: 2019-02-25T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---

        

<hr style="border: solid 1px #dddddd ;">    

LESSON    

In this lesson, we'll cover some of the more complex aspects of Python, including iterating over data structures, list comprehensions, list slicing, and lambda expressions.      

**설명:** [ 학습방향 ]     
이 장에서는 Python 을 활용한 다양한 자료구조를 학습한다.     
Data structure, list comprehension, list slicing, lambda 를 배워보자.
{: .notice--info}  
    
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 1. Iterators for Dictionaries    

Let's start with iterating over a dictionary. Recall that a dictionary is just a collection of keys and values.
```python
d = {
  "Name": "Guido",
  "Age": 56,
  "BDFL": True
}
print d.items()
# => [('BDFL', True), ('Age', 56), ('Name', 'Guido')]
```
Note that the .items() method doesn't return key/value pairs in any specific order.

 



**설명:** [ Learn ]     
• Ch1. Iterators for Dictionaries 에서는 딕셔너리를 집중 학습한다.     
• 딕셔너리의 반복문에 대해서 연습해 보자.    
• 앞에서 배운 딕셔너리의 key 와 value를 조작하는 법을 연습해 본다.    
• d.items() 는 딕셔너리 d 의 key 와 value 를 리스트 형태로 보여준다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create your own Python dictionary, `my_dict`, in the editor to the right with **two or three key/value** pairs.    
* Then, print the result of calling the `my_dict.items()`.


**설명:** [ Instruction ]    
• 딕셔너리 my_dict 작성하라.    
• 이 딕셔너리는 2 or 3 개의 key/value 쌍을 가진다.        
• 메서드 my_dict.item() 를 실행후, 그 결과를 출력하라.     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can think of dictionaries as unordered key/value pairs.


**설명:** [ Hint ]    
• 딕셔너리는 key/value 가 출력될때, 입력한 순으로 정렬되지 않는다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
my_dict = {
  'name': 'Nick',
  'age':  31,
  'occupation': 'Dentist',
}

print my_dict.items()

```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 딕셔너리 my_dict 에 다음과 같은 정보가 key/value 쌍으로 저장되어 있다.    
• 'name' : 'Nick',     
• 'age' : 31,     
• 'occupation' : 'Dentist'    
• 메서드 my_dict.items() 를 호출후 출력한다.
{: .notice--info}


**결과**     
```
[('age', 31), ('name', 'Nick'), ('occupation', 'Dentist')]
```      
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 2. keys() and values()    

While `.items()` returns an array of **tuples** with each tuple consisting of a key/value pair from the dictionary:

The `.keys()` method returns a list of the dictionary's keys, and
The `.values()` method returns a list of the dictionary's values.
Again, these methods will not return the keys or values from the dictionary in any specific order.
You can think of a tuple as an immutable (that is, unchangeable) list. Tuples are surrounded by ()s and can contain any data type.    


**설명:** [ Learn ]     
• Ch2. keys() and values() 에서는 딕셔너리의 메서드 및 튜플을 학습한다.    
• 메서드 .items() 는 key/value 로 구성된 각각의 튜플 형태의 배열로 반환한다.    
• 메서드 .keys() 는 key 값을 리스트 형태로 반환한다.        
• 메서드 .values() 는 value 값을 리스트 형태로 반환한다.    
• key 와 value 쌍값은 순서 없이 반환된다.    
• 주의) 튜플은 리스트와 동일하지만, 틀린점은 ()로 둘러쌓인 그 항목 값을 변경할수 없다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Remove your call to `.items()` and replace it with a call to `.keys()` and a call to `.values()`, each on its own line. Make sure to print both!


**설명:** [ Instruction ]    
• 메서드 .item() 를 지우고, 대신에 .keys() 와 .values() 로 대체하라.    
• 그리고 각각을 출력하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* For instance, your call to `my_dict.keys()` might look like:    

```python
print my_dict.keys()
```

**설명:** [ Hint ]   
• 메서드 my_dict.keys() 는 key 만 출력한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
my_dict = {
  'name': 'Nick',
  'age':  31,
  'occupation': 'Dentist',
}

print my_dict.keys()
print my_dict.values()
```

**설명:** [ Solution ]     
• 메서드 my_dict.keys() 는 딕셔너리 my_dict 의 key 값만 리스트 형태로 출력한다.    
• 메서드 my_dict.values() 는 딕셔너리 my_dict 의 value 값만 리스트 형태로 출력한다.
{: .notice--info}


**결과**     
``` 
['age', 'name', 'occupation']
[31, 'Nick', 'Dentist']
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 3. The 'in' Operator    

For iterating over lists, tuples, dictionaries, and strings, Python also includes a special keyword: `in`. You can use `in` very intuitively, like so:

```python
for number in range(5):
  print number,

d = { 
  "name": "Eric",
  "age": 26
}

for key in d:
  print key, d[key],

for letter in "Eric":
  print letter,  # note the comma!
```
* In the example above, first we create and iterate through a range, printing out 0 1 2 3 4. Note that the trailing comma ensures that we keep printing on the same line.    
* Next, we create a dictionary and iterate through, printing out age 26 name Eric. Dictionaries have no specific order.
Finally, we iterate through the letters of a string, printing out E r i c.
  



**설명:** [ Learn ]     
• Ch3. The `in` Operator 에서는 for 문의 `in` 문법을 학습한다.    
• `in` 연산자는 다음을 반복적으로 추출할때 직관적으로 사용한다.    
• - 리스트(list),    
• - 튜플(tuple),    
• - 딕셔너리(dictionarie),    
• - 문자열(string)    
• 함수 range(5) 는 숫자 0, 1, 2, 3, 4 를 생성해 준다.    
• 이를 한줄로 출력 할려면, ( , ) 를 사용한다.     
• 문자열 *Erir* 를 한줄출력 ( , ) 를 사용하여, "E r i c" 로 출력한다.    
• 딕셔너리는 순서가 보장 안되는 것을 잊지 말라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* For each key in `my_dict`: print out the key , then a space, then the value stored by that key. (You should use print a, b rather than print a + " " + b.)


**설명:** [ Instruction ]    
• 딕셔너리 my_dict 의 key 와 value 를 출력하라.    
• 단, key 와 value 사이에 공백 하나가 있어야 한다.     
• 출력시 print a + " " + b 보다는 print a, b 를 사용하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You'll want to do something like this:    

```python
for key in some_dict:
  print key, some_dict[key]
```

**설명:** [ Hint ]    
• 출력시 key 와 some_dict[key] 사이에 공백이 있어야 한다.    
• 공백은 ( " " ) 아닌, ( , ) 를 사용하라.    
• e.g.  print key, some_dict[key]
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
my_dict = {
  'name': 'Nick',
  'age':  31,
  'occupation': 'Dentist',
}
```
<p style="page-break-before: always;"></p>
<br>

```python
for key in my_dict:
  print key, my_dict[key]
```

**설명:** [ Solution ]     
• 딕셔너리 my_dict 에서 key 값을 읽는다.    
• key 값과 value값(my_dict[key]) 을 출력한다. 
{: .notice--info}



**결과** 
```
age 31
name Nick
occupation Dentist
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 4. Building Lists    

Let's say you wanted to build a list of the numbers from 0 to 50 (inclusive). We could do this pretty easily:
```python
my_list = range(51)
```
But what if we wanted to generate a list according to some logic—for example, a list of all the even numbers from 0 to 50?

Python's answer to this is the list comprehension. List comprehensions are a powerful way to generate lists using the for/in and if keywords we've learned.


**설명:** [ Learn ]     
• Ch4. Building Lists 에서는 리스트 컴프레션을 학습한다.    
• 0 ~ 50 까지의 정수를 리스트에 저장하는 법은 다음과 같다.    
• e.g. my_list = range(51)     
• 만약, 0부터 50사이의 짝수만 저장하고 싶다면?     
• Python 에서는 우리가 익히 잘 사용하는 for / if 문을 사용하여,       
• 리스트 컴프레션(list comprehension)을 기능을 사용하면 쉽게 만들수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the list comprehension example in the editor. When you're pretty sure you know what it'll do, click Run to see it in action.


**설명:** [ Instruction ]    
• Editor 화면에 있는 소스를 이해하고 실행하라. 
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
evens_to_50 = [i for i in range(51) if i % 2 == 0]
print evens_to_50
```    

**설명:** [ Solution ]     
• 리스트 컴프레션(list comprehension) 을 사용하여 리스트를 만들었다.    
• 리스트 컴프레션은 다음과 같이 동작한다.    
• 리스트 안에 for 문과 if문을 두어 조건에 해당하는 값을 산출한다.    
• for 문에서 함수 range(51)을 사용하여 0 ~ 50까지 값을 산출후 변수 i 에 저장한다.    
• 만약, 저장된 i 값을 % 2 로 계산하여 나머지가 0 이면, 제일 앞 변수 i 저장한다.    
• 저장된 i 의 값은 리스트 형태로 변수 event_to_50 에 저장한다.
{: .notice--info}    



**결과**     
``` 
[0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50]
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 5. List Comprehension Syntax    

Here's a simple example of list comprehension syntax:    
```python
new_list = [x for x in range(1, 6)]
# => [1, 2, 3, 4, 5]
```    
This will create a new_list populated by the numbers one to five. If you want those numbers doubled, you could use:    
```python
doubles = [x * 2 for x in range(1, 6)]
# => [2, 4, 6, 8, 10]
```    
And if you only wanted the doubled numbers that are evenly divisible by three:    
```python
doubles_by_3 = [x * 2 for x in range(1, 6) if (x * 2) % 3 == 0]
# => [6]
```



**설명:** [ Learn ]      
• Ch5. List Comprehension Syntax 에서는 리스트 컴프레션 문법을 학습한다.    
• 다음 예제는 list comprehension 에 관한것이다.    
• 예제 1) new_list = [ x for x in range(1, 6)]    
• 예제 1 은 맨 앞 x 에 for 문 결과값이 저장된다.    
• 예제 2) doubles = [x * 2 for x in range(1, 6)]    
• 예제 2 는 맨 앞 x 에 for 문 결과값이 저장되고, 다시 x 값에 곱하기 2 한 값이 저장된다.    
• 예제 3) doubles_by_3 = [x * 2 for x in range(1, 6) if (x * 2) % 3 == 0]    
• 예제 3은 for 문과 if 문이 실행되어 만족한 x 값 3이 맨앞 x 변수에 저장된다.    
• 그리고 그 값에 x 에 곱하기 2 한 값이 리스트에 저장된다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

* Use a list comprehension to build a list called `even_squares` in the editor.

* Your `even_squares` list should include the squares of the even numbers between 1 to 11. Your list should start [4, 16, 36...] and go from there.


**설명:** [ Instruction ]    
• 리스트 even_squares 를 작성하라.         
• 리스트 even_squares 는 1 부터 11 사이의 숫자중 짝수의 제곱을 저장하는 리스트이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can use `x ** 2` to square a number, and `x % 2 == 0` to check if it's even.      

```python
# from 1 to 10
range(1,11) 
# from 1 to 11
range(1,12)
```

**설명:** [ Hint ]    
• 제곱은 ( x ** 2 ) 로 구하고, 짝수는 ( x % 2 == 0 ) 로 구한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
doubles_by_3 = [x * 2 for x in range(1, 6) if (x * 2) % 3 == 0]

# Complete the following line. Use the line above for help.
even_squares = [x ** 2 for x in range(1, 12) if x % 2 == 0]

print even_squares
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 리스트 even_squares 를 리스트 컴프레션을 사용하여 다음과 같이 만들어진다.    
• for 문에서  1(포함) 부터 12(미포함) 까지 산출하고, 변수 x 에 저장한다.    
• if 문에서 변수 x 를 % 2 로 나누어서 나머지가 0 인지 확인한다.    
• 맨 앞 변수 x 에 나머지가 0 ( 즉, 짝수 ) 인 값을 저장한다.    
• 변수 x 값을 제곱( e.g. x ** 2 )한다.    
• 리스트 even_squares 에 저장한다.     
• 리스트 even_squares 를 출력한다. 
{: .notice--info}



**결과**     
``` 
[4, 16, 36, 64, 100]
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 6. Now You Try!    

Great work! Now it's time for you to create a list comprehension all on your own.    
```python
c = ['C' for x in range(5) if x < 3]
print c
```    
The example above creates and prints out a list containing ['C', 'C', 'C'].

 

**설명:** [ Learn ]     
• Ch6. Now You Try! 에서는 리스트 컴프레션을 집중 학습한다.    
• for 문에서 5개의 x 값을 구한다.    
• 구한 x 값이 3보다 작은 경우는 0, 1, 2이다. 횟수가 3 회이다.     
• 즉, 3 번의 'C' 문자가 리스트에 저장되고, 이 리스트 c 를 출력한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Use a list comprehension to create a list, `cubes_by_four`.

* The comprehension should consist of the cubes of the numbers 1 through 10 only if the cube is evenly divisible by four.

* Finally, print that list to the console.

* Note that in this case, the cubed number should be evenly divisible by 4, not the original number.




**설명:** [ Instruction ]    
• 리스트 cubes_by_four 를 리스트 컴프레션을 사용하여 작성하라.    
• 1 부터 10까지의 숫자를 세제곱(cube) 한다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

• 이 값을 4로 나누어 떨어지는 값만 리스트에 저장하라.     
• 위 결과가 담긴, 리스트 cubes_by_four 를 출력하라.    
• 리스트 cubes_by_four 는 4로 나누어 떨어지는 값들이다.    
• 원래 x 값이 아니라, 세제곱한 ( x ** 3 )한 값을 리스트에 저장하는 것이다.     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
#from 1 to 10
range(1,11)
```


**설명:** [ Hint ]    
• 1부터 10 까지를 출력하려면, 함수 range(1 , 11) 을 해야한다.    
• x ** 3 한 값이 ( x % 4 == 0 )인 값을 저장한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
cubes_by_four = [x ** 3 for x in range(1, 11) if ((x ** 3) % 4) == 0]
print cubes_by_four
```

**설명:** [ Solution ]     
• 리스트 컴프레션을 사용하여 리스트 cubes_by_four를 작성한다.    
• for 문에서, 1 부터 10 까지 숫자를 산출하여, 변수 x 에 저장한다.    
• if 문에서, x 값을 세제곱한다. 그리고 4 로 나누어 떨어지는지를 비교한다.    
• if 문에서 True 인 x 값을, 맨앞 변수 x 에 저장한다.    
• 맨앞 변수 x 를 세제곱한다.    
• 세제곱한 변수 x 를 리스트 cubes_by_four 에 저장한다.    
• e.g. 숫자 8 은 (8 % 4 == 0)를 충족하고, x=2일때, (2 ** 3) 도 충족한다.      
• e.g. 숫자 16 은 (16 % 4 == 0)은 충족하지만 (x ** 3 = 16)은 충족하지 않는다.    
• e.g. 숫자 64 는 (64 % 4 == 0)을 충족하고, x=4일때, (4 ** 3)도 충족한다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>


**결과**     
``` 
[8, 64, 216, 512, 1000]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>    

### 7. List Slicing Syntax    

Sometimes we only want part of a Python list. Maybe we only want the first few elements; maybe we only want the last few. Maybe we want every other element!

List slicing allows us to access elements of a list in a concise manner. The syntax looks like this:    
```python
[start:end:stride]
```    

Where start describes where the slice starts (inclusive), end is where it ends (exclusive), and stride describes the space between items in the sliced list. For example, a stride of 2 would select every other item from the original list to place in the sliced list.



**설명:** [ Learn ]    
• Ch7. List Slicing Syntax  에서는 리스트 슬라이싱을 학습한다.    
• 우리는 list 의 일부분을 발췌하고 싶을때가 있다.    
• 이런경우 List slicing 을 사용한다.    
• List slicing 은 리스트를 간편하게 접근하게 해준다.    
• 문법은 다음과 같다.     
• e.g. [시작:끝:간격]     
• - 시작(start) : Slicing을 시작할 위치(포함)     
• - 끝(end) : Slicing 끝낼 위치(포함하지 않음)    
• - 간격(stride) : 시작을 포함하여 몇번째를 가져올지(옵션)    
• 시작은 해당값을 포함한다.    
• 끝은 포함하지 않는다.     
• 간격은 옵션이다. 시작을 포함하여 몇 번씩 가져올지를 나타낸다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* We've generated a list with a list comprehension in the editor to the right, and we're about to print a selection from the list using list slicing.     

<p style="page-break-before: always;"></p>
<br>

* Can you guess what will be printed out? Click Run when you think you know!


**설명:** [ Instruction ]    
• Editor 화면에 작성되어진 list comprehension을 실행해 보자.    
• 어떤 값이 예상되는가?     
• 결과값과 당신이 예상한 값이 맞는지 확인하라. 
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
l = [i ** 2 for i in range(1, 11)]
# Should be [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]

print l[2:9:2]
```

**설명:** [ Solution ]     
• 리스트 컴프레션을 이용하여 리스트의 값을 구한다.     
• for 문에서 1(포함)부터 11(미포함) 값을 산출하여 변수 i 에 저장한다.    
• 변수 i 값을 제곱하여 리스트 l 에 추가한다.    
• 리스트의 값은 i 값의 제곱값이 저장된다.[1, 4, 9, 16, ... 81, 100]    
• 출력시 리스트 슬라이싱을 활용한다.    
• 슬라이싱 조건은 index 2번(포함) 부터 index 9(미포함) 사이의 값을 잘라낸다.    
• 슬라이싱 옵션은 첫번째를 기준으로 1칸씩 건너뛰어 출력한다.    
• index 2번 값은 9 이다. (포함)   
• index 9번 값은 100 이다. (미포함)    
• 이 사이의 값중 9부터 1칸씩 건너뛰니, [9, 25, 49, 81]가 출력된다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**결과**     
``` 
[9, 25, 49, 81]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 8. Omitting Indices    

If you don't pass a particular index to the list slice, Python will pick a default.    
```python
to_five = ['A', 'B', 'C', 'D', 'E']

print to_five[3:]
# prints ['D', 'E'] 

print to_five[:2]
# prints ['A', 'B']

print to_five[::2]
# print ['A', 'C', 'E']
```    
The default starting index is 0.
The default ending index is the end of the list.
The default stride is 1.




**설명:** [ Learn ]   
• Ch8. Omitting Indices 에서는 리스트 슬라이싱 활용을 학습한다.    
• 리스트에서 특정 index를 지정하지 못할 경우가 있다.    
• 이런경우, 범위와 조건을 주어 리스트의 특정 값을 골라 낼수 있다.     
• e.g. to_five[3:] 는 index 3번(포함)부터 마지막(미포함)의 값을 골라 낸다.    
• e.g. to_five[:2] 는 처음(포함)부터 index 2번(미포함)까지의 값을 골라 낸다.   
• e.g. to_five[::2] 는 처음(포함)부터 마지막(미포함)까지의 값중, 하나씩 건너 뛰면서 골라낸다.   
• index는 0 부터 시작한다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Use list slicing to print out every odd element of `my_list` from start to finish.

<p style="page-break-before: always;"></p>
<br>

* Omit the start and end index. You only need to specify a stride.

* Check the Hint if you need help.


**설명:** [ Instruction ]    
• 리스트 my_list 에서 홀수값만 골라 내어 출력하라.    
• 처음과 마지막을 표현한는 곳에는 값을 넣지 말라.     
• 옵션 조건(stride)을 활용하라.    
• 힌트를 참조하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, the syntax for list slicing is    

```python
[start:end:stride]
```    
* Since you're using the entire list, you should leave out the start and end indices (but leave in the colons!) and give the slice a stride that will select every other (that is, odd) element.


**설명:** [ Hint ]    
• [start(처음) : end(마지막) : stride(조건, 옵션)]        
• 처음과 마지막은 빈칸이란 의미는 전체를 사용해야 한다. (e.g. [ : : stride])    
• 홀수만 추출해야 하기에, 옵션인 조건(stride) 이 필요하다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
my_list = range(1, 11) # List of numbers 1 - 10

# Add your code below!
print my_list[::2]
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 1부터 10 까지의 정수를 생성한다.    
• 리스트 my_list 에 [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 ] 를 저장한다.    
• 리스트 my_list[::2] 를 출력한다.    
• 출력 조건은 다음과 같다.    
• index 처음(0)부터 끝(9)까지 추출한다.    
• 첫번째(index : 0)는 포함,    
• 마지막은(index : 10) 미포함.    
• 옵션은 1칸씩 건너뛴다.     
• e.g. my_list=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]    
• e.g. index -> 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10(Null) 
{: .notice--info}



**결과**     
``` 
[1, 3, 5, 7, 9]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 9. Reversing a List    

We have seen that a **positive stride** progresses through the list from left to right.

A **negative stride** progresses through the list from right to left.    
```python
letters = ['A', 'B', 'C', 'D', 'E']
print letters[::-1]
```    
In the example above, we print out ['E', 'D', 'C', 'B', 'A'].



**설명:** [ Learn ]     
• Ch9. Reversing a List 에서는 역순(Revers)을 학습한다.    
• 지금껏 옵션(stride)을 양수값만 주었다.    
• 양수값은 왼쪽부터 오른쪽으로 index를 읽는다.    
• 반대로 음수값을 주어 보자.    
• 옵션(stride)을 음수를 지정하면, 오른쪽부터 왼쪽으로 index를 읽어 처리한다.       
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a variable called `backwards` and set it equal to the reversed version of `my_list`.

* Make sure to reverse the list in the editor by passing your list slice a negative stride, like in the example above.


**설명:** [ Instruction ]    
• 리스트 backwards 를 생성하라.    
• 리스트 my_list 의 값을 역순으로 만들어, 리스트 backwards 에 저장하라.    
• Editor 화면에서, list slice의 옵션(stride)을 사용하여 역순으로 만들어라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
list_reverse[::-1] # reverse
```     

* Do not print `backwards`

**설명:** [ Hint ]    
• 리스트 옵션의 ( -1 ) 값은 리스트를 역순으로 슬라이싱 한다.    
• e.g. list_reverse[::-1]    
• 리스트 backwards 에 list_reverse의 역순값만 저장하고, 출력은 하지마라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
my_list = range(1, 11)

# Add your code below!
backwards = my_list[::-1]
```

**설명:** [ Solution ]     
• 리스트 my_list 에 1번(포함)부터 11번(미포함)까지의 값을 저장한다.    
• 리스트 my_list 를 오른쪽부터 읽어서 리스트 backwards 에 저장한다.    
• 리스트 backwards 에는 [ 10, 9, 8, 7, 6, 5, 4, 3, 2, 1] 이 저장된다.    
• 궁금하면, 살짝 print (backwards) 를 코딩하고, 실행 시켜 본다.    
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
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 10. Stride Length    

A positive stride length traverses the list from left to right, and a negative one traverses the list from right to left.

Further, a stride length of 1 traverses the list "by ones," a stride length of 2 traverses the list "by twos," and so on.



:**설명:** [ Learn ]    
• Ch10. Stride Length 에서는 리스트 옵션(stride)을 집중 학습한다.    
• 옵션인 stride(건너뛰다) 는 다음과 같이 동작한다.    
• 양수이면 왼쪽에서 오른쪽으로 진행한다.    
• 음수이면 오른쪽에서 왼쪽으로 진행한다.     
• 옵션(stride)의 값에 따라, 1 이면 1 칸씩 , 2 이면 2칸씩 건너뛴다.     
• 1 에서 2 로 가는것은 1 칸씩 건너뛰는 것이다.    
• 1 에서 3 으로 가는것은 2 칸씩 건너뛰는 것이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a variable, `backwards_by_tens`, and set it equal to the result of going backwards through `to_one_hundred` by tens. Go ahead and print `backwards_by_tens` to the console.


**설명:** [ Instruction ]    
• 역순 조건에서 건너뛰기(stride) 값을 주는것을 연습한다.    
• 리스트 backwards_by_tens 를 생성하라.        
• 리스트 to_one_hundred 에서 생성된 값을 역순으로 만들어라.        
• 리스트 to_one_hundred 를 역순으로 만들때, stride 값으로 10 칸씩 건너뛰게 하라.    
• 리스트 backwards_by_tens 에 to_one_hundred(역순&10칸) 을 저장하라.        
• 리스트 backwards_by_tens 를 출력하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)        
* Remember, the syntax is:      

```python
new_list = old_list[begin:end:stride]
```

**설명:** [ Hint ]    
• 리스트 슬라이싱 old_list[begin:end:stride] 를 활용하라.    
• stride 값으로 역순이고, 10 칸씩 건너뛰는 것은 -10 이다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
to_one_hundred = range(101)
# Add your code below!

backwards_by_tens = to_one_hundred[::-10]
print backwards_by_tens
```    

**설명:** [ Solution ]     
• 리스트 to_one_hundred 에 0(포함)부터 101(미포함)까지 값을 생성하여 저장한다.    
• 리스트 to_one_hundred[ : : -10] 은 역순으로 10 칸씩 건너뛰는 것이다.    
• [100, 99, 98, 97, 96,....,0] 중 10 칸씩 건너뛰면, [100, 90, 80, ...., 0]    
• 리스트 backwards_by_tens 를 출력한다.
{: .notice--info}



**결과**     
``` 
[100, 90, 80, 70, 60, 50, 40, 30, 20, 10, 0]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 11. Practice Makes Perfect    

Great work! See? This list slicing business is pretty straightforward.

Let's do one more, just to prove you really know your stuff.



**설명:** [ Learn ]    
• Ch11. Practice Makes Perfect 에서는 리스트 슬라이싱을 집중 학습한다.    
• List slicing 은 정말 유용하다. 그럼, 한번더 당신의 실력을 발휘해 보자.
{: .notice--info}


<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a list, `to_21`, that's just the numbers from 1 to 21, inclusive.

* Create a second list, `odds`, that contains only the odd numbers in the `to_21` list (1, 3, 5, and so on). Use list slicing for this one instead of a list comprehension.

* Finally, create a third list, `middle_third`, that's equal to the middle third of `to_21`, from 8 to 14, inclusive.


**설명:** [ Instruction ]    
• 리스트 변수 to_21 을 생성하고, 값을 1 부터 21 까지 저장하라.    
• 리스트 변수 odds 에 리스트 to_21 의 홀수 값(1,3,5,...)를 저장하라.     
• 단, list slicing 만 사용하라. (list comprehension 사용금지)    
• 리스트 middle_third 에 리스트 to_21 중 8 부터 14 까지 값을 저장하라.
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
to_21 = range(1, 22)
#print (to_21)
#[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21]
odds = to_21[::2]
#print (odds)
#[1, 3, 5, 7, 9, 11, 13, 15, 17, 19, 21]
middle_third = to_21[7:14]
#print (middle_third)
#[8, 9, 10, 11, 12, 13, 14]
```

**설명:** [ Solution ]     
• 함수 range(1, 22) 는 1 부터 21 까지 총 21 개 정수를 생성한다.         
• 리스트 슬라이싱 to_21[ : : 2] 는 index 0 부터 끝까지 잘라낸다.    
• Stride 2 는 2 칸씩 건너뛰어 값을 고른다.         
• 이 값을 리스트 odds 에 저장한다.    
• 리스트 슬라이싱 to_21[7 : 14] 는 index 7 부터 index 14 를 잘라낸다.    
• 이 값을 리스트 middle_third 에 저장한다.
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
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 12. Anonymous Functions    

One of the more powerful aspects of Python is that it allows for a style of programming called **functional programming**, which means that you're allowed to pass functions around just as if they were variables or values. Sometimes we take this for granted, but not all languages allow this!

Check out the code at the right. See the **lambda** bit? Typing    
```python
lambda x: x % 3 == 0
```    
Is the same as    
```python
def by_three(x):
  return x % 3 == 0
```     
Only we don't need to actually give the function a name; it does its work and returns a value without one. That's why the function the lambda creates is an anonymous function.    

When we pass the lambda to filter, filter uses the lambda to determine what to filter, and the second argument (my_list, which is just the numbers 0 – 15) is the list it does the filtering on.    




**설명:** [ Learn ]      
• Ch12. Anonymous Functions 에서는 람다(**lambda**)를 학습한다.    
• Python의 특징중 하나가, 변수나 값을 넘기듯이 함수 자체를 넘길수 있다는 것이다.    
• 이는 모든 언어에서 지원하는 것은 아니고, Python에서는 이 기능을 지원한다.    
• Python의 문법중, 독특한 것이 하나 있는데, 이는 함수 lambda 라는 것이다.    
• 함수 lambda 는 함수의 이름을 호출하지 않고도 anonymous(익명)함수를 만들어 동작한다.    
• 다음 장에서 함수 lambda 에 대한 자세한 문법을 배울것이다.     
• 함수 lambda 는 다음과 같이 동작한다.    
• 입력값을 인자에 넘겨(필터링 한다고 표현), 표현식을 진행하고 그 결과값을 다시 돌려받는다.    
• 함수 lambda 의 두번째 인수는 입력값 이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Can you guess what the this code will print to the console?    
* Click Run to see.


**설명:** [ Instruction ]    
• Editor 화면에 있는 소스를 실행시켜 어떻게 처리 되는지 살펴보자.
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
my_list = range(16)
print filter(lambda x: x % 3 == 0, my_list)
```

**설명:** [ Solution ]     
• 리스트 my_list 에 0 부터 15 까지의 숫자 16 개를 산출하여 저장한다.    
• 리스트 my_list 를 lambda 에 입력값으로 넘겨준다.    
• 리스트 my_list 값에서 하나씩 값을 추출하여 변수 x 에 저장한다.     
• 비교 연산 ( x % 3 == 0 ) 에 True 조건인것만 필터링 하여 뽑아낸다.    
• filtering 된 값을 출력한다.
{: .notice--info}



**결과**     
``` 
[0, 3, 6, 9, 12, 15]
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 13. Lambda Syntax    

Lambda functions are defined using the following syntax:    

```python
my_list = range(16)
filter(lambda x: x % 3 == 0, my_list)
```    
Lambdas are useful when you need a quick function to do some work for you.

If you plan on creating a function you'll use over and over, you're better off using def and giving that function a name.



**설명:** [ Learn ]    
• Ch13. Lambda Syntax 에서는 lambda 의 문법을 학습한다.    
• 함수 lambda 는 다음과 같이 사용한다.     
• e.g. filter(lambda x: x % 3 == 0, my_list)    
• 함수 lamda 를 정의할때, def 함수 선언이 필요없다.    
• 빠르게 한줄로 함수를 구현할때 사용이 가능하다.    
• 함수 이름을 지정할 필요도 없다.(Anonymous function)  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Fill in the first part of the `filter` function with a `lambda`. The `lambda` should ensure that only "Python" is returned by the filter.

* Fill in the second part of the filter function with languages, the list to filter.


**설명:** [ Instruction ]    
• filter 첫번째 항목에 함수 lambda 를 작성하라.    
• 함수 lambda 는 다음과 같이 동작한다.    
• 변수 x 가 입력된 리스트중 문자열값이 Python 과 같으면 그 결과를 반환한다.    
• filter 두번째 항목에 입력될 리스트를 넣어라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, `filter()` takes **two arguments**: the first is the function that tells it what to filter, and the second is the object to perform the filtering on.


**설명:** [ Hint ]    
• 함수 filter() 는 2개의 arguments 를 가진다.     
• 첫번째 인자는 필터링할 내용을 적어준다.    
• e.g. lambda x : x == "Python"    
• 두번째 인자는 필터링할 대상, 입력값을 적어준다.    
• e.g. 입력값 리스트 languages 를 적어준다.
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
languages = ["HTML", "JavaScript", "Python", "Ruby"]

# Add arguments to the filter()
print filter(lambda x: x == "Python", languages)
```

**설명:** [ Solution ]     
• 함수 filter() 에서 는 입력값이 문자열 Python 인것을 추출한다.    
• 함수 filter() 는 2개의 arguments 를 가지며, 다음과 같이 동작한다.    
• 첫번째 argument : 함수 lambda 를 실행시켜 변수 x 가 Python 인것만 반환한다.   
• 두번째 인자에는 입력값 리스트 languages 를 넣어준다.   
• filtering 된 결과값을 출력한다.
{: .notice--info}


**결과**     
``` 
['Python']
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 14. Try It!    

All right! Time to test out `filter()` and `lambda` expressions.    
```python
cubes = [x ** 3 for x in range(1, 11)]
filter(lambda x: x % 3 == 0, cubes)
```    
The example above is just a reminder of the syntax.



**설명:** [ Learn ]     
• Ch14. Try It! 에서는 람다(lambda)를 집중 추가 학습한다.    
• filter() 와 lambda 표현을 조금 더 연습해 보자.    
• 리스트 컴프레션을 사용하여, 1 부터 10 까지의 수를 세제곱(x ** 3)한 값을 생성한다.    
• 이 결과를 리스트 cubes 에 저장한다.     
• filter 첫번째 인자로 함수 lambda 를 사용하여 변수 x % 3 == 0 인값을 정의한다.     
• filter 두번째 인자로 리스트 cubes 를 입력 받는다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a list, `squares`, that consists of the squares of the numbers 1 to 10. A list comprehension could be useful here!

* Use `filter()` and a `lambda` expression to print out only the squares that are between 30 and 70 (inclusive).


**설명:** [ Instruction ]    
• 리스트 컴프레션을 사용하여 1 부터 10 까지의 제곱값을 생성한다.    
• 리스트 squares 에 이 값을 저장한다.    
• filter() 에서 lambda 를 사용하여 filtering 한다.    
• 첫번째 argument : lambda 조건은 입력값 중 30 이상 70 이하의 값을 추출한다.    
• 두번째 argument : 입력값은 리스트 squares 를 입력받는다.     
• filtering 한 결과를 출력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You'll want to filter for     

```python
x >= 30 and x <= 70.
```    

**설명:** [ Hint ]    
• lambda 조건식을 ( x >=30 and x <= 70 )을 활용하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
squares = [x ** 2 for x in range(1, 11)]

print filter(lambda x: x >= 30 and x <= 70, squares)
```

**설명:** [ Solution ]     
• list comprehension 을 사용하여 다음과 같이 동작한다.    
• 함수 range(1, 11) 을 사용하여 1 부터 10 까지를 산출한다.    
• for 문에서 x 값을 추출하여 제곱한 값을 산출한다.    
• 리스트 squares 에 산출한 값을 저장한다.    
• lambda를 사용하여 다음과 같이 filter() 한다.    
• 첫번째 argument : lambda 에서 변수 x 가 30 이상 & 70 이하인 조건만 추출한다.    
• 두번째 argument : 입력값으로 리스트 squares 를 입력 받는다.      
• filter() 결과값을 출력한다. 
{: .notice--info}


**결과**     
``` 
[36, 49, 64]
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 15. Iterating Over Dictionaries    

First, let's review iterating over a `dict`.



**설명:** [ Learn ]   
• Ch15. Iterating Over Dictionaries 에서는 딕셔너리리 반복을 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Call the appropriate method on `movies` such that it will print out all the items (hint, hint) in the dictionary—that is, each key and each value.




**설명:** [ Instruction ]    
• 적당한 함수를 이용하여 딕셔너리 movies 에 들어있는 항목들 key/value 값을 출력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You'll just want to print the result of calling the `.items()` method on your `movies`. No loops necessary!


**설명:** [ Hint ]    
• 메서드 .items() 를 활용하라.    
• 딕셔너리 movies 의 항목들 key/value 을 출력하여라.     
• loop 를 사용할 필요가 없다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
movies = {
  "Monty Python and the Holy Grail": "Great",
  "Monty Python's Life of Brian": "Good",
  "Monty Python's Meaning of Life": "Okay"
}

print ( movies.items() )
```

**설명:** [ Solution ]     
• 메서드 movies.items() 는 딕셔너리의 항목값들을 튜플 형태로 반환한다. 
{: .notice--info}

**결과**     
``` 
[("Monty Python's Life of Brian", 'Good'), ("Monty Python's Meaning of Life", 'Okay'), ('Monty Python and the Holy Grail', 'Great')]
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 16. Comprehending Comprehensions    

Good! Now let's take another look at list comprehensions.    
```python
squares = [x ** 2 for x in range(5)]
```



**설명:** [ Learn ]     
• Ch16. Comprehending Comprehensions 에서는 리스트 컴프레션을 집중 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Use a list comprehension to create a list, `threes_and_fives`, that consists only of the numbers between 1 and 15 (inclusive) that are evenly divisible by 3 or 5.


**설명:** [ Instruction ]    
• 리스트 threes_and_fives 를 생성하라.    
• 이 리스트에  1 부터 15 까지의 숫자중 3 or 5 로 나누어지는 떨어지는 값들만 저장하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, list comprehension syntax looks like this:    

<p style="page-break-before: always;"></p>
<br>

```python
list_name = [var for var in range]
```    

* You can include an optional `if` statement after the range. (You'll need such an `if` statement to check whether the numbers are evenly divisible by 3 or 5.)    

* Remember, modulo (`%`) is a good way to check if a number is evenly divisible by another.




**설명:** [ Hint ]    
• 리스트 컴프레션을 이용하여 작성하여야 한다.     
• for 문에서 내부 함수 range() 로 구한 값 만큼 loop(반복)한다.    
• for 문 블럭에서 다음과 같이 동작한다.    
• if 문과 모듈 연산자 ( % ) 를 이용하여 3 or 5 로 나누어지는 값을 구한다.     
• 출력할 필요는 없지만, print문을 사용하여 확인해 보는것도 좋다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
threes_and_fives = [x for x in range(1, 16) if x % 3 == 0 or x % 5 == 0]

#print (threes_and_fives)
#[3, 5, 6, 9, 10, 12, 15]
```

**설명:** [ Solution ]     
• 리스트 컴프레션을 사용하여 다음과 같이 동작한다.    
• for 문에서 함수 range(1,16) 으로 1 부터 15 까지의 값을 구한다.    
• 산출된 값을 하나씩 변수 x 에 대입한다.    
• 변수 x 가 3 or 5 로 나누어 떨어지는지 확인한다.     
• True 인 경우만, 맨앞 변수 x 저장된다.    
• 리스트 threes_and_fives 에 변수 x 값이 저장된다.   
• 변수 threes_and_fives 를 출력하면 [3, 5, 6, 9, 10, 12, 15] 가 출력할 것이다.
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
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 17. List Slicing    

Great! Next up: list slicing.    

```python
str = "ABCDEFGHIJ"
start, end, stride = 1, 6, 2
str[start:end:stride]
```   
You can think of a Python string as a list of characters.



**설명:** [ Learn ]     
• Ch17. List Slicing 에서는 리스트 슬라이싱을 집중 학습한다.    
• List slicing 을 복습해 보자.    
• 변수 str 의 문자열 "A B C D E F G H I J" 를 list slicing 으로 잘라내라.    
• 리스트 슬라이싱 조건은 다음과 같다.    
• start = 1(포함),  end = 6(미포함),  stride = 2(옵션)    
• str[1 : 6 : 2] 이다.     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* The string in the editor is garbled in two ways:

  * Our message is backwards.
  * The letter we want is every other letter.    
  * Use list slicing to extract the message and save it to a variable called message.




**설명:** [ Instruction ]    
• Editor 화면에 있는 문자열을 다음 2 가지 문제가 있다.         
• 글자를 거꾸로 읽어야 한다.    
• 우리가 원하지 않는 문자들이 섞여 있다.    
• List slicing 을 사용하여 변수 message 에 원하는 문자만 저장하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* It's important to remember that lists are mutable (changeable) in Python, but strings aren't; when you slice a string, you get back a new string.     
* The original string is unchanged unless you purposely "save over" it, like this:    

```python
my_string = "Monty Python"
# => Monty Python
my_string = my_string[:-7]
# => Monty
```

**설명:** [ Hint ]    
• 역순으로 읽는 법은 ( - ) 옵션을 준다.    
• index -7 부터 읽는 방법은 my_string[ : -7] 이다.    
• 역순 index도 0 부터 -1, -2 씩으로 읽는다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
garbled = "!XeXgXaXsXsXeXmX XtXeXrXcXeXsX XeXhXtX XmXaX XI"

message = garbled[::-2]

#print message
#I am the secret message!
```

**설명:** [ Solution ]     
• -2 값은 역순으로 -2 칸씩을 건너 뛰는 것이다.     
• 시작하는 첫번째 글자는 포함하기에 문자열 I 는 출력된다.    
• -2 칸씩 건너뛰기에, I 찍고, X 건너뛰고, " " 찍고, X 건너뛰고, a 찍고, ...     
• 마지막에 ! 를 찍는다.    
• 만약, print 문을 실행해 보면, 다음과 같이 결과가 나올 것이다.  
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**결과**     
``` 
I am the secret message!
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font>     

### 18. Lambda Expressions    

Last but not least, let's look over some `lambdas`.    
```python
my_list = range(16)
filter(lambda x: x % 3 == 0, my_list)
```     
We've given you another (slightly different) garbled. Sort it out with a `filter()` and a `lambda`.



**설명:** [ Learn ]     
• Ch18. Lambda Expressions 에서는 fileter() 와 lambda 를 집중 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a new variable called `message`.

* Set it to the result of calling `filter()` with the appropriate `lambda` that will filter out the "X"s. The second argument will be `garbled`.

* Finally, print your `message` to the console.




**설명:** [ Instruction ]    
• 변수 message 를 생성하라.         
• filter() 와 lambda 를 사용하여라.    
• Arguments 첫번째는 입력값에 문자열 X 를 제거한다.    
• Arguments 두번째는 입력값으로 리스트 garbled 를 입력받는다.    
• Filter() 된 값을 변수 message 에 저장한다.      
• 변수 message 값을 출력하라. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, a lambda expression looks like this:   

```python
lambda variable: variable expression
```    

* For example, you might have    

```python
lambda x: x != 10
```

**설명:** [ Hint ]    
• 함수 lambda 사용법은 다음과 같이 연산자 ( != ) 를 사용할 수 있다.    
• e.g. lambda x: x != 10     
• 변수 x 가 10 이 아닌 값이 변수 x 에 저장된다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
garbled = "IXXX aXXmX aXXXnXoXXXXXtXhXeXXXXrX sXXXXeXcXXXrXeXt mXXeXsXXXsXaXXXXXXgXeX!XX"

message = filter(lambda x: x != "X", garbled)
print message
```

**설명:** [ Solution ]     
• filter() 는 lambda 를 사용하여 다음과 같은 입력값을 받는다.    
• Argument 첫번째는 변수 x 가 문자열 X 가 아닌 값을 저장한다.     
• Argument 두번째는 입력값으로 리스트 garbled 를 입력받는다.    
• filter() 된 결과를 변수 message 에 저장한다.     
• 변수 message 를 출력한다.
{: .notice--info}


**결과**     
``` 
I am another secret message!
```   