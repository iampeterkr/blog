---
# layout : rchive
title: "Advanced Topics in Python"
permalink: /--/
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
이 장에서는 Python 을 활용한 다양한 자료구조를 학습한다. 딕셔너리, 리스트 등을 합칙, 분리하고, lambda 표현등을 학습한다. 
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
① editor 화면에 있는 소스를 이해하고 실행시켜 보아라. 
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
• 이 리스트 `even_squares`는 1부터 11사이의 숫자중 짝수의 제곱을 저장하는 리스트이다.
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
제곱은 `x ** 2`로 구하고, 짝수는 `x % 2 == 0`으로 구한다.
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
• 1부터 10까지의 숫자를 3제곱(cube) 하여 4로 나누어 떨어지는 값(X ** 3)을 리스트에 저장하라.     
• 위 결과가 담긴 리스트 `cubes_by_four`을 출력하라.    
리스트 `cubes_by_four`는 4로 나눈 나머지 값들이다. 원래 x 값이 아니라, x ** 3한 값을 저장하는 것이다.     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
#from 1 to 10
range(1,11)
```


**설명:** [ Hint ]    
• 1부터 10까지를 출력하려면, `range(1,11)`을 해야한다.    
• x ** 3 한 값이 `x%4 ==0` 인 값을 저장하는 것이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
cubes_by_four = [x ** 3 for x in range(1, 11) if ((x ** 3) % 4) == 0]
print cubes_by_four
```

**설명:** [ Solution ]     
• 8 은 `8%4==0`를 충족하고, x=2일때, `2 ** 3` 도 충족한다.      
• 16 은 `16%4==0`은 충족하지만 `x ** 3 = 16`은 충족하지 않는다.    
• 64 는 `64%4==0`을 충족하고, x=4일때, `4 ** 3`도 충족한다. 
{: .notice--info}



**결과**     
``` 
[8, 64, 216, 512, 1000]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 7. List Slicing Syntax    

* Sometimes we only want part of a Python list. Maybe we only want the first few elements; maybe we only want the last few. Maybe we want every other element!

* List slicing allows us to access elements of a list in a concise manner. The syntax looks like this:
```python
[start:end:stride]
```
* Where start describes where the slice starts (inclusive), end is where it ends (exclusive), and stride describes the space between items in the sliced list. For example, a stride of 2 would select every other item from the original list to place in the sliced list.



**설명:** [ Learn ]    
• 우리는 list의 일부분을 발췌하고 싶을때가 있다. 이럴때 List slicing 을 사용한다.    
• List slicing은 우리가 리스트를 간편하게 접근하게 해준다. 문법은 다음과 같다. `[시작:끝:간격]    
`시작(start)` : Slicing을 시작할 위치(포함)    
`끝(end)` : Slicing 끝낼 위치(포함하지 않음)    
`간격(stride)` : 시작을 포함하여 몇번째를 가져올지(옵션)
• 시작은 포함하고, 끝은 포함하지 않는다. 간격은 옵션으로 시작을 포함하여 몇 번씩 가져올지를 나타낸다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① We've generated a list with a list comprehension in the editor to the right, and we're about to print a selection from the list using list slicing. Can you guess what will be printed out? Click Run when you think you know!


**설명:** [ Instruction ]    
① Editor 화면에서 list comprehension을 돌려 보자. 어떤 값이 예상되는가? 결과값과 당신이 예상한 값이 맞는지 확인해 보라. 
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
l = [i ** 2 for i in range(1, 11)]
# Should be [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]

