---
# layout : rchive
title: "A Day at the Supermarket"
permalink: /day-supermarket/
excerpt: "We learn about list, dictionary Syntax."
# last_modified_at: 2019-02-13T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---


<hr style="border: solid 1px #dddddd ;">    

LESSON    

Let's manage our own supermarket and buy some goods along the way!    

**설명:** [ 학습방향 ]     
수퍼마켓에서 물건 구입 및 계산하는 프로그램을 만들면서, 리스트와 딕셔너리의 기능을 학습하고, 연습한다.
{: .notice--info}     
     
     
    
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 1. BeFOR We Begin    

Before we begin our exercise, we should go over the Python **for** loop one more time. For now, we are only going to go over the **for** loop in terms of how it relates to **lists** and **dictionaries**. We'll explain more cool for loop uses in later courses.

**for** loops allow us to **iterate** through all of the elements in a list from the left-most (or zeroth element) to the right-most element. A sample loop would be structured as follows:    

```python
a = ["List", "of", "some", "sort"]
for x in a: 
  # Do something for every x
```     

This loop will run all of the code in the indented block under the `for x in a:` statement. The item in the **list** that is currently being evaluated will be `x`. So running the following:

```python
for item in [1, 3, 21]: 
  print item
```  
<p style="page-break-before: always;"></p>
<br>

would print **1**, then **3**, and then **21**. The variable between for and in can be set to any variable name (currently item), but you should be careful to **avoid using the word** list as a variable, since that's a **reserved word** (that is, it means something special) in the Python language.

 



**설명:** [ Learn ]    
• Ch1. BeFOR We Begin 에서는 for문에서 리스트를 활용하는 연습을 한다.    
• ( for x in a: )는 리스트 a 에 있는 값들을 하나씩 추출하여 변수 x 에 넣어준다.   
• Python 예약어를 변수로 사용하면 안된다.    
• e.g. for print in list: ( X )    
• 예약어 print 를 변수로 사용하면 안된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Use a for loop to print out all of the elements in the list names.


**설명:** [ Instruction ]         
• for 문을 사용하여, 리스트의 내용들을 하나씩 출력하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Look at the sample code in the instructions if you need help!


**설명:** [ Hint ]         
• 상단의 Learn 에서 설명한 소스 코드를 참조하라. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
names = ["Adam","Alex","Mariah","Martine","Columbus"]

for name in names:
  print name
```

**설명:** [ Solution ]         
• 리스트 names 에 있는 항목(값)을 하나씩 추출해서 변수 name 에 하나씩 넣어 준다.     
• 변수 name 을 출력한다.
{: .notice--info}


**결과** 
``` 
Adam
Alex
Mariah
Martine
Columbus
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 2. This is KEY!    

You can also use a **for** loop on a **dictionary** to loop through its **keys** with the following:

```python
# A simple dictionary
d = {"foo" : "bar"}

for key in d: 
  print d[key]  # prints "bar"
```  

Note that dictionaries are unordered, meaning that any time you loop through a dictionary, you will go through every key, but you are not guaranteed to get them in any particular order.





**설명:** [ Learn ]     
• Ch2. This is KEY! 에서는 for 문에서 딕셔너리를 활용하는 방법을 연습한다.       
• for 문으로 딕셔너리의 항목(값)을 추출할수 있다.     
• 딕셔너리를 for 문으로 추출할 때 모든 키를 추출한다.    
• 단, 주의 할점은  특정 순서로 키를 가져올 수는 없다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Use a for loop to go through the `webster` dictionary and print out all of the definitions.


**설명:** [ Instruction ]     
• 딕셔너리 webster 에서 for 문을 사용하여 딕셔너리 항목(값)을 출력하라. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* The definitions are the values associated with each key.    
* print webster["Aardvark"] will give you an output of "A star of a popular children's cartoon show."

* Since you can loop through every key, you should be able to get every value


**설명:** [ Hint ]     
• 딕셔너리는 key 값과 매치되는 value 가 있다.    
• 딕셔너리 webster 는 key 값을 지정하여 해당 value 를 가져올 수 있다.    
• e.g. print webster["Aardvark"]    
• 모든 key 값을 for 문을 반복하면서 key 에 해당하는 value 값을 가져올 수 있다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
webster = {
  "Aardvark" : "A star of a popular children's cartoon show.",
  "Baa" : "The sound a goat makes.",
  "Carpet": "Goes on the floor.",
  "Dab": "A small amount."
}

