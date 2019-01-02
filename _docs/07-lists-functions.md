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



**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
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



**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
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
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
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
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
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
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
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
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
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
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
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
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
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
