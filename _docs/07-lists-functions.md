---
# layout : rchive
title: "Lists and Functions"
permalink: /lists-functions/
excerpt: "We learn about lists and functions."
last_modified_at: 2019-01-02T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    
 <hr style="border: solid 1px #dddddd ;">

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 1. List accessing    

This exercise goes over just pulling information from a list, which we've covered in a previous section! 



**설명:**    
리스트의 항목값을 접근하는 방법을 배운다. 이미 우리는 앞장에서 이와 관련하여 해보았다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Please add the code to print out the second element in the list.


**설명:** ① 리스트 `n`의 두번째 항목을 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember that elements in a list start from index 0 and they are accessed in the form
```python
x[n]
```
where `x` is the name of the list and n is the index in that list that you're trying to access.


**설명:**     
리스트의 인덱스는 0 부터 시작한다. 만약 첫번째 자리의 값을 접근할려면 `n[0]`으로 해야 한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = [1, 3, 5]

# Add your code below
print n[1]
```

**설명:**     
리스트 n 의 `3`을 접근할려면, `n[1]`로 해야 한다. 
{: .notice--info}


**결과** 
``` 
3
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 2. List element modification   

You've already learned how to modify elements of a **list** in a previous section. This exercise is just a recap of that! 



**설명:**     
앞장에서 배운 리스트를 다시한번 연습해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** On line 3, multiply the second element of the `n` list by `5`

**Overwrite** the second element with that result.

Make sure to print the list when you are done!


**설명:**     
① 3 라인에서, 두번째 항목의 `3`값에 `x 5`한 값으로 변경하시오. 작업이 완료되면 출력하시오. 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
An item in a list in Python can be set to a value using the form
```python
x[n] = v
```
where x is the name of the list, n is the index in the array and v is the value you want to set.


**설명:**    
리스트의 특정 항목을 변경하기 위해서는 `x[n]=v`와 같이 `n:index`, `v=값`이다.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = [1, 3, 5]
# Do your multiplication here
n[1] = n[1] * 5
print n
```

**설명:**     
인덱스 1번(두번째값) 자리에, `n[1]`값에다 x 5 한 값을 저장한다. 
{: .notice--info}


**결과** 
``` 
[1, 15, 5]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 3. Appending to a list    

Here, we'll quickly recap how to `.append()` elements to the end of a list.



**설명:**     
리스트에  `.append()`를 이용하면, 제일 마지막에 값을 추가할 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Append the number 4 to the end of the list n.


**설명:**     
① 리스트 `n[]`에 정수 4를 추가하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
The function to append to the end of a list is
```python
x.append(item)
```
where `x` is the name of the list and item is the object you want to append.


**설명:**     
리스트 `x` 에 `.append(item)`을 활용하라.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = [1, 3, 5]
# Append the number 4 here
n.append(4)
print n
```

**설명:**     
`n.append(4)`는 리스트의 맨 끝에 추가된다. 
{: .notice--info}



**결과** 
``` 
[1, 3, 5, 4]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 4. Removing elements from lists    

This exercise will expand on ways to **remove items from a list**. You actually have a few options. For a list called `n`:

`n.pop(index)` will remove the item at index from the list and return it to you:

```python
n = [1, 3, 5]
n.pop(1)
# Returns 3 (the item at index 1)
print n
# prints [1, 5]
```
`n.remove(item)` will remove the actual item if it finds it:
```python
n.remove(1)
# Removes 1 from the list,
# NOT the item at index 1
print n
# prints [3, 5]
```
`del(n[1])` is like `.pop` in that it will remove the item at the given index, **but it won't return it**:
```python
del(n[1])
# Doesn't return anything
print n
# prints [1, 5]
```




**설명:**     
리스트의 항목값을 삭제 하는 것을 다시 연습해보자.    
`n.pop(index)` index 값에 해당하는 항목이 삭제 된다. 
`n.remove(1)`  값 1을 찾아서 그 값이 삭제 된다. 
`del(n[`])` index 값에 대항하는 항목이 삭제 된다. (단, 결과값이 return 안된다. ex. print del(n[0]) 사용할 수 없다.)
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Remove the first item from the list n using either `.pop()`, `.remove()`, or `del`.


**설명:**     
① 리스트 `n`를 `.pop()`, `.remove()`, `del`중 하나를 사용하여 첫번째 값을 지워라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
One way of doing this would be
```python
n.pop(0)
```
where x is the list and index is the item you want to pop off the list. If no index is given, it removes the last item from the list.



**설명:**     
`n.pop(0)`은 첫번째 인덱스를 지우는 것이다. 만약, 인덱스 값을 주지 않으면 마지막 인덱스를 지운다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = [1, 3, 5]
# Remove the first item in the list here
n.pop(0)
print n
```

