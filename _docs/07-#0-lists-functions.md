---
# layout : rchive
title: "Lists and Functions"
permalink: /lists-functions/
excerpt: "We learn about lists and functions."
# last_modified_at: 2019-02-18T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---



<hr style="border: solid 1px #dddddd ;">    

LESSON    

Now that you've learned about lists, let's turbo-charge them with functions.    

**설명:** [ 학습방향 ]     
지금까지 리스트에 관한 것들을 배웠고, 지금부터 리스트와 함수를 강화해 보자.
{: .notice--info}     
     

    
    
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 1. List accessing    

This exercise goes over just pulling information from a list, which we've covered in a previous section! 



**설명:** [ Learn ]        
• Ch1. List accessing 에서는 리스트 항목에 접근하는 방법을 학습한다.    
• 우리는 앞장에서 이미 이와 관련하여 해보았다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Please add the code to print out the second element in the list.


**설명:** [ Instruction ]    
• 리스트 n 의 두번째 항목을 출력하라
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember that elements in a list start from index 0 and they are accessed in the form    

```python
x[n]
```    

* where `x` is the name of the list and n is the index in that list that you're trying to access.


**설명:** [ Hint ]    
• 리스트의 인덱스는 0 부터 시작한다.    
• 첫번째 항목값에 접근 하려면 n[0] 으로 접근한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = [1, 3, 5]

# Add your code below
print n[1]
```

**설명:** [ Solution ]          
• 리스트 n 의 항목값 3 에 접근할려면, n[1] 로 접근해야 한다.     
• 접근한 후 n[1] 의 항목값 3을 출력한다.
{: .notice--info}


**결과** 
``` 
3
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 2. List element modification     

You've already learned how to modify elements of a list in a previous section. This exercise is just a recap of that! 



**설명:** [ Learn ]          
• Ch2. List element modification 에서는 리스트의 항목값을 변경하는것을 학습한다.    
• 앞장 리스트에서 배웠지만 다시 한번 연습해 보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On line 3, multiply the second element of the `n` list by `5`

* Overwrite the second element with that result.

* Make sure to print the list when you are done!


**설명:** [ Instruction ]          
• 3 라인에서, 두번째 항목값 3 에 5를 곱한 값(e.g. 3 x 5 )으로 변경하라.    
• 변경 작업이 완료되면 해당 항목을 출력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* An item in a list in Python can be set to a value using the form

<p style="page-break-before: always;"></p>
<br>

```python
x[n] = v
```    

* where `x` is the name of the list, `n` is the index in the array and `v` is the value you want to set.


**설명:** [ Learn ]     
• 리스트의 특정 자리 항목을 변경하기 위해서는 다음과 같이 변경한다.    
• e.g. x[n]=v     
• x : 리스트,    
• n : index,    
• v : 값
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

**설명:** [ Solution ]          
• 인덱스 1번(두번째값) 자리 n[1] 에 값 5를 곱한다. (e.g. n[1] * 5)    
• 리스트 n 을 출력한다.    
• 출력 결과를 보면, 2번째 항목(n[1])만 곱하기 5를 한 결과값 15로 변경된다.
{: .notice--info}


**결과** 
``` 
[1, 15, 5]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 3. Appending to a list    

Here, we'll quickly recap how to `.append()` elements to the end of a list.



**설명:** [ Learn ]          
• Ch3. Appending to a list 에서는 메서드 .append()를 사용하는 법을 학습한다.    
• 리스트에  .append() 를 이용하면, 리스트 제일 마지막에 값을 추가할 수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Append the number 4 to the end of the list `n`.


**설명:** [ Instruction ]          
• 리스트 n 마지막 자리에 정수 4 를 추가하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* The function to append to the end of a list is    

```python
x.append(item)
```    
<p style="page-break-before: always;"></p>
<br>

* where `x` is the name of the list and item is the object you want to append.


**설명:** [ Hint ]          
• 리스트 x 에 .append(item) 를 활용한다.
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

**설명:** [ Solution ]          
• e.g. n.append(4) 는 리스트의 맨 끝에 값 4를 추가한다.
{: .notice--info}



**결과** 
``` 
[1, 3, 5, 4]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 4. Removing elements from lists    