# Add your code below!
for word in webster:
  print webster[word]
```

**설명:** [ Solution ]          
• 변수 word 에 리스트 webster 의 key 값이 저장된다.    
• 해당 key 의 value 를 출력하기 위해서는 리스트 webster[word] 로 출력할 수 있다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**결과** 
``` 
A star of a popular children's cartoon show.
Goes on the floor.
A small amount.
The sound a goat makes.
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 3. Control Flow and Looping    

The blocks of code in a **for** loop can be as big or as small as they need to be.

While looping, you may want to perform different actions depending on the particular item in the list.    

```python
numbers = [1, 3, 4, 7]
for number in numbers: 
  if number > 6:
    print number
print "We printed 7."
```   

In the above example, we create a list with 4 numbers in it.
Then we loop through the numbers list and store each item in the list in the variable number.
On each loop, if number is greater than 6, we print it out.     
So, we print 7.
Finally, we print out a sentence.
Make sure to keep track of your indentation or you may get confused!

 



**설명:** [ Learn ]     
• Ch3. Control Flow and Looping 에서는 for문 안에서 if 문을 사용하는 것을 학습한다.    
• for 문의 코드블럭 영역에는 크다/작다 와 같이 비교할수 있는 if 문을 작성할 수 있다.    
• 위 예제에서 for 문으로 리스트의 항목(값)을 추출한다.    
• 그리고 for 문 영역 안에서 if 문으로 6보다 큰 경우만 출력하도록 한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Like step 2 above, loop through each item in the list called `a`.

* Like step 3 above, if the `number` is **even**, print it out. You can test if the `item % 2 == 0` to help you out.

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]          
• 리스트 a 에서 항목을 호출하여 변수 number 에 저장하라.     
• 변수 number 의 항목값이 짝수(item % 2 == 0)만 출력 되게하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* A `number` is even if it's evenly divisible by 2.     
* You can determine divisibility with the modulus operator: %.
* For example, to check if the value inside of the variable item is divisible by 10, you can do `item % 10 == 0`. This will evaluate to True if the `number` in item is evenly divisible by 10 (yielding a remainder of zero).




**설명:** [ Hint ]          
• 변수 number 가 2로 나누어 지면 짝수이다.    
• 연산자 ( % )를 이용하여 나누어 지는것을 확인할 수 있다.    
• e.g. ( item % 10 == 0 )은 10 으로 나눠서 나머지가 0 이 되는것 이라는 의미이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
a = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13]

for number in a:
  if number % 2 == 0:
    print number

```

**설명:** [ Solution ]          
• 리스트 a 의 값 중 짝수( number % 2 )인 경우만 출력한다.    
• for 문으로 리스트 a 의 값을 변수 number에 저장한다.    
• 변수 number 를 2 로 나누어 나머지가 0 이면 짝수이므로 출력한다.    
• 짝수가 아니면 다시 for 문에서 리스트의 다음 값을 number 에 저장후, 반복한다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>


**결과** 
``` 
0
2
4
6
8
10
12
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 4. Lists + Functions    

Functions can also take lists as inputs and perform various operations on those lists.    

```python
def count_small(numbers):
  total = 0
  for n in numbers:
    if n < 10:
      total = total + 1
  return total

lotto = [4, 8, 15, 16, 23, 42]
small = count_small(lotto)
print small
```    

* In the above example, we define a function `count_small` that has one parameter, numbers.
* We initialize a variable `total` that we can use in the for loop.
* For each item n in `numbers`, if n is less than 10, we increment `total`.
* After the for loop, we return `total`.
* After the function definition, we create an array of numbers called `lotto`.
* We call the `count_small` function, pass in `lotto`, and store the returned result in `small`.
* Finally, we print out the returned result, which is 2 since only 4 and 8 are less than 10.