print l[2:9:2]
```

**설명:** [ Solution ]     
• 리스트의 값은 i 값의 제곱값이 저장된다.[1, 4, 9, 16, ... 81, 100]    
• 출력되는 값은 index 두번째 값인 9 부터(포함) index 아홉번째 값인 100(미포함)중, 9부터 2번째 항목인 `[9, 25, 49, 81]`가 출력 될 것이다.
{: .notice--info}


**결과**     
``` 
[9, 25, 49, 81]
```   

<br>
<br>    
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
리스트에서 특정 index를 지정하지 못할 경우에는, 범위와 조건을 주어 리스트의 특정 값을 골라 낼수 있다.     
[예]    
• `to_five[3:]` 는 index 3번(포함)부터 마지막(불포함)까지의 값을 골라 낸다.    
• `to_five[:2]` 는 처음(포함)부터 index 2번(불포함)까지의 값을 골라 낸다.   
• `to_five[::2]`는 처음(포함)부터 마지막(불포함)까지의 값 중, 하나씩 건너 뛰면서 골라낸다.   
• index의 처음은 0부터 시작한다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Use list slicing to print out every odd element of `my_list` from start to finish.

* Omit the start and end index. You only need to specify a stride.

* Check the Hint if you need help.


**설명:** [ Instruction ]    
① `my_list` 에서 홀수 값만 골라 내어 출력하여라.    
• 처음과 마지막을 표현한는 곳에는 값을 넣지 말라. 옵션인 조건(stride)을 활용하여라.    
• 힌트를 참조하여라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember, the syntax for list slicing is
```python
[start:end:stride]
```
Since you're using the entire list, you should leave out the start and end indices (but leave in the colons!) and give the slice a stride that will select every other (that is, odd) element.


**설명:** [ Hint ]    
`[start(처음):end(마지막):stride(조건, 옵션)]`    
• 전체를 사용해야 하므로 `[::stride]` 처음과 마지막에 빈칸이어야 한다.     
• 홀수만 추출해야 하기에, 옵션인 `조건(stride)`을 주어야 한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
my_list = range(1, 11) # List of numbers 1 - 10

# Add your code below!
print my_list[::2]
```

**설명:** [ Solution ]     
• 1부터 10까지의 정수를 리스트 `my_list=[1,2,3,4,5,6,7,8,9,10]`에 생성한다.   
• `my_list[::2]`를 index 처음(0)부터 끝(9)까지 추출하는데, 첫번(0)째 index부터 2칸 뛴 값 들을 출력한다.
• my_list=[1,2,3,4,5,6,7,8,9,10]    
• index -> 0,1,2,3,4,5,6,7,8, 9 
{: .notice--info}



**결과**     
``` 
[1, 3, 5, 7, 9]
```   

<br>
<br>    
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
지금껏 옵션(stride)을 양수값만 주었는데, 양수값은 왼쪽부터 오른쪽으로 index를 읽는다. 반대로 이번에는 음수값을 주어 보자.    
• 옵션(stride)을 음수를 지정하면, 오른쪽부터 왼쪽으로 index를 읽어 처리한다.       
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Create a variable called `backwards` and set it equal to the reversed version of `my_list`.

Make sure to reverse the list in the editor by passing your list slice a negative stride, like in the example above.


**설명:** [ Instruction ]    
① 리스트 변수 `backwards`를 만들어서, `my_list`의 값을 역순으로 `backwards`에 저장하라.    
• Editor 화면에서, list slice의 옵션(stride)를 사용하여 역순으로 만들어라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
list_reverse[::-1] # reverse
```
Do not print `backwards`

**설명:** [ Hint ]    
`list_reverse[::-1]`는 리스트를 역순으로 만든다. 역순인 `backwards`만 만들고 출력은 하지 마라.
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
`backwards`에는 [ 10, 9, 8, 7, 6, 5, 4, 3, 2, 1] 이 저장 될 것이다.    
궁금하면, 살짝 `print (backwards)`를 코딩하고, 실행 시켜 본다. 확인후 print문은 지우고 다음으로 넘어가자.
{: .notice--info}



**결과**     
``` 
skip
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 10. Stride Length    

A positive stride length traverses the list from left to right, and a negative one traverses the list from right to left.

Further, a stride length of 1 traverses the list "by ones," a stride length of 2 traverses the list "by twos," and so on.



:**설명:** [ Learn ]     
• 옵션인 stride(건너뛰다) 는 양수이면 왼쪽에서 오른쪽으로, 음수이면 오른쪽에서 왼쪽으로 진행한다.  
• 게다가 stride의 값에 따라, 1이면 1칸씩 , 2이면 두칸씩 건너뛴다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Create a variable, `backwards_by_tens`, and set it equal to the result of going backwards through `to_one_hundred` by tens. Go ahead and print `backwards_by_tens` to the console.