This exercise will expand on ways to remove items from a list. You actually have a few options. For a list called `n`:

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

**설명:** [ Learn ]          
• Ch4. Removing elements from lists 에서는 리스트의 항목값 삭제를 학습한다.    
• 리스트의 항목값을 삭제 하는 것을 다시 학습한다.     
• n.pop(1), index 1번 주소의 값이 삭제 된다.    
• n.remove(1), 숫자 1의 값을 찾아서 해당 값 1이 삭제된다.    
• n.remove(1)에서 1이 여러개 있으면 첫번째 값 1만 삭제된다.             
{: .notice--info}    


`del(n[1])` is like `.pop` in that it will remove the item at the given index, but it won't return it:    

```python
del(n[1])
# Doesn't return anything
print n
# prints [1, 5]
```    
<p style="page-break-before: always;"></p>
<br>


**설명:** [ Learn ]          
• del(n[1]) index 값 1 위치에 해당하는 값이 삭제 된다.     
• 주의, del(n[1])은 결과값이 return 안된다.     
• e.g. print del(n[0]) 사용불가.    
• (사용불가 이유는 삭제한 결과값이 없기에 print 를 할수 없다.)
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Remove the first item from the list n using either `.pop()`, `.remove()`, or `del`.


**설명:** [ Instruction ]          
• 리스트 n 를 .pop(), .remove(), del() 중 하나를 사용하여 첫번째 값을 지워라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* One way of doing this would be    

```python
n.pop(0)
```     

* where `x` is the list and index is the item you want to pop off the list. If no index is given, it removes the last item from the list.



**설명:** [ Hint ]    
• n.pop(0) 은 index 0 위치의 값을 지운다.    
• 만약, index 값을 주지 않으면 마지막 인덱스를 지운다.( e.g. n.pop() )
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = [1, 3, 5]
# Remove the first item in the list here
n.pop(0)
print n
```

**설명:** [ Solution ]          
• 메서드 n.pop(0) 을 사용하여 첫번째 index 0 값을 지웠다.     
• 리스트 n 을 출력한다. 
{: .notice--info}



**결과** 
``` 
[3, 5]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 5. Changing the functionality of a function    

In this exercise, you will just be making a minor change to a function to change what that function does.



**설명:** [ Learn ]          
• Ch5. Changing the functionality of a function 에서는 함수 변경을 학습한다.    
• 함수를 조금 변경해 봄으로써, 함수 사용에 익슥해진다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Change the function so the given argument is multiplied by 3 and returned.


**설명:** [ Instruction ]          
• Editor 화면에 작성되어 있는 함수를 변경하라.    
• 이 함수는 입력값에 값 3 을 곱한 결과값을 반환한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You'll want to change the `+` to a `*`.


**설명:** [ Hint ]          
• 연사자 ( + ) 를 ( * ) 로 변경하라. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
number = 5

def my_function(x):
    return x * 3

print my_function(number)
```

**설명:** [ Solution ]          
• 함수 my_function(x) 은 입력값 x 에 곱하기 3 을 한 결과를 반환한다.     
• 함수 my_function(number) 를 호출하여 출력한다.
{: .notice--info}



**결과** 
``` 
15
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 6. More than one argument    

This exercise will recap how to use more than one argument in a function.



**설명:** [ Learn ]     
• Ch6. More than one argument 에서는 1개 이상의 arguments 를 학습한다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function called `add_function` that has `2` parameters `x` and `y` and adds them together.


**설명:** [ Instruction ]          
• 함수 add_function(x, y) 를 정의하라.    
• 함수 add_function() 은 parameter 값으로 x 와 y 를 가진다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* A function is defined as follows:    

```python
def my_function(argument1, argument2, etc.):
  # Function body goes here
     return argument1 + argument2
```

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]          
• 함수는 다음과 같이 정의한다.    
• def my_function(argument1, argument2, etc.):
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

**설명:** [ Solution ]     
• 함수 add_function(x, y) 는 입력값 x 와 y 의 합을 반환(return)한다.    
• 함수 add_function(m, n) 을 입력한 후, 반환값을 출력한다.    
• 입력값 m = 5 , n = 13 이다.
{: .notice--info}