**설명:** [ Learn ]    
• Ch4. Lists + Functions 에서는 함수 호출시 리스트값을 넘겨 처리하는것을 학습한다.    
• 함수도 리스트를 입력 값으로 사용할 수 있다.    
• 리스트 lotto 항목 중에서 10 보다 작은값의 갯수를 반환한다.    
• 소스는 다음과 같이 동작한다.     
• 함수 count_samll(numbers) 을 정의한다. parameter 로 numbers 를 가진다.    
• 10 보다 작은 값을 저장하고 반환할 변수 total 을 선언후 초기화 한다.    
• parameter 로 받은, 리스트 numbers 의 항목값 n 이 10 보다 작은지 비교한다.    
• 변수 n 값이 10 보다 작으면 변수 total 에 저장한다.    
• for 문이 종료되면 결과값 total 을 반환한다.    
• 리스트 lotto 의 값을 함수 count_samll(lotto) 을 호출한다.    
• 함수 count_small(lotto) 의 결과값을 변수 small 에 저장한다.    
• 변수 small 을 출력한다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write a function that counts how many times the string "fizz" appears in a list.    
* Write a function called `fizz_count` that takes a list `x` as input.    
* Create a variable `count` to hold the ongoing count. Initialize it to zero.    

* for each `item in x`:, if that item is equal to the string "fizz" then **increment** the count variable.    

* After the loop, please return the count variable.

* For example, fizz_count(["fizz","cat","fizz"]) should return 2.




**설명:** [ Instruction ]     
• 리스트의 값 중 문자열 *fizz* 의 갯수를 알려주는 함수를 작성하라.    
• 함수명은 fizz_count(x) 이다. parameter 는 x 값을 가진다.    
• 변수 count 를 초기화 하고, 이 변수는 fizz 의 갯수를 세어 저장하는 변수이다.    
• for 문을 사용하여, 입력받은 리스트 x 의 값을 추출하여, 변수 item 에 저장한다.    
• if 문으로 변수 item 이 문자열 *fizz* 인지를 비교한다.    
• 만일, 문자열 *fixx* 와 같으면, 변수 count 를 1 증가 시킨다.     
• for 문이 종료되고, 최종 증가된 변수 count 를 반환(return) 한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* We need to count how many times "fizz" appears in our list.     
* To do this, make a counter variable (for example, count) in your function.     
* The counter variable could initially be set to zero. After that, you can loop through the list that you take as input and increase count by one every time an item in the list is equal to the string "fizz".    
* At the end, don't forget to return the number of "fizz"s!


<p style="page-break-before: always;"></p>
<br>


**설명:** [ Hint ]          
• 리스트에 문자열 *fizz* 가 몇 개 있는지 계산한다.    
• 함수에서 카운터할때 사용할 변수 count 를 만든다.    
• 카운터 변수는 초기에 0 으로 설정해야 한다.     
• if 문을 사용하여 문자열 *fizz* 와 같은 입력값이 있으면 개수를 하나씩 늘린다.    
• 마지막으로, *fizz* 의 수를 반환하는 것을 잊지 말자. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Write your function below!
def fizz_count(x):
  count = 0
  for item in x:
    if item == "fizz":
      count = count + 1
  return count
```

**설명:** [ Solution ]          
• 리스트 x 의 값에 *fizz* 의 갯수를 세어주는 함수 fizz_count(x) 이다.   
• 함수 fizz_count(x) 는 다음과 같이 작동한다.    
• 변수 count 를 초기화 한다. 이 변수는 문자열 *fizz* 의 갯수를 저장한다.    
• 리스트 x 에서 항목을 하나씩 추출하여, 변수 item 에 저장한다.    
• 변수 item 이 문자열 *fizz* 와 같으면, 변수 count 값을 1 증가 시킨다.    
• 리스트 x 의 모든 값을 추출하여 비교한다. 그리고 계속 반복한다.    
• 최종 결과값 변수 count 를 반환(return) 한다. 
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
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 5. String Looping      

As we've mentioned, strings are like lists with characters as elements. You can loop through strings the same way you loop through lists! While we won't ask you to do that in this section, we've put an example in the editor of how looping through a string might work.



**설명:** [ Learn ]        
• Ch5. String Looping 에서는 문자열을 관리하는 방법을 학습한다.    
• 문자열은 문자들의 리스트 이다.     
• 그러므로, for 문을 통하여 문자 하나씩 추출 할수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Run the code to see string iteration in action!


**설명:** [ Instruction ]    
• 문자열을 반복적으로 문자 하나씩 출력하는 프로그램을 실행하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ Hint ]          
• 소스를 읽어보고, Run을 실행하라. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
for letter in "Codecademy":
  print letter
    
# Empty lines to make the output pretty
print
print

word = "Programming is fun!"

for letter in word:
  # Only print out the letter i
  if letter == "i":
    print letter
```