**설명:**     
`n.pop(0)`을 사용하여 첫번째 값을 지웠다. 
{: .notice--info}



**결과** 
``` 
[3, 5]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 5. Changing the functionality of a function    

In this exercise, you will just be making a minor change to a function to change what that function does.



**설명:**     
함수를 설명하기 위해서 함수를 약간 변형해 볼것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Change the function so the given argument is multiplied by 3 and returned.


**설명:**     
① 주어진 함수를 입력값에 `x 3`한후 그 결과값을 반환하는 하는 기능을 하는 함수로 변경하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You'll want to change the `+` to a `*`.


**설명:**     
`+` 를 `*`로 변경하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
number = 5

def my_function(x):
    return x * 3

print my_function(number)
```

**설명:**     
입력값 `x`를 x 3하여 반환한다. 
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
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 6. More than one argument    

This exercise will recap how to use **more than one argument** in a function.



**설명:** 입력 argument가 1개 이상 일때를 연습해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function called `add_function` that has `2` parameters `x` and `y` and adds them together.


**설명:**     
① 함수 `add_function`은 `x`, `y` 2개의 parameters를 가지는 함수를 정의하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
A function is defined as follows:
```python
def my_function(argument1, argument2, etc.):
  # Function body goes here
     return argument1 + argument2
```


**설명:**     
함수의 parameters 갯수는 다음과 같이 `def my_function(argument1, argument2, etc.):` 정의한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
m = 5
n = 13
# Add add_function here!
def add_function(x, y):
  return x + y

print add_function(m, n)
```

**설명:**     
`x`, `y` parameter로 입력 받은 값 m=5, n=13을 더하는 함수이다. 
{: .notice--info}



**결과** 
``` 
18
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 7. Strings in functions    

This is a basic recap on using strings in functions.



**설명:**   
함수에서 문자열을 사용하는 방법을 연습해 보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Write a function called `string_function` that takes in a string argument `(s)` and then returns that argument **concatenated** with the word `'world'`. Don't add a space before world!


**설명:**     
① 함수 `string_function`은 스트링 parameter `s`를 입력받아, 입력받은 문자열에 `world` 문자열을 덧붙이는 기능을 하는 함수이다. ("world" 앞에 스페이스는 없다. ) 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
String concatenation utilizes the `+` symbol:
```python
print "Hello" + "world"
# outputs "Helloworld"
```

**설명:**     
`+` 연산자를 사용하여 문자를 이어 붙여라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = "Hello"
# Your function here!
def string_function(s):
	return s + 'world'

print string_function(n)
```

**설명:**     
입력받은 `s = "Hello"` 에다가 "world"를 붙인다. 
{: .notice--info}



**결과** 
``` 
Helloworld
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 8. Passing a list to a function    

You pass a list to a function the same way you pass any other argument to a function.



**설명:**    
함수에 리스트를 전달하는 연습을 해보자. 함수에 여러개의 인수를 전달할 수 있듯이, 함수에 리스트도 전달 할수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Click Run to see that using a list as an argument in a function is essentially the same as using just a number or string!


**설명:**     
① Run을 클릭하여 소스를 실행시켜 보자. 함수에 리스르를 넘겼더니, 다시 리스트를 반환하는 것이다.  
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
def list_function(x):
    return x

n = [3, 5, 7]
print list_function(n)
```

**설명:**     
함수 `list_function(n)`에 리스트 `n`을 넣어서 호출 하였더니, 해당 함수가 입력받은 `x`를 그대로 반환했다. 리스트를 입력하고, 리스트를 반환하는 소스이다.  
{: .notice--info}



**결과** 
``` 
[3, 5, 7]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 9. Using an element from a list in a function    

Passing a list to a function will store it in the argument (just like with a string or a number!)
```python
def first_item(items):
  print items[0]

numbers = [2, 7, 9]
first_item(numbers)
```
In the example above, we define a function called `first_item`. It has **one argument** called `items`.
Inside the function, we print out the item stored at **index zero of items.**
After the function, we create a new list called `numbers`.
Finally, we call the `first_item` function with `numbers` as its argument, which prints out 2.