**결과** 
``` 
18
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 7. Strings in functions    

This is a basic recap on using strings in functions.



**설명:** [ Learn ]    
• Ch7. Strings in functions 에서는 함수에서 문자열 사용법을 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write a function called `string_function` that takes in a string argument `(s)` and then returns that argument concatenated with the word `'world'`. Don't add a space before world!


**설명:** [ Instruction ]          
• 함수 string_function(s) 를 작성하라.    
• 이 함수는 스트링형 parameter 값으로 s 를 가진다.    
• 입력받은 문자열 변수 s 에 문자열 *world* 를 덧붙이고 그 결과를 반환한다.    
• 문자열 *world* 앞에 스페이스는 없다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* String concatenation utilizes the `+` symbol:    

```python
print "Hello" + "world"
# outputs "Helloorld"
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]          
• 연산자 ( + ) 를 사용하여 문자를 이어 붙인다. 
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

**설명:** [ Solution ]          
• 변수 n = "Hello" 를 대입한다.    
• 함수 string_function(n) 을 호출한다.    
• 함수 string_function(s) 은 다음과 같이 동작한다.    
• 입력받은 변수 s 에 문자열 *world* 를 붙인다.    
• 그 결과( "Helloworld" )를 반환한다.
{: .notice--info}



**결과** 
``` 
Helloworld
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 8. Passing a list to a function    

You pass a list to a function the same way you pass any other argument to a function.



**설명:** [ Learn ]         
• Ch8. Passing a list to a function 에서는 함수에 리스트를 전달하는것을 학습한다.   
• 함수에 여러개의 인수를 전달할 수 있듯이, 함수에 리스트도 전달 할수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Click Run to see that using a list as an argument in a function is essentially the same as using just a number or string!


**설명:** [ Instruction ]    
• Run 을 클릭하여 소스를 실행시켜 보자.    
• 함수의 arguments 로 리스트를 사용하여 호출한다.    
• 리스트에는 숫자와 문자열을 사용한다.
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
def list_function(x):
    return x

n = [3, 5, 7]
print list_function(n)
```

**설명:** [ Solution ]          
• 함수 list_function(n) 을 호출하였다.    
• 함수의 입력값 리스트 n 은 숫자 3, 5, 7 을 가지고 있다.    
• 함수 list_function(x) 는 입력 받은 리스트를 그대로 반환(return) 한다.
{: .notice--info}



**결과** 
``` 
[3, 5, 7]
```    
<p style="page-break-before: always;"></p>
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

In the example above, we define a function called `first_item`. It has one argument called `items`.
Inside the function, we print out the item stored at index zero of items.
After the function, we create a new list called `numbers`.
Finally, we call the `first_item` function with `numbers` as its argument, which prints out 2.




**설명:** [ Learn ]          
• Ch9. Using an element from a list in a function 에서는 함수에 입력된 값을 관리하는 법을 학습한다.    
• 함수 first_item(numbers) 를 호출한다.    
• 입력값 리스트 numbers = [2, 7, 9] 가 입력된다.    
• 정의된 함수 first_item(numbers) 는, parameter 값으로 numbers 를 가진다.    
• numbers 에는 [2, 7, 9] 가 입력된다.    
• 함수 기능에서, 리스트 items[0]의 첫번째 index 값은 2 가 출력된다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Change line 2 so that `list_function` returns only the item stored in index one of x, rather than the entire x list.


**설명:** [ Instruction ]          
• 함수 list_function(x) 의 기능을 다음과 같이 변경하라.    
• 입력받은 x 의 1 번 index 값을 출력하는 기능으로 바꿔라.   
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
def list_function(x):
  return x[1]

n = [3, 5, 7]
print list_function(n) 