**설명:** [ Solution ]     
• 첫번째 for 문은 문자열 *Codecademy* 의 문자를 하나씩 출력하는 것이다.    
• 두번째 for 문은 문자열 *Programming is fun* 의 문자중 문자 *i* 만 출력한다.
{: .notice--info}



**결과** 
``` 
C
o
d
e
c
a
d
e
m
y


i
i
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 6. Your Own Store!   

Okay—on to the core of our project.

Congratulations! You are now the proud owner of your very own Codecademy brand supermarket.    

```python
animal_counts = {
  "ant": 3,
  "bear": 6,
  "crow": 2
}
```    

In the example above, we create a **new dictionary** called `animal_counts` with three entries. One of the entries has the key "ant" and the value 3.


**설명:** [ Learn ]    
• Ch6. Your Own Store! 에서는 딕셔너리 활용을 학습한다.    
• 딕셔너리 animal_counts 는 3개의 key / value 쌍을 가지고 있다.     
• "ant" : 3, "bear" : 6, "crow" : 2 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a new dictionary called `prices` using {} format like the example above.

* Put these values in your prices dictionary, in between the {}:    

```python
"banana": 4,
"apple": 2,
"orange": 1.5,
"pear": 3
```    
<p style="page-break-before: always;"></p>
<br>

* Yeah, this place is really expensive. (Your supermarket subsidizes the zoo from the last course.)    


**설명:** [ Instruction ]     
• 딕셔너리 prices 를 {} 를 사용하여 작성하라.     
• 딕셔너리 prices = { } 에 key / value 값들을 넣어라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* dictionary uses as `dic = { "aa":4, "bb":5 }`

**설명:** [ Hint ]          
• 딕셔너리는 다음 예제와 같이 사용한다.     
• e.g. dic = {"aa" : 4, "bb" : 5} 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
prices = {"banana": 4,"apple": 2,"orange": 1.5,"pear": 3}
```

**설명:** [ Solution ]          
• 딕셔너리 prices 는 4 개의 key / value 를 가진다.     
• "banana" : 4,  "apple" : 2,  "orange" : 1.5,  "pear" : 3
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
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 7. Investing in Stock      

Good work! As a store manager, you’re also in charge of keeping track of your stock/inventory.



**설명:** [ Learn ]          
• Ch7. Investing in Stock 에서는 딕셔너리 변경하는 방법을 학습한다.    
• 딕셔너리를 이용하여 재고(stock / inventory)를 정리하는 프로그램을 연습해 보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a `stock` dictionary with the values below.

```python
"banana": 6,
"apple": 0,
"orange": 32,
"pear": 15
```

**설명:** [ Instruction ]          
• 딕셔너리 stock 을 작성하라.     
• 딕셔너리 stock 의 항목값은 아래 내용을 넣어라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember to use curly braces to make a dictionary. Don't forget to separate each key/value pair with a comma!

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Hint ]          
• 딕셔너리를 만들때 ( {} ) 와, key / value 사이에 ( , ) 로 구분 하는것을 잊지말자.    
• e.g. ddd = { "apple" : 1, "banana" : 2}
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
prices = {"banana": 4,"apple": 2,"orange": 1.5,"pear": 3}

stock = {"banana": 6, "apple": 0, "orange": 32, "pear": 15}
```

**설명:** [ Solution ]          
• 재고 정보를 가지고 있는 딕셔너리 prices, stock 을 정의 하였다.
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
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 8. Keeping Track of the Produce    

Now that you have all of your product info, you should print out all of your inventory information.    

```python
once  = {'a': 1, 'b': 2}
twice = {'a': 2, 'b': 4}
for key in once:
  print "Once: %s" % once[key]
  print "Twice: %s" % twice[key]