**설명:**     
함수 `first_item(numbers)`를 호출하면, 리스트 `numbers =[2,7,9]`가 넘겨지고,
이미 정의되어진 함수 `first_item()`는 인자 `numbers`에 `[2, 7, 9]`가 들어가 있다. 리스트 `items[0]` 첫번째 인자 값은 `2`가 출력된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Change line 2 so that `list_function` returns only the item stored in index **one of x**, rather than the entire x list.


**설명:**     
① 함수 `list_function(x)`의 기능을 다음과 같이 변경 하라. 입력 받은 `x`의 1번 index의 값을 출력하는 기능으로 바꿔라.   
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
def list_function(x):
  return x[1]

n = [3, 5, 7]
print list_function(n) 

```

**설명:**     
입력값 `n=[3,5,7]`중 1번 index 값만 출력하는 (ex. `x[1]`) 함수이다. 
{: .notice--info}



**결과** 
``` 
5
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 10. Modifying an element of a list in a function   

Modifying an element in a list in a function is the same as if you were just modifying an element of a list outside a function.

```python
def double_first(n):
  n[0] = n[0] * 2

numbers = [1, 2, 3, 4]
double_first(numbers)
print numbers
```
We create a list called `numbers`.
We use the `double_first` function to modify that list.
Finally, we print out [2, 2, 3, 4]
When we pass a list to a function and modify that list, like in the double_first function above, we end up modifying the original list.



**설명:**     
함수를 이용하여 리스트의 특정 값을 변경 할수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Change list_function to:

* Add 3 to the item at index 1 of the list.
* Store the result back into index 1.
* Return the list.


**설명:**     
① 함수 `list_function`을 수정하라.    
  • 입력 받은 리스트 x의 index 1번 값에 3을 더하라.
  • 그 결과 값을 리스트 x의 index 1번 값에 저장하라.     
  • 리스트 x를 반환하라.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Add 3 to x[1]'s value and store result
```python
x[1] = x[1] + 3
```

**설명:**     
결과값(x[1] + 3)을 x[1]에 저장하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def list_function(x):
  x[1] = x[1] + 3
  return x

n = [3, 5, 7]
print list_function(n)
```

**설명:**     
입력받은 리스트 `x`의 1번 index에 `3`을 더하고, 그 결과 값을 다시 `x[1]`에 저장한후 반환한다.
{: .notice--info}



**결과** 
``` 
[3, 8, 7]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 11. List manipulation in functions    

You can also **append or delete** items of a list inside a function just as if you were manipulating the list outside a function.
```python
my_list = [1, 2, 3]
my_list.append(4)
print my_list
# prints [1, 2, 3, 4]
```
The example above is just a reminder of how to append items to a list.

 



**설명:**     
함수를 통하여 리스트를 추가, 삭제 하는 등 조작해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function called `list_extender` that has **one parameter** `lst`.

* Inside the function, append the number 9 to lst.

* Then return the modified list.


**설명:**     
① 함수 `list_extender()`는 `lst`라는 파라미터를 하나 가진다.   
  • 입력받은 리스트 `lst`에 숫자 9를 추가하라.     
  • 변경된 리스트 `lst`를 반환하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Check `.append()` learned before chapter


**설명:**     
앞자에서 배운 `.append()`를 확인해 보자. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = [3, 5, 7]
# Add your function here
def list_extender(lst):
  lst.append(9)
  return lst


print list_extender(n)
```

**설명:**     
리스트에 값을 추구하는 것은 `lst.append(9)` 이다. 
{: .notice--info}



**결과** 
``` 
[3, 5, 7, 9]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 12. Printing out a list item by item in a function    

This exercise will go over how to utilize every element in a list in a function. You can use the existing code to complete the exercise and see how running this operation inside a function isn't much different from running this operation outside a function.

Don't worry about the range function quite yet—we'll explain it later in this section.





**설명:**     
함수를 사용하여 리스트의 값들을 활용하는 방법을 배워보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function called `print_list` that has one argument called `x`.

* Inside that function, print out each element one by one. Use the existing code as a scaffold.

* Then call your function with the argument n.