**설명:** [ Instruction ]    
① 역순 list slicing에서 stride 값을 주는것을 연습해 보자.    
• 리스트 변수 `backwards_by_tens`를 만들어라.    
• 리스트 `to_one_hundred`에서 생성된 값을 역순으로 만어라.    
• `to_one_hundred`를 역순으로 만들때, 옵션으로 10칸씩 건너뛰게 하라.    
• 생성된 값을 `backwards_by_tens`에 넣어라.     
• 그리고 `backwards_by_tens`를 출력한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember, the syntax is:
```python
new_list = old_list[begin:end:stride]
```

**설명:** [ Hint ]    
• `old_list[begin:end:stride]`를 활용하세요.    
• stride 값으로 역순이고, 10칸씩 건너뛰는 것은 -10
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
• `range(101)`은 0부터 100까지 총 101개 생성한다.   
• `to_one_hundred[::-10]`은 역순으로 10칸씩 건너뛰는 것이다.
{: .notice--info}



**결과**     
``` 
[100, 90, 80, 70, 60, 50, 40, 30, 20, 10, 0]
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 11. Practice Makes Perfect    

Great work! See? This list slicing business is pretty straightforward.

Let's do one more, just to prove you really know your stuff.



**설명:** [ Learn ]    
list slicing은 정말 유용하다. 그럼, 한번더 당신이 실력 발휘를 해보세요.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Create a list, `to_21`, that's just the numbers from 1 to 21, inclusive.

* Create a second list, `odds`, that contains only the odd numbers in the `to_21` list (1, 3, 5, and so on). Use list slicing for this one instead of a list comprehension.

* Finally, create a third list, `middle_third`, that's equal to the middle third of `to_21`, from 8 to 14, inclusive.


**설명:** [ Instruction ]    
① 리스트 변수 `to_21`을 만들고, 값을 1부터 21까지 저장하라.    
• 리스트 변수 `odds`에 `to_21`의 홀수 값(1,3,5,...)를 입력하라. 단, list slicing만 사용하여야 한다.(list comprehension사용하지 말라.)    
• 리스트 변수 `middle_third`에 `to_21`중 8부터 14까지 값을 저장하라.
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
• `range(1,22)`는 1붜 21까지 총 21개 정수 발생    
• `to_21[::2]`는 index 0 값(1)부터 끝까지 중 2칸씩 건너뛰어 발생   
• `to_21[7:14]`는 index 7값(8)부터 index 14(15) 값을 발생
{: .notice--info}



**결과**     
```
skip
```   

<br>
<br>    
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
• Python의 특징중 하나가, 변수나 값을 넘기듯이 함수 자체를 넘길수 있다는 것이다. 이는 모든 언어에서 지원하는 것은 아니고, Python에서는 이 기능을 지원한다.    
• Python의 특징중, 독특한 것이 하나 있는데, `lambda`라는 것이다. `lambda`는 함수의 이름을 호출하지 않고도 함수를 호출하여 계산한 것처럼, anonymous함수를 만들어 동작한다. 다음장에서 `lambda`에 대한 자세한 문법을 배울것이다. 
• `lambda`는 입력값에서 값을 인자에 넘겨(필터링 한다고 표현), 표현식을 진행하고 그 결과값을 다시 돌려 받는다.`lambda`의 두번째 인수는 입력값 이다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Can you guess what the this code will print to the console? Click Run to see.


**설명:** [ Instruction ]    
① Editor 화면에 있는 소스를 실행시켜 어떻게 처리 되는지 알아보자.
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
my_list = range(16)
print filter(lambda x: x % 3 == 0, my_list)
```

**설명:** [ Solution ]     
• 입력값 `my_list`에서 값을 추출하여 `x`에 저장한다.     
• `x%3==0`인것만 `filter` 하여 뽑아낸다.    
• 출력한다.
{: .notice--info}



**결과**     
``` 
[0, 3, 6, 9, 12, 15]
```   

<br>
<br>    
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
`lambda`함수는 다음 예와 같이 사용한다.     
`filter(lambda x: x % 3 == 0, my_list)`    
`lamda`는 함수를 정의할때, `def`함수 선언이 필요없이 빠르게 한줄로 함수를 구현할때 사용이 가능하다. 함수 이름을 줄 필요도 없다.(Anonymous function)  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Fill in the first part of the `filter` function with a `lambda`. The `lambda` should ensure that only "Python" is returned by the filter.

• Fill in the second part of the filter function with languages, the list to filter.