```   

In the above example, we create two dictionaries, once and twice, that have the same keys.
Because we know that they have the same keys, we can loop through one dictionary and print values from both once and twice.




**설명:** [ Learn ]     
• Ch8. Keeping Track of the Produce 에서는 딕셔너리의 key / value 값을 활용하는 방법을 학습한다.         
• Key 이름은 딕셔너리 별로 관리된다.    
• 2개의 딕셔너리에서 key 이름이 같아도, 딕셔너리 이름이 다르면 다른 key 로 인식한다.    
• 딕셔너리별로 해당 키 값을 호출 하면, 해당 딕셔너리 key의 value 값이 반환된다.     
• e.g. once[key], twice[kye] , key 이름은 같지만, value 값은 다르다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Loop through each key in prices.

* Like the example above, for each key, print out the key along with its price and stock information.

* Print the answer in EXACTLY the following format:    
<p style="page-break-before: always;"></p>
<br>

```
apple
price: 2
stock: 0
```    
<br>

* Like the example above, because you know that the prices and stock dictionary have the same keys, you can access the stock dictionary while you are looping through prices.

* When you're printing, you can use the syntax from the example above.




**설명:** [ Instruction ]          
• 다음과 같이 출력 되도록 코드를 수정하라.     
{: .notice--info}

```
apple
price: 2 
stock: 0
```    
• 참고로, 위와같이 출력할려면, 딕셔너리 price, stock 의 각 key 값이 apple 이어야 한다.
{: .notice--info}



<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Reference above example !!


**설명:** [ Hint ]          
• 상단의 Learn 예제를 참조하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>


```python
prices = {"banana": 4,"apple": 2,"orange": 1.5,"pear": 3}

stock = {"banana": 6, "apple": 0, "orange": 32, "pear": 15}

for food in prices:
  print food
  print "price: %s" % prices[food]
  print "stock: %s" % stock[food]
```

**설명:** [ Solution ]    
• 딕셔너리 prices 의 key 를 기준으로 잡는다.    
• for 문을 돌면서 prices 의 key 값을 추출한다.    
• 딕셔너리 prices 의 key 값을 출력한다.    
• 딕셔너리 prices 의 key 의 value 를 출력한다.    
• e.g. print price: %s prices[food]    
• 딕셔너리 stock 의 key 의 value 를 출력한다.    
• e.g. print stock: %s stock[food]
{: .notice--info}



**결과** 
``` 
orange
price: 1.5
stock: 32
pear
price: 3
stock: 15
banana
price: 4
stock: 6
apple
price: 2
stock: 0
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 9. Something of Value   

For paperwork and accounting purposes, let's record the total value of your inventory. It's nice to know what we're worth! 



**설명:** [ Learn ]          
• Ch9. Something of Value 에서는 서로 다른 딕셔너리의 항목값을 계산하는 방법을 학습한다.    
• 이 장에서는 모든 물품의 재고와 가격을 정리하는 프로그램을 이해한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Let's determine how much money you would make if you sold all of your food.

  * Create a variable called `total` and set it to zero.
  * Loop through the `prices` dictionary.
  * For each key in `prices`, **multiply** the number in prices by the number in stock. Print that value into the console and then **add** it to `total`.
  * Finally, outside your loop, **print** `total`.



**설명:** [ Instruction ]          
• 가지고 있는 모든 물건을 판매했을 경우 전체 금액이 얼마인지 계산해 보자.    
• 변수 total 을 만들고, 0 으로 초기화 한다.    
• 딕셔너리 prices 를 for 문으로 순환하며 계산한다.       
• prices 와 stock 의 각 key 별 value 를 곱하여 항목별 전체 금액을 계산한다.     
• for 문이 끝나면 최종 total 값을 출력한다.   
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>

<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* The value of any given product is its number of items in stock multiplied by its price. For instance, the total cost for bananas would be 24 (a price of 4 multiplied by 6 bananas in stock).

* You should print the number all by itself—no need for any additional text!



**설명:** [ Hint ]          
• 변수 total 에 각 항목별 재고 갯수와 가격을 곱한 금액을 추가로 더한다.    
• e.g. 바나나의 전체 가격은 (개별 가격 : 4) x (제고 : 6) = 24 이다.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
prices = {"banana": 4,"apple": 2,"orange": 1.5,"pear": 3}

stock = {"banana": 6, "apple": 0, "orange": 32, "pear": 15}

total = 0
for food in prices:
  print prices[food] * stock[food]
  total = total + prices[food] * stock[food]
print total
```

**설명:** [ Solution ]          
• 변수 total 을 초기화 한다.     
• 딕셔너리 prices 를 for 문으로 순환하면서 prices 와 stock 의 value 를 추출한다.    
• 추출한 값을 변수 food 에 저장한다.    
• 딕셔너리 prices[food] 값과 stock[food] 값을 곱하여 출력한다.(제품별 전체 값)    
• 변수 total 에 먼저 출력한 제품별 전체값을 계산하여 더한다.    
• for 문이 완료되면, 전체 제품의 가격을 더한 변수 total 을 출력한다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>


**결과** 
``` 
48.0
45
24
0
117.0
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 10. Shopping at the Market    