**설명:**     
① 함수 `print_list(x)` 를 정의하자.    
  • 함수 내부 기능으론, 리스트의 항목을 하나씩 출력하는 것이다. 기존의 코드를 발판으로 활용하세요.    
  • argument `n`을 가진 함수를 호출 하세요. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can simply place the code on lines 3 - 4 inside a function definition. Make sure to indent properly! And you'll have to change the `n` to `x`


**설명:**     
for 문의 argument `n`값을 `x`으로 바꿔 주시오. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = [3, 5, 7]

def print_list(x):
  for i in range(0, len(x)):
    print x[i]
    
print_list(n)
```

**설명:**     
함수 `print_list(x)`는 리스트를 입력 받안 해당 항목들을 하나씩 출력해주는 기능을 한다. 
{: .notice--info}



**결과** 
``` 
3
5
7
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 13. Modifying each element in a list in a function    

This exercise shows how to **modify each element in a list**. It is useful to do so in a function as you can easily put in a list of any length and get the same functionality. As you can see, **len(n)** is the length of the list.





**설명:**     
리스트의 각 항목들을 수정하는 것을 연습해 보자.     
**len(n)**함수를 이용하여 리스트의 길이를 알수 있다.    
어떤 길이의 리스트도 함수를 통하여 쉽게 조작할 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a function called **`double_list`** that takes a single argument **`x`** (which will be a list) and **multiplies each element by 2** and **returns that list**. Use the existing code as a scaffold.


**설명:**     
① 함수 **`double_list`**를 만들고, 이 함수는 argument **` x`**를 가진다. 그리고 이 함수는 리스트의 각 항목의 값에다 **`x 2`**를 한 결과 값을 반환한다. 작성되어진 코드를 활용하여 작성하라.     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can place the code on lines 3 - 5 inside a function definition. You will need to change the n[i]s in the for loop to x[i]. Make sure to indent properly!


**설명:**     
3~5라인 사이에서 함수를 정의하라. for 문 안에 있는 **`n[1]`**를 **`x[1]`**로 바꿔야 한다.
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = [3, 5, 7]

def double_list(x):
  for i in range(0, len(x)):
    x[i] = x[i] * 2
  return x
# Don't forget to return your new list!

print double_list(n)
```

**설명:**     
리스트 **`n`**을 argument **`x`**로 넘겨 받은 함수 **`double_list(x)`**는 각 항목의 값에다 **`X 2`** 한 값을 반환한다. 
{: .notice--info}


**결과** 
``` 
[6, 10, 14]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 14. Passing a range into a function    

Okay! Range time. The Python **`range()`** function is just a shortcut for **generating a list**, so you can use ranges in all the same places you can use lists.
```python
range(6) # => [0, 1, 2, 3, 4, 5]
range(1, 6) # => [1, 2, 3, 4, 5]
range(1, 6, 3) # => [1, 4]
```
The range function has three different versions:
```python
range(stop)
range(start, stop)
range(start, stop, step)
```
In all cases, the **`range()`** function **returns a list** of numbers from **start up to (but not including) stop**. Each item increases by step.

**If omitted, start defaults to 0 and step defaults to 1.**





**설명:**     
내장 함수 **`range()`**는 1~3개의 arguments를 가질수 있다.    
• range(stop) : 예)range(6)는 index 6까지 리스트를 생성하는데, 6은 포함하지 않는다. # [0,1,2,3,4,5]   
• range(start, stop) : 예)range(1,6)는 index 1번 부터 6번까지 리스트 생성, 단, 6은 생성하지 않음 # [1,2,3,4,5]      
• range(start, stop, step) : 예)range(1,6,3)는 index 1번부터 6번까지 리스트를 생성, 단, 3칸씩 간격을 두고 생성 # [1, 4]    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** On line 6, **replace** the (____) with a **`range()`** that returns a list containing [0, 1, 2].


**설명:**     
① 6라인 **`(____)`**에 [0,1,2]가 출력되도록 **`range()`**함수를 사용하여 작성하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
range(3) # [0,1,2]
range(0,3) # [0,1,2]
range(0,3,1) # [0,1,2]
```

**설명:**         
**`range()`**를 사용하여 리스트 [0,1,2]를 만들어 내는 방법은 여러가지가 있다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def my_function(x):
  for i in range(0, len(x)):
    x[i] = x[i]
  return x

print my_function(range(3)) # Add your range between the parentheses!
```