**설명:** [ Instruction ]    
① `filter` 첫번째 항목에 `lambda`를 사용하라. `lambda` 기능은 `x`가 "Python"인지를 확인한여 맞으면 `filter`에 그 결과를 반환한다.    
•  `filter` 두번째 항목에 전달할 리스트를 넣어라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember, `filter()` takes **two arguments**: the first is the function that tells it what to filter, and the second is the object to perform the filtering on.


**설명:** [ Hint ]    
• `filter()`함수는 2개의 arguments를 가진다.     
• 첫번째 인자는 필터링할 내용(즉, 조건 `lambda x:x=="Python"`)을 적어준다.    
• 두번째 인자는 필터링할 대상(즉, 입력값 `languages`)를 적어준다.
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
languages = ["HTML", "JavaScript", "Python", "Ruby"]

# Add arguments to the filter()
print filter(lambda x: x == "Python", languages)
```

**설명:** [ Solution ]     
• `filter()`함수에서 첫번째, `lambda`를 실행시켜 `x`가 "Python" 인것만 반환한다.   
• 두번째 인자에는 입력값 `languages`를 넣어준다.   
• 그 결과값을 반환한다.
{: .notice--info}


**결과**     
``` 
['Python']
```   

<br>
<br>    
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
• `filter()`과 `lambda`표현을 조금 더 연습해 보자.    
• list comprehension을 사용하여 변수 리스트 `cubes`에 `x`가 1부터 10까지의 x 값을 이용하여 `x ** 3`값을 저장한다. 
• `filter`에서 `cubes`를 입력받아, `x % 3 ==0`값을 골라 낸다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Create a list, `squares`, that consists of the squares of the numbers 1 to 10. A list comprehension could be useful here!

* Use `filter()` and a `lambda` expression to print out only the squares that are between 30 and 70 (inclusive).


**설명:** [ Instruction ]    
① 변수 리스트 `squares`에  1부터 10까지의 제곱 값을 list comprehension 을 사용하여 저장하라.   
• `filter()`, `lambda`를 사용하여 제곱 값중 30과 70이하의 값을 출력하라. 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You'll want to filter for 
```python
x >= 30 and x <= 70.
```

**설명:** [ Hint ]    
`x >=30 and x <= 70`을 활용하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
squares = [x ** 2 for x in range(1, 11)]

print filter(lambda x: x >= 30 and x <= 70, squares)
```

**설명:** [ Solution ]     
• list comprehension 을 사용하여 1부터 10까지를 산출(`range(1,11)`)한 값을 제곱(`x ** 2`)한 결과를 변수 `squares`에 저장한다.     
• `filter()`를 사용하여 입력값 `squares`를 두번째 인자에 넣고, `lambda`로 조건(`x>=30 and x<=70`)을 첫번째 인자에 기술한다.    
• `filter()`결과값을 출력한다. 
{: .notice--info}


**결과**     
``` 
[36, 49, 64]
```   



<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
### 15. Iterating Over Dictionaries    

First, let's review iterating over a `dict`.



**설명:** [ Learn ]   
딕셔너리의 반복을 다시 복습해 보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Call the appropriate method on `movies` such that it will print out all the items (hint, hint) in the dictionary—that is, each key and each value.




**설명:** [ Instruction ]    
① 적당한 내재 함수를 이용하여 변수 `movies`에 들어있는 항목들 key/value값을 출력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You'll just want to print the result of calling the `.items()` method on your `movies`. No loops necessary!


**설명:** [ Hint ]    
`.items()`를 활용하여 딕셔너리 `movies`의 항목들 key/value을 출력하여라. loop를 사용할 필요가 없다. 
{: .notice--info}

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
`movies.items()`는 딕셔너리의 항목값들을 튜플 상태로 반환해 준다. 
{: .notice--info}