Great work! Now we're going to take a step back from the management side and take a look through the eyes of the shopper.

In order for customers to order online, we are going to have to make a consumer interface. Don't worry: it's easier than it sounds!




**설명:** [ Learn ]          
• Ch10. Shopping at the Market 에서는 리스트 활용을 학습한다.    
• 온라인 구매자의 사용 프로그램을 만들어 보면서, 리스트의 활용법을 숙지하자.    
• 차근 차근히 진행하니 천천히 따라하면 된다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* First, make a list called `groceries` with the values "banana","orange", and "apple".    


**설명:** [ Instruction ]     
• 리스트 groceries 를 작성하라.    
• groceries 는 다음 값( "banana", "orange", apple" )을 가진다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember to use square brackets for a list: `[]`.

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]          
• 이 장은 리스트를 학습한다. 리스트 표현은 ( [] ) 을 사용한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
groceries = ["banana", "orange", "apple"]
```

**설명:** [ Solution ]          
• 리스트 groceries 를 만들어서, 항목("banana", "orange", "apple")을 대입한다. 
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
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 11. Making a Purchase    

Good! Now you're going to need to know **how much** you’re **paying** for all of the items on your grocery list.    

```python
def sum(numbers):
  total = 0
  for number in numbers:
    total += number
  return total

n = [1, 2, 5, 10, 13]
print sum(n)
```    

In the above example, we first define a function called `sum` with a parameter `numbers`.
We initialize the variable `total` which we will use as our running `sum`.
For each `number` in the list, we add that `number` to the running sum `total`.
At the end of the function, we return the running `sum`.
After the function, we create, `n`, a list of numbers.
Finally, we call the `sum(numbers)` function with the variable `n` and print the result.



**설명:** [ Learn ]     
• Ch11. Making a Purchase  에서는 함수에서 리스트의 활용법을 학습한다.    
• 함수 sum(numbers) 은 리스트 numbers를 입력 받는다.     
• 함수 sum(numbers) 은 리스트의 각 값을 더하여 최종 반환한다.    
• 함수 sum(n) 은 리스트 ( n=[1,2,5,10,13] )을 arguments 로 입력하여 호출한다.    
• 함수 sum(n) 의 결과값 을 출력한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    
<p style="page-break-before: always;"></p>
<br>

* Define a function `compute_bill` that takes one argument `food` as input.

* In the function, create a variable `total` with an initial value of zero.

* For each item in the `food` list, add the price of that item to `total`.

* Finally, return the `total`.

* Ignore whether or not the item you're billing for is in stock. Note that your function should work for any `food` list.

<br>


**설명:** [ Instruction ]    
• 함수 compute_bill(food) 을 작성하라.    
• 이 함수는 argument 로 food 를 입력 받는다.    
• 다음과 같이 구현하라.    
• 변수 total 을 만들고 0 으로 초기화 하라.     
• 입력 받은 리스트 food 의 항목을 하나씩 추출하여 변수 total 에 저장하라.    
• 최종 변수 total 값을 반환(return)하라.     
• 청구 대상 품목의 재고가 있는지 여부는 신경쓰지 마라.    
• 리스트에 있는것은 재고 목록에 있다는 전제하에 작성한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Only add the prices of the items !!


**설명:** [ Hint ]          
• 리스트의 항목별 가격만 더하는 것이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>

```python
shopping_list = ["banana", "orange", "apple"]

stock = {
  "banana": 6,
  "apple": 0,
  "orange": 32,
  "pear": 15
}
    
prices = {
  "banana": 4,
  "apple": 2,
  "orange": 1.5,
  "pear": 3
}

# Write your code below!
def compute_bill(food):
  total = 0
  for item in food:
    total = total + prices[item]
  return total

