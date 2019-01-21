---
# layout : rchive
title: "Advanced Topics in Python"
permalink: /advanced-topics-python/
excerpt: "We learn about String, Console, and Output Syntax."
last_modified_at: 2019-01-18T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
<hr style="border: solid 1px #dddddd ;">    
LESSON

In this lesson, we'll cover some of the more complex aspects of Python, including iterating over data structures, list comprehensions, list slicing, and lambda expressions.      

**설명:** [ 학습방향 ]     
이 장에서는 Python 을 활용한 다양한 자료구조를 학습한다. 딕셔너리, 리스트 등을 합칙, 분리하고, lambda 표현등을 연습한다. 
{: .notice--info}  
    
<hr style="border: solid 1px #dddddd ;">    


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
딕셔너리의 반복문에 대해서 연습해 보자. 앞에서 배운 딕셔너리의 key 와 value를 조작하는 법을 연습해 본다.    
`d.items()`는 딕셔너리 `d`의 key 와 value를 리스트로 보여준다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Create your own Python dictionary, `my_dict`, in the editor to the right with **two or three key/value** pairs.

Then, print the result of calling the `my_dict.items()`.


**설명:** [ Instruction ]    
① 딕셔너리 `my_dict{}`작성하여라. 이 딕셔너리는 2, 3개의 key/value 쌍을 가지고 있다.    
• `my_dict.item()`를 실행하여 그 결과를 출력하라.     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can think of dictionaries as unordered key/value pairs.


**설명:** [ Hint ]    
딕셔너리는 key/value가 출력될때, 입력한 순으로 정렬되지 않습니다.
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

**설명:** [ Solution ]     
딕셔너리 `my_dict`에 `name`, `age`, `occupation`를 key/value 쌍으로 입력한후, `my_dict.items()`내재 함수로 출력하였다.
{: .notice--info}


**결과**     
```
[('age', 31), ('name', 'Nick'), ('occupation', 'Dentist')]
```   

<br>
<br>    
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
`.items()` 내재 함수는 딕셔너리에서 key/value로 구성된 각각의 튜플 형태의 배열로 반환 됩니다.    
• `.keys()` 내재 함수는 딕셔너리의 key값을 리스트 형태로 반환 됩니다.    
• `.values()` 내재 함수는 딕셔너리의 value값을 리스트 형태로 반환 됩니다.   
• key와 value 값은 순서 없이 반환 됩니다.    
• 튜플은 리스트와 동일하지만, 틀린점은 `()`로 둘러쌓인 그 항목 값을 변경할 수 없습니다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Remove your call to `.items()` and replace it with a call to `.keys()` and a call to `.values()`, each on its own line. Make sure to print both!


**설명:** [ Instruction ]    
① `.item()`를 지우고, 대신에 `.keys()`와 `.values()`로 대체하여라. 그리고 각각을 출력하여라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
For instance, your call to `my_dict.keys()` might look like:
```python
print my_dict.keys()
```

**설명:** [ Hint ]   
`my_dict.keys()`는 key만 출력하는 것이다. 
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
• `my_dict.keys()`는 key만 리스트 형태로 출력한다.    
• `my_dict.values()`는 value만 리스트 형태로 출력한다. 
{: .notice--info}


**결과**     
``` 
['age', 'name', 'occupation']
[31, 'Nick', 'Dentist']
```   

<br>
<br>    
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
1. In the example above, first we create and iterate through a range, printing out 0 1 2 3 4. Note that the trailing comma ensures that we keep printing on the same line.
2. Next, we create a dictionary and iterate through, printing out age 26 name Eric. Dictionaries have no specific order.
Finally, we iterate through the letters of a string, printing out E r i c.
  



**설명:** [ Learn ]     
리스트(list), 튜플(tuple), 딕셔너리(dictionarie), 문자열(string)을 반복적으로 추출할때 직관적으로 `in`을 사용할 수 있다.     
① `range(5)`로 0,1,2,3,4를 출력할때, `,`를 사용하면 같은 줄에 문자열을 출력할수 있다.     
② 딕셔너리는 순차적으로 출력이 안된다. 그리고 E r i c로 출력된다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① For each key in `my_dict`: print out the key , then a space, then the value stored by that key. (You should use print a, b rather than print a + " " + b.)


**설명:** [ Instruction ]    
① 딕셔너리 `my_dict`를 key를 출력하고 중간에 공백 하나가 있고, 그다음에 value가 출력되도록 하라. `print a + " " + b` 보다는 `print a, b`를 사용하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You'll want to do something like this:
```python
for key in some_dict:
  print key, some_dict[key]
```