**설명:**     
우리는 **`range(3)`**을 활용하여 리스트 [0,1,2]를 생성했다. 
{: .notice--info}


**결과** 
``` 
[0, 1, 2]
```



<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 15. Iterating over a list in a function    

Now that we've learned about **range**, we have **two ways of iterating through a list**.

Method 1 - **for** item in list:
```python
for item in list:
  print item
```  
Method 2 - **iterate through indexes**:
```python
for i in range(len(list)):
  print list[i]
```  
Method 1 is useful to loop through the list, but it's not possible to modify the list this way.

Method 2 uses indexes to loop through the list, making it possible to also modify the list if needed. Since we aren't modifying the list, feel free to use either one on this lesson!





**설명:**     
리스트를 자동으로 생성해주는 방법에는 2가지가 있다. **for**문을 활용하는 법과 **indexes**를 활용하는 법이다.     
첫번째는 리스트를 생성할수는 있으나, 변경은 불가능하다.     
두번째는 리스트를 생성하고, 변경도 가능하다.     
이 장에서는 리스트를 변경할 일이 없기에, 본인이 편한것을 선택하여 연습하면 된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a function that **returns the sum of a list of numbers**.

* On line 3, define a function called **`total`** that accepts **one argument** called **`numbers`**. It will be a **list**.
* Inside the function, create a variable called **`result`** and **set it to zero**.
* Using **one of the two methods** above, iterate through the numbers list. **For each number, add it to result**.
* Finally, **return result**.



**설명:**     
① 리스트안에 있는 숫자들의 값을 더하는 함수를 만드시오.    
• 3라인에서, 함수 **`total(numbers)`** 를 만드시오. **`numbers`**는 리스트이다.    
• 함수 안에서 변수 **`result`**를 만들고 기본 값으로 **0**으로 채우시오.    
• 위, 2가지 방법중 하나를 선택하여 리스트를 생성하고, 각 항목 값을 더하시오.   
• 최종적으로, **`result`**를 반환하시오. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
if use method2, you shoud careful **range()**
```python
for in range(0, len(numbers)):
```  


**설명:**    
방법 2를 사용할 경우, **`range()`** 함수를 사용할때, 리스트를 산출할 범위를 지정해 주어라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = [3, 5, 7]

def total(numbers):
  result = 0
  for i in range(0,len(numbers)):
    result += numbers[i]
  return result
```

**설명:**     
**`range(0, len(numbers))`**는 0번부터 입력된 `numbers`의 갯수만큼 리스트를 만드는 것이다. 
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
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 16. Using strings in lists in functions    

Now let's try working with **strings**!

```python
for item in list:
  print item

for i in range(len(list)):
  print list[i]
```  
The example above is just a reminder of the two methods for iterating over a list.





**설명:**     
리스트를 자동 생성하는 방법은 2가지가 있다는 것을 잊지 말자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a function that **concatenates strings**.

* Define a function called **`join_strings`** accepts an argument called **`words`**. It will be a **list**.
* Inside the function, create a variable called **`result`** and set it to **""**, an empty string.
* Iterate through the **`words`** list and concatenate each word to **`result`**.
* Finally, **return the result**.
Don't add spaces between the joined strings!




**설명:**     
① 문자열을 연결하는 함수를 만드시오.     
• 함수 **`join_strings(words)`**를 만드시오.    
• 함수 내부에 변수 **`result`**를 만들고, ""로 초기화 하시오.    
• 입력받은 **`words`**를 하나씩 꺼내어 변수 **`result`**에 연결하시오.    
• 마지막으로 **`result`**값을 반환 하시오.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
For example,
```python
join_strings("Hello", "there")
should return "Hellothere".
```

**설명:**      
두개의 문자열을 입력 받아서 연결하는 것이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = ["Michael", "Lieberman"]
# Add your function here

def join_strings(words):
  result = ""
  for word in words:
    result += word
  return result

# use method 2
#def join_string(words):
#  result = ""
#  for i in range(len(words)):
#    result = result + words[i]
#  return result

print join_strings(n)
```

**설명:**     
**`word`**에 두개의 문자가 들어 있고, 각 항목을 하나씩 추출하여 **`result`**에 더한후 반환한다. 
{: .notice--info}