```

**설명:** [ Solution ]          
• 함수 list_function(n) 을 호출한다.    
• 입력값 리스트 n = [3,5,7] 이 입력된다.    
• 함수 list_function(x) 는 입력된 리스트 x 의 1 번 index 를 반환한다.    
• 함수 list_function(n) 의 결과값이 출력된다.    
• e.g. print list_function(n)
{: .notice--info}



**결과** 
``` 
5
```    
<p style="page-break-before: always;"></p>
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
<br>

We create a list called `numbers`.
We use the `double_first` function to modify that list.
Finally, we print out [2, 2, 3, 4]
When we pass a list to a function and modify that list, like in the double_first function above, we end up modifying the original list.

<br>

**설명:** [ Learn ]          
• Ch10. Modifying an element of a list in a function 에서는 함수를 이용하여 리스트의 특정 값을 변경하는것을 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Change list_function to:

  * Add 3 to the item at index 1 of the list.
  * Store the result back into index 1.
  * Return the list.

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]          
• 함수 list_function 을 수정하라.    
• 입력 받은 리스트 x 의 index 1번 값에 3을 더하라.    
• 그 결과 값을 리스트 x 의 index 1번 값에 저장하라.     
• 리스트 x 를 반환하라.
{: .notice--info}


<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Add 3 to x[1]'s value and store result    

```python
x[1] = x[1] + 3
```
<br>
**설명:** [ Hint ]          
• 결과값 ( x[1] + 3 )을 x[1] 에 저장한다. 
{: .notice--info}

<br>
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

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• 함수 list_funciton(n) 을 호출한다.    
• 입력값 리스트 n 은 [3, 5, 7] 이 입력된다.    
• 함수 list_function(x) 는 다음과 같이 동작한다.    
• 입력받은 리스트 x 의 1 번 index 에 값 3 을 더한다.    
• 그리고, 그 결과값을 x[1] 에 다시 저정한다.        
• 리스트 x 를 반환(return)한다.     
• 함수 list_function(n) 의 결과값을 출력한다.    
• e.g. print list_function(n)
{: .notice--info}



**결과** 
``` 
[3, 8, 7]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 11. List manipulation in functions    

You can also append or delete items of a list inside a function just as if you were manipulating the list outside a function.    

```python
my_list = [1, 2, 3]
my_list.append(4)
print my_list
# prints [1, 2, 3, 4]
```    

The example above is just a reminder of how to append items to a list.

 

**설명:** [ Learn ]    
• Ch11. List manipulation in functions 에서는 함수를 통하여 리스트를 추가, 삭제를 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function called `list_extender` that has one parameter `lst`.

* Inside the function, append the number 9 to lst.

* Then return the modified list.


**설명:** [ Instruction ]          
• 함수 list_extender() 는 parameter 로 lst 가진다. 그리고 기능은 다음과 같다.      
• 입력받은 리스트 lst 에 숫자 9 를 추가하라.     
• 변경된 리스트 lst 를 반환하라. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Check `.append()` learned before chapter


**설명:** [ Hint ]          
• 앞장에서 배운 메서드 .append() 를 사용한다.
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

**설명:** [ Solution ]          
• 함수 list_extender(n) 를 호출한다.    
• 입력값은 리스트 n = [3, 5, 7] 이다.    
• 정의된 함수 list_extender(lst) 는 다음과 같이 동작한다.    
• 입력받은 lst 에 메서드 lst.append(9) 사용하여 값 9 를 리스트에 추가한다.    
• 최종 리스트 lst 를 반환(return)한다.    
• 호출한 함수 lst_extender(n) 의 반환된 결과값을 출력한다.
{: .notice--info}