**결과**     
``` 
[("Monty Python's Life of Brian", 'Good'), ("Monty Python's Meaning of Life", 'Okay'), ('Monty Python and the Holy Grail', 'Great')]
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">ADVANCED TOPICS IN PYTHON </font> 
## 16. Comprehending Comprehensions    

Good! Now let's take another look at list comprehensions.
```python
squares = [x ** 2 for x in range(5)]
```



**설명:** [ Learn ]     
list comprehensions를 복습해 보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Use a list comprehension to create a list, `threes_and_fives`, that consists only of the numbers between 1 and 15 (inclusive) that are evenly divisible by 3 or 5.


**설명:** [ Instruction ]    
① 변수 리스트`threes_and_fives`를 만들고, 1부터 15까지의 숫자중 3 or 5로 나누어 떨어지는 값들만 저장하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember, list comprehension syntax looks like this:
```python
list_name = [var for var in range]
```
You can include an optional `if` statement after the range. (You'll need such an `if` statement to check whether the numbers are evenly divisible by 3 or 5.)

Remember, modulo (`%`) is a good way to check if a number is evenly divisible by another.




**설명:** [ Hint ]    
• `for`문으로 `range()`를 구하고, 그 밑에 `if`문과 모듈연산자 `%`를 이용하여 3 or 5로 나누어 지는 값을 구한다. 
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
`for`문으로 `range(1,16)`으로 1부터 15까지의 값을 구하고, 그값 `x`가 `x%3==0 or x%5==0`인지를 확인하고, 그 결과를 맨 앞 `x`에 넣어서 저장한다. 
변수 `threes_and_fives`를 출력하면 `[3,5,6,9,10,12,15]`가 출력할 것이다.
{: .notice--info}


**결과**     
``` 
skip
```   

<br>
<br>    
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
list slicing을 복습해 보자.    
변수 문자열 `str`의 무자열을 list slicing으로 `[1:6:2]`즉, 1번(포함) index부터 6번(미포함) index까지의 값중 2칸씩 건너 뛰어 저장하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① The string in the editor is garbled in two ways:

* Our message is backwards.
* The letter we want is every other letter.    
Use list slicing to extract the message and save it to a variable called message.




**설명:** [ Instruction ]    
① Eeditor 화면에 있는 문자열을 다음 2가지 문제가 있다.         
• 글자를 거꾸로 읽어야 한다.    
• 우리가 원하지 않는 문자들이 섞여 있다.    
list slicing을 사용하여 변수 `message`에 원하는 문자만 저장해라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
It's important to remember that lists are mutable (changeable) in Python, but strings aren't; when you slice a string, you get back a new string. The original string is unchanged unless you purposely "save over" it, like this:
```python
my_string = "Monty Python"
# => Monty Python
my_string = my_string[:-7]
# => Monty
```

**설명:** [ Hint ]    
• 역순으로 index -7부터 읽는 방법은 `my_string[:-7]`이다.    
• 역순 index도 0부터 -1,-2 씩으로 읽는다.
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
• -2값은 1칸씩을 건너 뛰는 것이다. 첫번째 글자는 포함하고 즉, I 찍고, X 건너뛰고, " "찍고, X건너뛰고, a찍고, X건너뛰고......마지막에 !를 찍는다.    
• 만약, print문을 실행해 보면, 다음과 같이 결과가 나올 것이다.  
{: .notice--info}


**결과**     
``` 
I am the secret message!
```   

<br>
<br>    
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
`fileter()`와 `lambda`를 사용하여 복습해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① Create a new variable called `message`.

* Set it to the result of calling `filter()` with the appropriate `lambda` that will filter out the "X"s. The second argument will be `garbled`.

Finally, print your `message` to the console.




**설명:** [ Instruction ]    
① 변수 `message`를 만들어라.    
• `filter()`와 `lambda`를 사용하여 입력값 `garbled`에 있는 "X"를 제거하라.    
• 변수 `message`에 의 결과값을 저장하여라.    
• 변수 `message`값을 출력하여라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember, a lambda expression looks like this:
```python
lambda variable: variable expression
```
For example, you might have
```python
lambda x: x != 10
```

**설명:** [ Hint ]    
• `lambda` 사용법은 `lambda x: x != 10`와 같이 `x`가 10이 아닌 값을 `x`에 저장한다.
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
• `filter()`에 입력값 `garbled`를 두번째 인수에 입력한다.    
• 첫번째 인수에는 `lambda x: x != "X"`의 조건값을 실행하여 `x`가 "X"가 아닌 값만 `lambda` `x`에 저장한다.    
• 최종, `filter()`값이 반환되어 출력된다.
{: .notice--info}


**결과**     
``` 
I am another secret message!
```   

<br>
<br>    
<br>    