**결과** 
``` 
MichaelLieberman
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 17. Using two lists as two arguments in a function    

Using **multiple lists** in a function is no different from just using multiple arguments in a function!

a = [1, 2, 3]
b = [4, 5, 6]
print a + b
# prints [1, 2, 3, 4, 5, 6]
The example above is just a reminder of how to concatenate two lists.





**설명:**     
두개의 리스트를 argument로 넘기는 방법을 연습해 보자.     
상기 2개의 리스트를 합치는 방법은 이미 공부한바 있다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a function that **joins two lists together**.

On line 5, define a function called **`join_lists`** that has **two arguments**, **`x`** and **`y`**. They will both be **lists**.
Inside that function, **return the result** of concatenating **`x`** and **`y`** together.



**설명:**     
① 두개의 리스트를 합치는 함수를 만드시오.    
• 함수 **`join_lists(x, y)`** 만드시오. arguments 는 리스트 이다.    
• 함수 내부에서 **`x`, `y`**를 연결하여 결과 값을 반환하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can just use **`+`** to concatenate two lists. (You don't want to use append, because this just adds the entire second list as a single object at the end of the first.)


**설명:**     
**`+`**를 사용하여 리스트를 연결하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
m = [1, 2, 3]
n = [4, 5, 6]

# Add your code here!

def join_lists(x, y):
	return x + y


print join_lists(m, n)
# You want this to print [1, 2, 3, 4, 5, 6]
```

**설명:**     
**`+`** 연산자를 활용하여 두개의 리스느를 합친다. 
{: .notice--info}


**결과** 
``` 
[1, 2, 3, 4, 5, 6]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 18. Using a list of lists in a function    

Finally, this exercise shows how to make use of a single list that contains multiple lists and how to use them in a function.
```python
list_of_lists = [[1, 2, 3], [4, 5, 6]]

for lst in list_of_lists:
  for item in lst:
    print item

```    
In the example above, we first create a list containing two items, each of which is a list of numbers.
Then, we iterate through our outer list.
For each of the two inner lists (as lst), we iterate through the numbers (as item) and print them out.
We end up printing out:

1
2
3
4
5
6




**설명:**    
하나의 리스트에 여러개의 리스트가 값으로 들어가 있는 리스트를 어떻게 활용하는지를 배워 보자.    
하나의 리스트안에 또다시 2개의 리스트가 항목 값으로 들어가 있다. 이를 다시 각 값으로 봅아내는 함수이다. 
for 문 2개를 활용하여 사용한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a function called **`flatten`** that takes a **single list** and **concatenates** all the **sublists** that are part of it into a single list.

* On line 3, define a function called **`flatten`** with one argument called **`lists`**.
* Make a new, empty list called **`results`**.
* Iterate through lists. Call the looping variable numbers.
* Iterate through numbers.
* For each number, **`.append()`** it to **`results`**.
* Finally, return results from your function.



**설명:**     
① 함수 **`flatten(lists)`** 은 여러개 리스트를 포함한 싱글 리스트를 하나의 싱글 리스트를 가지는 리스트로 만드는 함수를 만드시오.    
• 3라인에서, 함수 **`flatten(lists)`**를 만드시오.    
• **`results`** 리스트를 만들고 초기화 하시오.    
• 입력 받은 리스트를 iterate 하면서 리스트의 각 값을 뽑아 내시오.    
• **`.append()`**함수를 사용하여 결과 값을 **`results`** 변수에 추가하시오.    
• 최종적으로 결과값 **`results`**를 반환하시오.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

For instance, it should turn
```python
[[1, 2, 3], [4, 5, 6]]
into

[1, 2, 3, 4, 5, 6]
```
**results is list**

**설명:**     
**`[[1,2,3], [4,5,6]]`**을 **`[1,2,3,4,5,6]`**으로 변경하시오.     
**`results`** 는 리스트다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = [[1, 2, 3], [4, 5, 6, 7, 8, 9]]
# Add your function here

def flatten(lists):
  results = []
  for numbers in lists:
    for number in numbers:
      results.append(number)
  return results

# use method 2
# def flatten(lists):
#   results = []
  
#   for i in range(0, len(lists)):
#     for j in range(0, len(lists[i])):
#       results.append(lists[i][j])
#   return results


print flatten(n)
```

**설명:**     
만약, 방법2 range()를 사용할 경우 인덱스 주소와 값을 혼동하지 말지. 
{: .notice--info}


**결과** 
``` 
[1, 2, 3, 4, 5, 6, 7, 8, 9]
```

<br>
<br>    
<br>    