**결과** 
``` 
[3, 5, 7, 9]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 12. Printing out a list item by item in a function    

This exercise will go over how to utilize every element in a list in a function. You can use the existing code to complete the exercise and see how running this operation inside a function isn't much different from running this operation outside a function.

Don't worry about the range function quite yet—we'll explain it later in this section.





**설명:** [ Learn ]          
• Ch12. Printing out a list item by item in a function 에서는 함수 안에서 for 문을 사용하여 입력받은 리스트의 항목 값들을 활용하는 방법을 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function called `print_list` that has one argument called `x`.    
* Inside that function, print out each element one by one. Use the existing code as a scaffold.

* Then call your function with the argument `n`.


**설명:** [ Instruction ]          
• 함수 print_list(x) 를 정의하라.     
• 함수 print_list(x) 는 리스트 x 를 parameter 로 가진다.    
• 함수 내부 기능은, 리스트의 항목을 하나씩 출력한다.    
• Editor 화면에 있는 기존 코드를 변경하라.     
• argument n 을 가진 함수를 호출하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can simply place the code on lines 3 - 4 inside a function definition. Make sure to indent properly! And you'll have to change the `n` to `x`


**설명:** [ Hint ]          
• for 문의 argument n 값을 x 로 변경하라.
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

**설명:** [ Solution ]          
• 함수 print_list(n) 을 호출한다.    
• 입력값 n = [ 3, 5, 7] 이다.     
• 정의된 함수 print_list(x) 는 다음과 같이 동작한다.    
• 입력받은 리스트 x 의 함수 len(x) 으로 길이를 구한다.    
• 함수 range(0, len(x)) 를 호출하여, 리스트의 index 갯수를 구한다.    
• for 문으로 리스트의 항목의 index 값을 하나씩 추출하여 변수 i 에 저장한다.     
• 리스트 x 의 index 주소에 해당하는 항목을 출력한다.( e.g. print x[i] )
{: .notice--info}



**결과** 
``` 
3
5
7
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 13. Modifying each element in a list in a function    

This exercise shows how to modify each element in a list. It is useful to do so in a function as you can easily put in a list of any length and get the same functionality. As you can see, len(n) is the length of the list.





**설명:** [ Learn ]    
• Ch13. Modifying each element in a list in a function 에서는 리스트의 항목값을 수정하는 것은 학습한다.     
• 함수 len(n) 를 이용하여 어떤 리스트의 길이도 쉽게 알 수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a function called `double_list` that takes a single argument `x` (which will be a list) and multiplies each element by 2 and returns that list. Use the existing code as a scaffold.


**설명:** [ Instruction ]          
• 함수 double_list() 를 만들어라.    
• 이 함수는 argument  x 를 가진다.    
• 이 함수의 기능은 입력받은 리스트의 각 항목값에 값 2 를 곱한 결과를 반환한다.    
• Editor 화면에 미리 작성되어 있는 코드를 재활용하여 작성하라.     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)   
<p style="page-break-before: always;"></p>
<br>

* You can place the code on lines 3 - 5 inside a function definition.     
* You will need to change the `n[i]`s in the for loop to `x[i]`.    
* Make sure to indent properly!


**설명:** [ Hint ]          
• Editor 화면 3 ~ 5 라인 사이에서 함수를 정의하라.    
• for 문 안에 있는 n[i] 를 x[i] 로 변경하라.
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

**설명:** [ Solution ]          
• 함수 double_list(n) 을 호출한다.    
• 함수는 arguments 인 n = [3, 5, 7] 을 가진다.    
• 정의된 함수 double_list(x) 는 parameter 로 리스트 x 를 가진다.     
• 이 함수는 다음과 같은 기능을 가진다.    
• 입력받은 리스트 x 의 길이를 함수 len(x) 를 사용하여 계산한다.    
• 리스트 x 의 길이 만큼 index 값을 산출한다. (e.g. range(0, len(x)))    
• for 문에서 리스트 x 의 index 값을 하나씩 추출한다.    
• 추출한 값을 변수 i 에 저장한다.    
• 리스트 x 의 i 번째 항목값에 값 2 를 곱한다. (e.g. x[i] * 2)    
• 값 2 를 곱한 결과를, 다시 리스트 x[i] 에 저장한다.    
• 리스트 x 를 반환한다.    
• 함수 double_list(n) 을 호출하고 받은 결과값을 출력한다.
{: .notice--info}