**설명:** [ Hint ]    
`print (key , some_dict[key])`key 와 some_dict[key] 사시에 공백이 있어야 한다. 
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

for key in my_dict:
  print key, my_dict[key]
```

**설명:** [ Solution ]     
딕셔너리 `my_dict`에서 key 값을 읽어서, 해당 key 와 value값(my_dict[key])을 출력한다. 
{: .notice--info}



**결과** 
```
age 31
name Nick
occupation Dentist
```

<br>
<br>    
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
0부터 50까지의 정수를 리스트에 저장하고 싶으면 `my_list = range(51)`이라고 사용하면 된다. 만약, 0부터 50사이의 짝수만 저장하고 싶다면?     
Python 에서는 우리가 익히 잘 사용하는 for/if문을 사용하여 list comprehension을 기능을 사용하면 쉽게 만들수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Check out the list comprehension example in the editor. When you're pretty sure you know what it'll do, click Run to see it in action.


**설명:** [ Instruction ]    
① edit 창에 있는 소스를 이해하고 실행시켜 보아라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
skip


**설명:** [ Hint ]    
skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
evens_to_50 = [i for i in range(51) if i % 2 == 0]
print evens_to_50
```

**설명:** [ Solution ]     
리스트 안에 for 문과 if문을 두어 해당 결과값이 for 앞에 있는 i에 저장되어 리스트에 i 값이 장된다. 
{: .notipce--info}



**결과**     
``` 
[0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50]
```   

<br>
<br>    
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
다음 예제는 list comprehension에 관한것이다.    
• `new_list = [ x for x in range(1, 6)]`는 맨 앞 x에 for 문 결과값이 저장된다.    
• `doubles = [x * 2 for x in range(1, 6)]`는 맨 앞 x에 for문 결과값이 저장되고 그 결과에에  `x * 2` 한값이 저장된다.   
• `doubles_by_3 = [x * 2 for x in range(1, 6) if (x * 2) % 3 == 0]` for문과 if문이 실행되어 만족한 x 값 3이 맨앞 x 변수에 저장되어, 그 값에 `x * 2`한 값 6이 리스트에 저장된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Use a list comprehension to build a list called `even_squares` in the editor.

Your `even_squares` list should include the squares of the even numbers between 1 to 11. Your list should start [4, 16, 36...] and go from there.


**설명:** [ Instruction ]    
① 리스트 `even_squares`를 만들어라.     
• 이 리스트 `even_squares`는 1부터 11사이의 숫자중 짝수의 제곱근을 저장하는 리스트이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can use `x ** 2` to square a number, and `x % 2 == 0` to check if it's even.
```python
# from 1 to 10
range(1,11) 
# from 1 to 11
range(1,12)
```

**설명:** [ Hint ]    
제곱근은 `x ** 2`로 구하고, 짝수는 `x % 2 == 0`으로 구한다.
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

**설명:** [ Solution ]     
• 먼저 for문을 실행하여 1부터 11까지의 숫자를 변수 x에 저장된다.    
• if 문에서 추출된 x 의 값이 2로 나누어 나머지가 0이면, 즉 짝수인지를 판단하고,   
• x가 if 조건을 만족하면 해당 x 값의 제곱을 구하여 리스트에 저장한다.   
{: .notice--info}



**결과**     
``` 
[4, 16, 36, 64, 100]
```

<br>
<br>    
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
for문에서 5개의 x값을 구하고 이 x 값이 3보다 작은 경우는 0, 1, 2이다. 즉, 3번의 'C'문자가 리스트에 저장되고, 이 리스트 c 를 출력한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Use a list comprehension to create a list, `cubes_by_four`.

* The comprehension should consist of the cubes of the numbers 1 through 10 only if the cube is evenly divisible by four.

* Finally, print that list to the console.

Note that in this case, the cubed number should be evenly divisible by 4, not the original number.




**설명:** [ Instruction ]    
① 리스트 `cubes_by_four`에 list comprehension을 만들어라.     
• 1부터 10까지의 숫자를 3제곱(cube) 하여 4로 나누어 떨어지는 값을 리스트에 저장하라.     
• 위 결과가 담긴 리스트 `cubes_by_four`을 출력하라.    
리스트 `cubes_by_four`는 4로 나눈 나머지 값들이다.    


{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}



**결과**     
``` 
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 7. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}


**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 8. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}



**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 9. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}



**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 10. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}



**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 11. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}



**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 12. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}



**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 13.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}


**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 14. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

**결과**     
``` 
```   

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}


**결과**     
``` 
```   



<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 15.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}

**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 16. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}


**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 17.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}


**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 18.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}


**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 19.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     
{: .notice--info}


**결과**     
``` 
```   


<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