```

**설명:** [ Solution ]     
• 함수 compute_bill(food) 을 작성하였다.    
• 이 함수는 입력 받은 리스트 food 의 해당 항목의 가격을 찾는다.(e.g. "banana")   
• for 문에서, food 에서 찾은 "banana" 의 가격을 리스트 prices 에서 찾는다.    
• 전체 값을 저장하는 변수 total 에 "banana" 의 가격을 더하여 저장한다.    
• 최종 total 값을 반환(return) 한다. 
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
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 12. Stocking Out    

Now you need your `compute_bill` function to take the stock/inventory of a particular item into account when computing the cost.

Ultimately, if an item isn't in stock, then it shouldn't be included in the total. You can't buy or sell what you don't have!



**설명:** [ Learn ]    
• Ch12. Stocking Out 에서는 딕셔너리의 value를 조작하는 방법을 학습한다.     
• 함수 compute_bill() 을 통하여 쇼핑하는 프로그램을 만들었다.    
• 이 장에서는 재고가 없는 상품은 구매 할 수 없는 기능을 추가한다.    
• 재고가 없는 상품은 가격을 계산하면 안된다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Make the following changes to your `compute_bill` function:

* While you loop through each item of food, **only add the price** of the item to total if the item's **stock count** is greater than zero.

* if the item is in stock and after you add the price to the total, subtract one from the item's stock count.


**설명:** [ Instruction ]          
• 함수 compute_bill() 을 계산할때, 딕셔너리 stock 항목 중 재고가 있는 것만 계산한다.    
• 딕셔너리 stock 에 재고가 0 인것은 계산하면 안된다.    
• 만약, 상품이 재고가 있으면, 그 가격을 전체 total 에 추가한다.    
• 그리고, 해당 제품의 숫자를 1 개 감소 시켜야 한다.   
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>

<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* If you're buying a banana, check if it's in stock (larger than zero). If it's in stock, add the cost of a banana to your bill. Finally, decrement the stock of bananas by one!


**설명:** [ Hint ]         
• "banana" 는 재고가 존재하므로, 가격을 구할수 있다.    
• "apple" 은 재고가 0 이므로 함수에서 재고 유무를 점검해야 한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
shopping_list = ["banana", "orange", "apple"]

stock = {
  "banana": 6,
  "apple": 0,
  "orange": 32,
  "pear": 15
}
    
prices = {
  "banana": 4,
  "apple": 2,
  "orange": 1.5,
  "pear": 3
}

# Write your code below!
def compute_bill(food):
  total = 0
  for item in food:
    if stock[item] > 0:
      total += prices[item]
      stock[item] -= 1
  return total
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• 함수 compute_bill(food) 에서는 딕셔너리 stock[item] > 0 인 것들만 계산한다.    
• 딕셔너리 stock[item] 이 0 보다 크면, 그 가격을 변수 total 에 추가한다.    
• 그리고 stock[item] 의 갯수를 하나 줄여준다. 
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
<font size="3"  face="돋움">A DAY AT THE SUPERMARKET</font> 
### 13. Let's Check Out!    

Perfect! You've done a great job with lists and dictionaries in this project. You've practiced:

* Using for loops with lists and dictionaries
* Writing functions with loops, lists, and dictionaries
* Updating data in response to changes in the environment (for instance, decreasing the number of bananas in stock by 1 when you sell one).
Thanks for shopping at the Codecademy supermarket!





**설명:** [ Learn ]     
• Ch13. Let's Check Out! 에서는 지금까지 작성한 소스를 정리해 보자.    
• 리스트와 딕셔너리를 for 문에서 사용하는 방법을 배웠다.     
• 함수에서 리스트, 딕셕너리, for 문을 활용하는 방법을 배웠다.    
• 딕셔너리의 값을 추가, 삭제 하는 방법을 배웠다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Print your result and click Run to finish this course.


**설명:** [ Instruction ]      
• 지금까지 작성한 소스를 실행시켜 보아라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>


* skip


**설명:** [ Hint ]      
• skip
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
shopping_list = ["banana", "orange", "apple"]

stock = {
  "banana": 6,
  "apple": 0,
  "orange": 32,
  "pear": 15
}
    
prices = {
  "banana": 4,
  "apple": 2,
  "orange": 1.5,
  "pear": 3
}

# Write your code below!
def compute_bill(food):
  total = 0
  for item in food:
    if stock[item] > 0:
      total += prices[item]
      stock[item] -= 1
  return total

print (compute_bill(shopping_list))
```

**설명:** [ Solution ]     
• 함수 compute_bill(shopping_list) 을 호출하여 출력한다.     
• 함수는 재고 항목 딕셔너리 food 의 항목을 하나씩 읽어서 재고가 있는지 확인한다.    
• 재고가 있으면 (item > 0) 해당 물품의 가격을 딕셔너리 prices 에서 찾는다.    
• 변수 total 에 item 의 가격을 추가한다.    
• 물품의 전체 가격이 저장된 변수 total 을 반환(return)한다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**결과** 
``` 
5.5
```