**결과** 
``` 
[6, 10, 14]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 14. Passing a range into a function    

Okay! Range time. The Python `range()` function is just a shortcut for generating a list, so you can use ranges in all the same places you can use lists.    

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

In all cases, the `range()` function returns a list of numbers from start up to (but not including) stop. Each item increases by step.

If omitted, start defaults to 0 and step defaults to 1.




**설명:** [ Learn ]          
• Ch14. Passing a range into a function 에서는 내부 함수 range() 사용법을 학습한다.    
• 내부 함수 range() 는 1 ~ 3 개의 arguments 를 가진다.     
• ---------------------     
• Arguments (1)    
• 사용법 : range(stop)     
• 설명 : e.g. range(6) 는 index 6 번까지 리스트를 생성한다. (6은 미포함)    
• 결과 : [0,1,2,3,4,5]    
• ---------------------      
• Arguments (2)    
• 사용법 : range(start, stop)     
• 설명 : e.g. range(1, 6) 는 index 1 번 부터 6 번까지 리스트 생성. (6은 미포함)    
• 결과 : [1,2,3,4,5]    
• ---------------------      
• Arguments (3)    
• 사용법 : range(start, stop, step)     
• 설명 : e.g. range(1,6,3) 는 index 1 번 부터 6번까지 리스트 생성.(6은 미포함)    
• 결과 : [1,4]  (단, 3칸씩 간격을 두고 생성)   
• ---------------------      
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Python3 ]          
• python2 와 python3 에서 range() 의 차이는 리스트를 생성할때 차이가 있다.    
• 단순히 range(5) 는 python2 와 python3 는 차이가 없다.    
• 다만, python2 에서 변수 var_python2 = range(5) 를 넣으면,    
• 리스트 [0,1,2,3,4] 가 변수에 대입된다.       
• python3 에서 변수 var_python3 = range(5) 를 넣으면,     
• 리스트 [0,1,2,3,4] 가 아닌, range(0.5) 가 대입된다.    
• python3 에서 변수에 대입 할때는 다음과 같이 대입해야 한다.    
• e.g. var_python3 = list( range(5) )    
• 대입하는 값이 리스트임을 명확히 알려줘야 한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On line 6, replace the (____) with a `range()` that returns a list containing [0, 1, 2].


**설명:** [ Instruction ]          
• Editor 화면 6라인 ( ____ ) 에 [0, 1, 2] 가 출력 되게하라.    
• 내부 함수 range() 를 사용하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
range(3) # [0,1,2]
range(0,3) # [0,1,2]
range(0,3,1) # [0,1,2]
```

**설명:** [ Hint ]              
• 내부 함수 range() 를 사용하여 리스트 [0,1,2] 를 만들어 내는 방법은 여러 가지가 있다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
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

**설명:** [ Solution ]          
• 이 장에서는 range(3) 을 활용하여 리스트 [0, 1, 2] 를 생성했다. 
{: .notice--info}


**결과** 
``` 
[0, 1, 2]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 15. Iterating over a list in a function    

Now that we've learned about range, we have two ways of iterating through a list.

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




**설명:** [ Learn ]          
• Ch15. Iterating over a list in a function 에서는 리스트 자동 생성법을 학습한다.     
• 리스트를 자동으로 생성 해주는 방법에는 2 가지가 있다.    
• 1st Method : for 문을 활용. (리스트 생성: O,  변경: X)   
• 2nd Method : indexes 활용. (리스트 생성: O,  변경: O)    
• 본인이 편한것을 선택하여 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

* Create a function that returns the sum of a list of numbers.

* On line 3, define a function called `total` that accepts one argument called `numbers`. It will be a list.    

* Inside the function, create a variable called `result` and set it to zero.    

* Using one of the two methods above, iterate through the numbers list. For each number, add it to result.    

* Finally, return result.



**설명:** [ Instruction ]          
• 리스트안에 있는 숫자들의 값을 더하는 함수를 작성하라.    
• 라인 3 에서, 함수 total(numbers) 를 만들어라.    
• 함수 total(numbers) Parameter 는 리스트 numbers 이다.    
• 이 함수는 다음과 같은 기능을 한다.    
• 변수 result 를 만들고 기본 값으로 0 으로 초기화 하라.    
• 리스트 생성 방법 2가지 중 하나를 선택하여 리스트를 생성하라.    
• 리스트의 각 항목값을 변수 result 에 더하여라.      
• 마지막으로, 변수 result 를 반환(return)하라.
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* if use method2, you shoud careful range()    

```python
for in range(0, len(numbers)):
```  
<br>

**설명:** [ Hint ]         
• 내부 함수 range() 를 Method 2 방법으로 사용할때, 리스트의 산출할 범위를 지정해 주어라. 
{: .notice--info}

<br>
<hr/>

<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
n = [3, 5, 7]

def total(numbers):
  result = 0
  for i in range(0,len(numbers)):
    result += numbers[i]
  return result
```

**설명:** [ Solution ]          
• 함수 total(numbers) 는 입력값 리스트 numbers 값들의 합을 반환하는 함수이다.    
• 변수 result 를 초기화 한다.    
• for 문에서 다음과 같은 기능을 처리한다.    
• 입력값 리스트 numbers 의 길이를 구한다.    
• e.g. len(numbers)    
• 리스트 numbers 의 index 값을 산출한다.    
• e.g. range(0, len(numbers))    
• 변수 i 에 리스트 numbers 의 indext 값을 저장한다.    
• 리스트 numbers[i] 의 항목값을 변수 result 에 더해 준다.    
• for 문이 종료되어, 리스트의 모든 항목값이 더해진 결과를 반환(return)한다.
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
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 16. Using strings in lists in functions    

Now let's try working with strings!

```python
for item in list:
  print item

for i in range(len(list)):
  print list[i]
```  
The example above is just a reminder of the two methods for iterating over a list.





**설명:** [ Learn ]          
• Ch16. Using strings in lists in functions 에서는 리스트 항목값이 문자열인 리스트를 조작하는 방법을 학습한다.    
• 문자열 리스트를 조작하는 방법은 2 가지가 있다.    
• Method 01 : 입력된 리스트의 항목값을 직접 출력    
• e.g. for item in list:      
• Method 02 : 입력된 리스트의 항목값의 index 를 이용하여 출력( list[i] )
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a function that **concatenates strings**.

* Define a function called `join_strings` accepts an argument called `words`. It will be a **list**.
* Inside the function, create a variable called `result` and set it to **""**, an empty string.
* Iterate through the `words` list and concatenate each word to `result`.
* Finally, **return the result**.
Don't add spaces between the joined strings!

<p style="page-break-before: always;"></p>
<br>



**설명:** [ Instruction ]          
• 함수 join_strings(words) 를 작성하라.     
• 이 함수는 입력된 리스트의 문자열을 연결하는 기능을 가진다.     
• 함수 내부에 변수 result 를 만들고, ( "" )로 초기화 하라.    
• 입력받은 변수 words 에서 항목값을 하나씩 추출한다.    
• 변수 result 에 추출한 항목값을 연결하여 저장하라.    
• 마지막으로, 변수 result 값을 반환하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* For example,    

```python
join_strings("Hello", "there")
should return "Hellothere".
```

**설명:** [ Hint ]           
• 두개의 문자열을 입력 받아서 연결한다. 
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
```   
<p style="page-break-before: always;"></p>
<br>

```python
# use method 2
#def join_string(words):
#  result = ""
#  for i in range(len(words)):
#    result = result + words[i]
#  return result

print join_strings(n)
```

**설명:** [ Solution ]     
• 함수 join_string(words) 를 정의한다.    
• 이 함수는 다음과 같이 처리한다.    
• 입력값으로 words 를 받는다.    
• 변수 result 를 초기화 ( "" ) 한다.    
• for 문 안에서, 입력받은 words 의 항목값을 하나씩 추출한다.    
• 추출 받은 항목값을 변수 word 에 저장한다.    
• 변수 result 에 변수 word 를 저장한다.    
• for 문을 빠져나오면, 변수 result 를 반환한다.
{: .notice--info}


**결과** 
``` 
MichaelLieberman
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">LISTS AND FUNCTIONS</font> 
### 17. Using two lists as two arguments in a function    

Using **multiple lists** in a function is no different from just using multiple arguments in a function!    
```python
a = [1, 2, 3]
b = [4, 5, 6]
print a + b
# prints [1, 2, 3, 4, 5, 6]     
```
The example above is just a reminder of how to concatenate two lists.



**설명:** [ Learn ]          
• Ch17. Using two lists as two arguments in a function 에서는 2 개의 리스트를 사용하는 방법을 학습한다.     
• 2 개의 리스트를 합치는 방법은 이미 앞에서 배웠다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a function that **joins two lists together**.

* On line 5, define a function called `join_lists` that has **two arguments**, `x` and `y`. They will both be **lists**.
Inside that function, **return the result** of concatenating `x` and `y` together.



**설명:** [ Instruction ]          
• 함수 join_lists(x, y) 작성하라.    
• 함수 join_lists(x, y) 는 리스트인 2 개의 arguments 를 가진다.    
• 함수 내부에서 x, y 를 연결하여 결과 값을 반환하라. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can just use `+` to concatenate two lists. (You don't want to use append, because this just adds the entire second list as a single object at the end of the first.)


**설명:** [ Hint ]          
• ( + ) 를 사용하여 리스트를 연결한다.
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

**설명:** [ Solution ]          
• 함수 join_lists(m, n) 을 호출한다.    
• Arguments m = [ 1, 2, 3 ], n = [4, 5, 6] 이 입력된다.    
• 정의된 함수 join_lists(x, y) 는 parameter x, y 를 가진다.    
• 이 함수는 입력된 리스트 x, y 의 항목값을 연산자 ( + ) 를 사용하여 합친다.    
• 합친 결과를 반환(return) 한다. (e.g. return x + y )
{: .notice--info}


**결과** 
``` 
[1, 2, 3, 4, 5, 6]
```    
<p style="page-break-before: always;"></p>
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




**설명:** [ Learn ]         
• Ch18. Using a list of lists in a function 에서는 리스트 안에 리스트가 있는것을 학습한다.    
• 하나의 리스트 안에 또다시 2 개의 리스트가 항목 값으로 들어가 있다.    
• 이런 모양의 리스트를 추출하는 함수를 만든다.    
• for 문 2 개를 활용한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

* Create a function called `flatten` that takes a **single list** and **concatenates** all the **sublists** that are part of it into a single list.

* On line 3, define a function called `flatten` with one argument called `lists`.
* Make a new, empty list called `results`.
* Iterate through lists. Call the looping variable numbers.
* Iterate through numbers.
* For each number, `.append()` it to `results`.
* Finally, return results from your function.



**설명:** [ Instruction ]          
• 함수 flattern(listst) 는 복합 리스트를 싱글 리스트로 바꾸는 함수이다.     
• (e.g. [ a, [b,c], d ] )    
• Editor 화면 3 라인에서, 함수 flatten(lists) 를 만들어라.    
• 이 함수는 다음과 같은 기능을 한다.    
• 빈 리스트 results 만들고 초기화 하라.    
• 입력 받은 리스트를 iterate 하면서 리스트의 각 값을 뽑아내라.    
• 메서드 .append() 를 사용하여 결과 값을 리스트 results 에 추가하라.    
• 마지막으로, 결과값 results 를 반환(return)하라.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* For instance, it should turn    

```python
[[1, 2, 3], [4, 5, 6]]    

into    

[1, 2, 3, 4, 5, 6]
```
* `results` is list

**설명:** [ Hint ]          
• 리스트 [ [1,2,3], [4,5,6] ] 을 리스트 [1,2,3,4,5,6] 으로 변경한다.    
• 변수 results 는 리스트 변수이다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
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

**설명:** [ Solution ]          
• 함수 flatten(n) 을 호출한다.    
• Arguments n = [[1, 2, 3], [4, 5, 6, 7, 8, 9]] 이다.    
• 정의된 함수 flatten(lists) 는 다음과 같이 동작한다.    
• 입력받은 parameters 변수 lists 에는 변수 n 값이 들어있다.    
• 리스트 변수 results 를 초기화 환다. (e.g. results = [] )    
• for 문에서 lists 의 항목값을 변수 numbers 에 하나씩 추출하여 저장한다.    
• 이중 for 문에서 numbers 의 항목값을 변수 number 에 하나씩 추출하여 저장한다.    
• 빈 리스트 results 에 메서드 .append(number) 를 사용하여 추가한다.    
• for 문이 모두 끝나면 리스트 results 를 반환(return)한다.    
• 함수 flatten(n) 을 호출 후 반환된 결과값을 출력한다.    
• 만약) 방법2 range()를 사용할 경우 인덱스 주소와 값을 혼동하지 말것. 
{: .notice--info}


**결과** 
``` 
[1, 2, 3, 4, 5, 6, 7, 8, 9]
```
   