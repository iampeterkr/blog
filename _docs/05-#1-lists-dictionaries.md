---
# layout : rchive
title: "Lists & Dictionaries"
permalink: /lists-dictionaries/
excerpt: "We learn about Lists and Dictonaries Syntax."
# last_modified_at: 2019-02-11T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---



<hr style="border: solid 1px #dddddd ;">    

LESSON    

Lists and dictionaries are powerful tools you can use to store, organize, and manipulate all kinds of information.

**설명:** [ 학습방향 ]           
이 장에서는 리스트와 딕셔너리를 학습한다.    
이들은 모든 종류의 데이타를 저장, 구성 및 조작 하는데 활용할 수 있는 강력한 도구이다.     
{: .notice--info}     
     
    
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 1. Introduction to Lists    

Lists are a datatype you can use to store a collection of different pieces of information as a sequence under a single variable name. (Datatypes you've already learned about include strings, numbers, and booleans.)

You can assign items to a list with an expression of the form

```python
list_name = [item_1, item_2]
```

with the items in between brackets. A list can also be empty: empty_list = [].

Lists are very similar to strings, but there are a few key differences 



**설명:** [ Learn ]      
• Ch1. Introduction to Lists 에서는 리스트를 학습한다.         
• 리스트는 각기 다른 형태의 데이타 타입을 모을 수 있다.    
• 사용법은 다음과 같다.    
• e.g. 리스트 변수명 = [ item_1 , item_2 ]        
• e.g. test_list = [ item_1 , item_2 ]    
• 빈 리스트는 다음과 같이 만든다.    
• e.g. test_list = []     
• 리스트는 문자열과 비슷 하다는것을 알게 된다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* The list `zoo_animals` has three items (check them out on line 1). Go ahead and add a fourth! Just enter the name of your favorite animal (as a "string") on line 1, after the final comma but before the closing ].


**설명:** [ Instruction ]     
• Editor 화면에 있는 리스트 zoo_animals 에는 3개의 값이 미리 들어가 있다.    
• 마지막에 4번째 항목에 자신이 좋아하는 동물 이름을 추가하라.    
• 주의) 동물 이름은 String 형으로 해야한다. 그리고, 리스트 마지막에 추가 해야한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

* Remember:

```python
list_name = ["item_0", "item_1", "item_2", "your_item"]
```
* If your favorite animals are already on the list, add an animal that's exciting, but inexpensive. (This is a poor zoo with very few animals.)    

**설명:** [ Hint ]             
• 리스트 목록에 자신이 좋아하는 동물이 이미 있는가?    
• 그렇다면, 두번째로 좋아하는 동물을 추가하라.     
• 주의) 리스트에 같은 문자열이 있어서는 안된다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>


```python
zoo_animals = ["pangolin", "cassowary", "sloth", "dog"];
# One animal is missing!

if len(zoo_animals) > 3:
  print "The first animal at the zoo is the " + zoo_animals[0]
  print "The second animal at the zoo is the " + zoo_animals[1]
  print "The third animal at the zoo is the " + zoo_animals[2]
  print "The fourth animal at the zoo is the " + zoo_animals[3]
```

**설명:** [ Solution ]                
• 리스트 zoo_animals 에 문자열 *dog* 을 추가하였다.    
• 리스트 zoo_animals 의 항목이 4개 이상이면, 리스트 zoo_aimals 의 값이 출력된다.
{: .notice--info}


**결과** 
``` 
The first animal at the zoo is the pangolin
The second animal at the zoo is the cassowary
The third animal at the zoo is the sloth
The fourth animal at the zoo is the dog
```   
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font>    

### 2. Access by Index    

You can access an individual item on the list by its index. An index is like an address that identifies the item's place in the list. The index appears directly after the list name, in between brackets, like this:    

```python
list_name[index]
```

List indices begin with 0, not 1! You access the first item in a list like this: list_name[0]. The second item in a list is at index 1: list_name[1]. Computer scientists love to start counting from zero.    


**설명:** [ Learn ]    
• Ch2. Access by Index 에서는 index를 통하여 리스트에 접근하는 방법을 학습한다.    
• 리스트는 각 항목별로 주소(index)가 배정되어 있다.    
• 주소(index)는 0 부터 시작한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write a statement that prints the result of adding the second and fourth items of the list. Make sure to access the list by index!    

```python
numbers = [5, 6, 7, 8]

print "Adding the numbers at indices 0 and 2..."
print numbers[0] + numbers[2]
print "Adding the numbers at indices 1 and 3..."
# Your code here!

```    
<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]             
• *# Your code here !* 밑에 다음 코드를 구현하라.    
• 리스트 numbers 의 2번째 항목(6)과 4번째 항목(8)을 더하여라.    
• 그리고 출력하라.
{: .notice--info}



<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

* Remember:

  1 List indices begin with 0, not 1.
  2 The second item will have an index of 1.
  3 The fourth item will have an index of 3.    

**설명:** [ Hint ]             
• 리스트의 주소(index)는 0 부터 시작한다.    
• 2번째 항목의 주소(index)는 1 이다.    
• 4번째 항목의 주소(index)는 3 이다.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
numbers = [5, 6, 7, 8]

print "Adding the numbers at indices 0 and 2..."
print numbers[0] + numbers[2]
print "Adding the numbers at indices 1 and 3..."
# Your code here!
print numbers[1] + numbers[3]

```

**설명:** [ Solution ]    
• 리스트 numbers[1]의 항목 값은 6 이다.      
• 리스트 numbers[3]의 항목 값은 8 이다.    
• 이 둘의 값을 더한 후, 그 결과 값을 출력하였다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>


**결과** 
```
Adding the numbers at indices 0 and 2...
12
Adding the numbers at indices 1 and 3...
14
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)   
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 

### 3. New Neighbors    

A list index behaves like any other variable name! It can be used to access as well as assign values.    

```python
zoo_animals = ["pangolin", "cassowary", "sloth", "tiger"]
# Last night our zoo's sloth brutally attacked 
# the poor tiger and ate it whole.

# The ferocious sloth has been replaced by a friendly hyena.
zoo_animals[2] = "hyena"

# What shall fill the void left by our dear departed tiger?
# Your code here!

```    

You saw how to access a list index like this:

```python
zoo_animals[0]
# Gets the value "pangolin"
```    

You can see how assignment works on line 5:

```python
zoo_animals[2] = "hyena"
# Changes "sloth" to "hyena"
``` 

**설명:** [ Learn ]     
• Ch3. New Neighbors 에서는 리스트 항목값을 주소(index)를 이용하여 변경하는것을 학습한다.    
• 리스트 zoo_animals 의 index 값을 지정하면 다음 예와 같다.    
• e.g. zoo_animals[0]        
• 리스트 zoo_animals[0] 의 항목값 *pangolin* 을 읽을 수 있다.    
• 리스트 zoo_animals[2] = "hyena" 로 대입하면, 원래 *sloth* 을 *hyena* 로 변경된다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write an assignment statement that will replace the item that currently holds the value `"tiger"` with another animal (as a string). It can be any animal you like.

**설명:** [ Instruction ]   
• 리스트 zoo_animals[3] = "tiger" 을 당신이 좋아하는 다른 동물로 바꾸어라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

* Remember:

  1. List indices begin with 0, not 1!
  2. The fourth item will have an index of 3.    


**설명:** [ Hint ]    
• 주소(index)는 0 부터 시작한다.     
• 4번째 항목값은 index 값이 3 이다.  
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>


```python
zoo_animals = ["pangolin", "cassowary", "sloth", "tiger"]
# Last night our zoo's sloth brutally attacked 
# the poor tiger and ate it whole.

# The ferocious sloth has been replaced by a friendly hyena.
zoo_animals[2] = "hyena"

# What shall fill the void left by our dear departed tiger?
# Your code here!
zoo_animals[3] = "lion"
```

**설명:** [ Solution ]     
• 리스트 zoo_animals[3] 의 항목값 *tiger* 를 *lion* 으로 변경했다.
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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font>     

### 4. Late Arrivals & List Length    

A list doesn't have to have a fixed length. You can add items to the end of a list any time you like!

```python
letters = ['a', 'b', 'c']
letters.append('d')
print len(letters)
print letters
```    

1. In the above example, we first create a list called `letters`.
2. Then, we add the string `'d'` to the end of the letters list.
3. Next, we print out 4, the length of the letters list.
4. Finally, we print out `['a', 'b', 'c', 'd']`.


**설명:** [ Learn ]    
• Ch4. Late Arrivals & List Length 에서는 리스트에 항목을 추가하는 방법을 학습한다.    
• 리스트 letters 를 만든다.    
• 리스트 letters 에 항목값으로  'a', 'b', 'c' 를 넣는다.    
• 문자열 'd' 를 메소드 .append()를 사용하여, 리스트 letters 의 마지막 위치에 추가한다.    
• 리스트 letters 의 길이를 내장 함수 len() 을 사용하여 계산후 출력한다.  
• 리스트 letters 의 전체 값을 출력한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On lines 5, 6, and 7, append three more items to the `suitcase` list, just like the second line of the example above. (Maybe bring a bathing suit?)

* Then, set `list_length` equal to the length of the suitcase list.

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]    
• Editor 화면 5, 6, 7 라인에서 리스트 suitcase 에 3개 이상의 항목값을 추가하라.    
• 리스트에 메소드 .append() 사용하라.    
• 변수 list_length 에 리스트 suitcase 의 길이를 함수 len()을 사용하여 저장하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

* That bit of `%` magic on line 11 is the string formatting we learned earlier.     
* The `%d` tells Python to expect an integer to insert instead of a string value (%s).    



**설명:** [ Hint ]    
• 앞에서 배운바와 같이 ( % ) 는 변수의 값을 대체하는 기호이다.    
• e.g. ( %d )는 숫자를 출력하기 위한 대체 표현이다.    
• e.g. ( %s )는 문자열을 출력하기 위한 대체 표현이다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
suitcase = [] 
suitcase.append("sunglasses")

# Your code here!
suitcase.append("shirt")
suitcase.append("pants")
suitcase.append("shoes")

list_length = len(suitcase) # Set this to the length of suitcase

print "There are %d items in the suitcase." % (list_length)
print suitcase
```

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Solution ]    
• 리스트 suitcase 에 .append() 메서드를 사용하여, 문자열 *shirt* 를 추가 하였다.    
• 리스트 suitcase 에 .append() 메서드를 사용하여, 문자열 *pants* 를 추가 하였다.    
• 리스트 suitcase 에 .append() 메서드를 사용하여, 문자열 *shoes* 를 추가 하였다.    
• 리스트 suitcase 의 길이를 len() 내장 함수를 사용하여 계산한다.    
• 변수 list_length 에 len(suitcase) 의 결과를 대입한다.    
• 변수 list_length 의 값을 ( %d ) 에 대체하여 출력한다.    
• 리스트 suitcase 를 출력한다.
{: .notice--info}



**결과** 
``` 
There are 4 items in the suitcase.
['sunglasses', 'shirt', 'pants', 'shoes']
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font>    

### 5. List Slicing    

Sometimes, you only want to access a portion of a list. Consider the following code:    

```python
letters = ['a', 'b', 'c', 'd', 'e']
slice = letters[1:3]
print slice
print letters
```   

What is this code doing?

**First**, we create a list called `letters`.

Then, we take a subsection of the list and store it in the slice list. We do this by defining the indices we want to include after the name of the list: `letters[1:3]`. In Python, when we specify a portion of a list in this manner, we include the element with the first index, 1, but we exclude the element with the second index, 3.

Next, we print out slice, which will print `['b','c']`. Remember, in Python indices always start at 0, so the 1 element is actually b.

Finally, we print out `['a', 'b', 'c', 'd', 'e']`, notice that we did not modify the original letters list.


**설명:** [ Learn ]     
• Ch5. List Slicing 에서는 문자열의 특정 범위를 잘라내는 방법을 학습한다.        
• 리스트 letters 의 특정 항목값 'b', 'c' 만 추출 하려면 어떻게 해야 할까?    
• 첫번째 방법은, 해당 문자열의 index 값을 지정해서 추출할 수 있다.    
• e.g. letters[1]        
• 이 장에서는 index 값의 범위를 지정하여 추출할 수 있다.    
• e.g. letters[1 : 3]            
• 리스트 letters[1 : 3]은 리스트 letters 1번 주소부터 3번 주소까지 잘라낸다는 의미이다.    
• 단, 잘라내는 규칙은 다음과 같다.     
• e.g. letters[Begin : End]        
• - Begin : 첫번째 index 포함.    
• - End :  마지막 index 미포함.    
• 리스트 index 는 0 부터 시작한다.    
• 리스트를 추출하여 출력하여도 해당 리스트의 원본은 변함이 없다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On line 7, create a list called `middle` containing only the two middle items from `suitcase`.

* On line 10, create a list called `last` made up only of the last two items from `suitcase`.


**설명:** [ Instruction ]             
• Editor 화면, 7번 라인에서, 리스트 middle 를 만들어라.    
• 리스트 middle 에는, 리스트 suitcase 의 중간 항목값 2개를 추출하여 저장하라.    
• 10 라인에서, 리스트 last 를 만들어라.    
• 리스트 last 에는, 리스트 suitcase 의 마지막 항목값 2개를 추출하여 저장하라.
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

* In order to slice the last two items from the list
`myList = [0,1,2,3,4]`, the ending index of your slice will be one beyond the actual last index of the list. Check it out:    
<br>
```python
myList[3:5]
# Returns [3, 4]    
```


**설명:** [ Hint ]             
• myList[3 : 5]는 myList[3]부터 myList[5] 까지 잘라낸다.    
• myList[3]은 포함된다. (항목값 : 3 )     
• myList[5]는 미포함된다. (myList[4] 항목값 : 4까지 잘라낸다.)   
• 즉, [0, 1, 2, 3, 4] 중  값 [3, 4] 만 잘라낸다.  
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
suitcase = ["sunglasses", "hat", "passport", "laptop", "suit", "shoes"]

# The first and second items (index zero and one)
first = suitcase[0:2]

# Third and fourth items (index two and three)
middle = suitcase[2:4]

# The last two items (index four and five)
last = suitcase[4:6]
```

**설명:** [ Solution ]     
• suitcase[2 : 4] 는 index 2, 3 인 *passport*, *laptop* 이 추출된다.    
• suitcase[4 : 6] 는 index 4, 5 인 *suit*, *shoes* 가 추출된다.
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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font>     

### 6. Slicing Lists and Strings    

You can slice a string exactly like a list! In fact, you can think of strings as lists of characters: each character is a sequential item in the list, starting from index 0.    

```python
my_list[:2]
# Grabs the first two items
my_list[3:]
# Grabs the fourth through last items
```   

If your list slice includes the very first or last item in a list (or a string), the index for that item doesn't have to be included.


**설명:** [ Learn ]   
• Ch6. Slicing Lists and Strings 에서는 문자열 Slicing 을 학습한다.    
• 문자열도 각 알파벳마다 index가 부여되어 있다.     
• 문자열도 각 index 값으로 잘라 낼수 있다.     
• my_list[ : 2] 는 처음부터 index 2번(미포함)까지 잘라낸다.(처음부터 2번째까지)    
• my_list[3 : ] 는 index 3번(포함)부터 끝까지 잘라낸다.(4번째 항목부터 끝까지)
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Assign to `dog` a slice of `animals` from index 3 up until but not including index 6.

* Assign to `frog` a slice of `animals` from index 6 until the end of the string.


**설명:** [ Instruction ]              
• 리스트 dog에 변수 animals 의 인덱스 3번(포함) ~ 6번(미포함)까지 잘라내서 저장하라.    
• 리스트 frog 에 animals 의 인덱스 6번(포함) 부터 끝까지 잘라내서 저장하라. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

* Remember: you don't need the first index if you're starting from the beginning of the string, and you don't need the second index if you're going all the way to the end!    


**설명:** [ Hint ]              
• 첫번째 index(1) 포함, 마지막 index(5) 미 포함    
• e.g. list[1 : 5]     
• 마지막 index( ) 를 적지 않으면 범위는 끝까지임    
• e.g. list[1 : ]
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
animals = "catdogfrog"

# The first three characters of animals
cat = animals[:3]

# The fourth through sixth characters
dog = animals[3:6]

# From the seventh character to the end
frog = animals[6:]
```

**설명:** [ Solution ]              
• animals[ : 3] 은 index 0(포함)부터 index 3(미포함)까지 잘라낸다.(e.g. 'cat')    
• animals[3 : 6] 은 index 3(포함)부터 index 6(미포함)까지 잘라낸다.(e.g. 'dog')    
• anmals[6 : ] 은 index 6(포함) 부터 끝까지 잘라낸다. (e.g. 'frog')
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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 

### 7. Maintaining Order    

Sometimes you need to search for an item in a list.    

```python
animals = ["ant", "bat", "cat"]
print animals.index("bat")
```    

* First, we create a list called `animals` with three strings.    

* Then, we print the first index that contains the string "bat", which will print 1.    

We can also insert items into a list.    

```python
animals.insert(1, "dog")
print animals
```    

* We insert "dog" at index 1, which moves everything down by 1.     

* We print out ["ant", "dog", "bat", "cat"]




**설명:** [ Learn ]     
• Ch7. Maintaining Order 에서는 리스트의 특정 index에 항목을 추가하는 방법을 학습한다.    
• 리스트 animals 에 3개의 문자열 *ant*, *bat*, *cat* 이 들어 있다.     
• 리스트 animals 의 index 1번 자리에 *dog* 를 추가하려면 다음과 같이 한다.    
• e.g. animals.insert(1, "dog")    
• 추가 하고자 하는 index 번호와 항목값을 지정해 준다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

* Use the `.index(item)` function to find the index of "duck".    
* Assign that result to a variable called `duck_index`.    
* Then `.insert(index, item)` the string "cobra" at that index.  


**설명:** [ Instruction ]              
• 리스트 animals 에서 *duck* 의 index 값을 찾아라.     
• 해당 항목의 index 값은 메서드 .index("duck") 를 사용하여 찾는다.    
• 항목값 *duck* 의 index 값을 변수 duck_index 에 저장하라.   
• 리스트 animals 의 문자열 *duck* 의 index 자리에 *cobra* 추가하라.    
• 메서드 .insert(index, item) 을 활용하여 추가하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

* You're not replacing "duck" with "cobra"—you're just finding "duck", then inserting "cobra".    



**설명:** [ Hint ]         
• (주의) *duck* 대신 *cobra* 항목 값으로 대체하는 것이 아니다.    
• 문자열 *duck* 의 index 값 자리에, *cobra* 를 넣는 것이다.    
• 즉, *duck* 자리에 *cobra*가 삽입 되는 것이다.    
• 정상적으로 완료되면 *duck*는 *cobra* 에 다음에 올 것이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
animals = ["aardvark", "badger", "duck", "emu", "fennec fox"]
duck_index = animals.index("duck")# Use index() to find "duck"

# Your code here!
animals.insert(duck_index,"cobra")

print animals # Observe what prints after the insert operation
```

**설명:** [ Solution ]          
• 리스트 animals 에서 *duck*의 index 값은 2 이다.    
• 변수 duck_index 에 *duck* 의 index 값 2가 저장된다.    
• index 2 번 자리에 문자열 *cobra*를 삽입한다.    
• e.g. animals.insert(duck_index, "cobra")    
• 변수 animals 를 출력한다.    
• 문자열 *duck* 의 index 값은 3 이 된다.     
• 문자열 *cobra* 의 index 값은 2 가 된다.
{: .notice--info}



**결과** 
``` 
['aardvark', 'badger', 'cobra', 'duck', 'emu', 'fennec fox']
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font>     

### 8. For One and All    

If you want to do something with every item in the list, you can use a for loop. If you've learned about for loops in JavaScript, pay close attention! They're different in Python.    

```python
for variable in list_name:
  # Do stuff!
```    

A `variable` name follows the `for` keyword; it will be assigned the value of each list item in turn.    

Then in `list_name` designates `list_name` as the list the loop will work on. The line ends with a colon `(:)` and the indented code that follows it will be executed once per item in the list.


**설명:** [ Learn ]    
• Ch8. For One and All 에서는 리스트의 값들을 추출하는것을 학습한다.    
• 리스트의 항목(값)들을 모두 뽑아 내려면 해당 index 값을 지정해 주면 된다.    
• for loop 문을 사용하여 리스트의 항목을 추출할 수 있다.    
• e.g. for variable in list_name:      
• 변수 variable 는 리스트 list_name 에서 뽑아낸 항목을 저장하는 변수이다.     
• for 문의 끝에는 ( : ) 이 있다.    
• for 문의 내용은 들여쓰기를 하여 작성한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write a statement in the indented part of the for-loop that prints a `number` equal to `2 * number` for every list item.


**설명:** [ Instruction ]     
• for 문을 사용하여 리스트 my_list 에서 추출한 값을 변수 number 에 저장하라.    
• 변수 number 값을 ( 2 x number ) 하여 출력하라. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

* Each list item is assigned to the user-defined variable `number` in turn. All you need to do is print two times number in the body of the loop (the indented part).

* The for loop will automatically execute your code as many times as there are items in my_list!    



**설명:** [ Hint ]         
• 변수 number 에 리스트 my_list 항목(값) 들이 하나씩 추출되어 자동으로 저장된다.    
• 변수 number 에 x 2 를 하여 출력한다.    
• 단, for 문을 쓰기 위해서는 들여 쓰기를 주의 해야한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
my_list = [1,9,3,8,5,7]

for number in my_list:
  # Your code here
  print (2 * number)
  
```    

**설명:** [ Solution ]         
• 리스트 my_list 의 값 [ 1, 9, 3, 8, 5, 7 ] 이 변수 number 에 자동 저장된다.    
• for 문을 반복적으로 돌면서, number x 2 계산된 값이 출력된다. 
{: .notice--info}



**결과** 
``` 
2
18
6
16
10
14
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font>     

### 9. More with 'for'    

If your list is a jumbled mess, you may need to `sort()` it.

```python
animals = ["cat", "ant", "bat"]
animals.sort()

for animal in animals:
  print animal
```   
  
* First, we create a list called `animals` with three strings. The strings are not in alphabetical order.     

* Then, we sort `animals` into alphabetical order. Note that `.sort()` modifies the list rather than returning a new list.    

* Then, for each item in `animals`, we print that item out as "ant", "bat", "cat" on their own line each.



**설명:** [ Learn ]         
• Ch9. More with 'for'  에서는 다양한 종류의 for 문을 학습한다.    
• 리스트 animals 에는 3개의 문자열이 알파벳 순서와 상관없이 뒤죽박죽 들어 있다.    
• 메서드 .sort() 를 사용하여, 리스트 animals 를 알파벳 오름차순으로 정렬한다.    
• 이후, 정렬된 리스트 animals 를 출력 한다.    
• 리스트 animals 의 각 항목(값)이, 알파벳 오름차순으로 정렬 되어 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write a for-loop that iterates over `start_list` and `.append()`s each number squared (x ** 2) to `square_list`.

<p style="page-break-before: always;"></p>
<br>

* Then sort `square_list`!


**설명:** [ Instruction ]         
• 리스트 start_list 에 리스트 square_list 의 항목값의 제곱을 저장하라.    
• 메서드 .append() 를 사용하라.    
• 리스트 square_list 를 sort 함수를 사용하여 정렬하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You will need to use:

  1. A for loop
  2. The .append() method
  3. The .sort() method

* Feel free to peek back at previous exercises in this section if you need to!


**설명:** [ Hint ]          
• for  문을 사용하라.    
• 메서드 .append() 를 사용하라.    
• 메서드 .sort() 를 사용하라.    
• 메서드 .append(), .sort() 사용법이 기억이 나지 않으면, 배운것을 다시 확인하라.
{: .notice--info}


<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
start_list = [5, 3, 1, 2, 4]
square_list = []

# Your code here!
for number in start_list:
  square_list.append(number ** 2)
square_list.sort()

print square_list
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• for 문에서, 리스트 start_list 의 각 항목값을 변수 number 에 저장한다.    
• 변수 number 를 메서드 .append()를 활용하여 제곱을 구한다.    
• 변수 number 제곱한 값을 리스트 square_list 에 저장한다.     
• 리스트 square_list 를 메서드 .sort() 를 사용하여 정렬한다.    
• 리스트 square_list 를 출력한다. 
{: .notice--info}



**결과** 
``` 
[1, 4, 9, 16, 25]
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font>    

### 10. This Next Part is Key    

A dictionary is similar to a list, but you access values by looking up a key instead of an index. A key can be any string or number. Dictionaries are enclosed in curly braces, like so:

```python
d = {'key1' : 1, 'key2' : 2, 'key3' : 3}
```

This is a dictionary called `d` with three key-value pairs. The key 'key1' points to the value 1, 'key2' to 2, and so on.

Dictionaries are great for things like phone books (pairing a name with a phone number), login pages (pairing an e-mail address with a username), and more!

 

**설명:** [ Learn ]      
• Ch10. This Next Part is Key 에서는 딕셔너리에 대하여 학습한다.    
• 딕셔너리는 리스트와 비슷하다.     
• 리스트는 눈에 보이지 않는 index를 가지고 해당 항목(값)을 나타낸다.    
• 딕셔너리는 key 를 이용하여 해당 항목(값)을 나타낸다.     
• e.g. 딕셔너리 d = {'key1' : 1, 'key2' : 2, 'key3' : 3}     
• 딕셔너리 항목(값)은 ( key : value ) 쌍으로 구성되어 있다.    
• 'key1' 을 키(key)라고 부르며, 이와 매칭되는 값 1 을 값(value)이라 부른다.    
• key 는 문자열, 숫자 모두 사용 가능하다.    
• key 와 value 는 한 쌍이다.    
• key 는 중복된 이름을 가질수 없다.       
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    


* Print the values stored under the `'Sloth'` and `'Burmese Python'` keys. Accessing dictionary values by key is just like accessing list values by index:    
<p style="page-break-before: always;"></p>
<br>

```python
residents['Puffin']# Gets the value 104
```

* Check the Hint if you need help!




**설명:** [ Instruction ]          
• 딕셔너리 residents 에서 key 값이 'Sloth' 인 것의 값(value)를 출력하라.    
• 딕셔너리 residents 에서 key 값이 'Python' 인 것의 값(value)를 출력하라.    
• 참고로, 리스트는 index 값을 지정하여 해당 값을 찾는다.     
• 하지만, 딕셔너리는 key 값을 지정하여 해당 값을 찾는다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* As an example, code has been provided that prints the value stored under the 'Puffin' key.     
* The code on line 4 It will print 104 (do you see why?).     
* Your code should be very similar, but should target the other two keys ('Sloth' and 'Burmese Python').    



**설명:** [ Hint ]         
• 딕셔너리 residents 의 key 'Puffin'을 지정하면 해당 key의 value 값 104가 반환된다.    
• e.g. print residents['Puffin'] # 104
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Assigning a dictionary with three key-value pairs to residents:
residents = {'Puffin' : 104, 'Sloth' : 105, 'Burmese Python' : 106}

print residents['Puffin'] # Prints Puffin's room number

# Your code here!
print residents['Sloth']
print residents['Burmese Python']
```

**설명:** [ Solution ]         
• residents['Sloth'] 와 같이 ( [] ) 에 Key 값을 주면 해당 key와 매치되는 value(값) 105 를 반환한다. 
{: .notice--info}

<br>


**결과** 
``` 
104
105
106
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font>    

### 11. New Entries    

Like Lists, Dictionaries are mutable. This means they can be changed after they are created. One advantage of this is that we can add new key/value pairs to the dictionary after it is created like so:

```python
dict_name[new_key] = new_value
```    

An empty pair of curly braces `{}` is an empty dictionary, just like an empty pair of `[]` is an empty list.

The length `len()` of a dictionary is the number of key-value pairs it has. Each pair counts only once, even if the value is a list. (That's right: you can put lists inside dictionaries!)





**설명:** [ Learn ]          
• Ch11. New Entries 에서는 딕셔너리의 다양한 기능을 학습한다.    
• 딕셔너리도 리스트와 마찬가지로 변형이 가능하다.    
• 여기서 변형은 추가/삭제 이다.     
• 추가/삭제는 key/value 쌍으로 추가/삭제 해야 한다.     
• e.g. dict_name[new_key]=new_value     
• 딕셔너리 초기화는 ( {} ) 를 사용한다.    
• e.g. dict_name = {}    
• 리스트 초기화와 구별하자.    
• e.g. list_name = []         
• 내장함수 len() 를 사용하여, 딕셔너리의 쌍의 갯수가 몇개인지 알 수 있다.    
• key/value 는 1:1 매칭이다.     
• value 의 값은 리스트 형(type)이기에, key1:[list1, list2] 와 같이 사용할 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Add at least three more key-value pairs to the `menu` variable, with the dish name (as a "string") for the key and the price (a float or integer) as the value. Here's an example:    

<p style="page-break-before: always;"></p>
<br>

```python
menu['Spam'] = 2.50
```

**설명:** [ Instruction ]          
• 딕셔너리 menu 에 3개 이상의 key/value 를 추가하라.     
• kye 값은 음식명으로 하고, value 값은 가격으로 하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
• You will need to add at least three key-value pairs. One has already been added on line 2.     
• Your code will follow the same format, but should create and assign different keys!


**설명:** [ Hint ]         
• 3개의 key/value가 필요하다.    
• 이미 1개는 있으니, 2번째, 3번째 key/vaue를 만들면 된다.     
• key는 중복이 안된다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
menu = {} # Empty dictionary
menu['Chicken Alfredo'] = 14.50 # Adding new key-value pair
print menu['Chicken Alfredo']

# Your code here: Add some dish-price pairs to menu!
menu['Hamburger'] = 8.50
menu['Pizza Slice'] = 3.50
menu['Salad'] = 10.00

print "There are " + str(len(menu)) + " items on the menu."
print menu
```

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• 딕셔너리 menu 에 key 값 'Hamburger' 에 value(값) 8.50 을 매칭시켜 저장한다.    
• 딕셔너리 menu 에 key 값 'Pizza Slice' 에 value(값) 3.50 을 매칭시켜 저장한다.    
• 딕셔너리 menu 에 key 값 'Salad' 에 value(값) 10.00 을 매칭시켜 저장한다.    
{: .notice--info}



**결과** 
``` 
14.5
There are 4 items on the menu.
{'Chicken Alfredo': 14.5, 'Pizza Slice': 3.5, 'Hamburger': 8.5, 'Salad': 10.0}
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font>    
### 12. Changing Your Mind    

Because dictionaries are mutable, they can be changed in many ways. Items can be removed from a dictionary with the `del` command:    

```python
del dict_name[key_name]
```    

will remove the key key_name and its associated value from the dictionary.

A new value can be associated with a key by assigning a value to the key, like so:    

```python
dict_name[key] = new_value
```



**설명:** [ Learn ]     
• Ch12. Changing Your Mind 에서는 딕셔너리 삭제(del)에 대하여 학습한다.    
• 딕셔너리 삭제는 명령어 del 을 사용하여 삭제할 수 있다.    
• e.g. del dict_name[key_name]     
• 딕셔너리 dict_name 에 key_name 과 매칭되는 value(값)를 삭제할 수 있다.   
• 삭제는 key/value 쌍이 삭제된다.    
• 참고로, dict_name[key]=new_value 로 추가할 수 있다.    
• 단, key는 중복 할 수 없다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Delete the 'Sloth' and 'Bengal Tiger' items from `zoo_animals` using `del`.

* Set the value associated with 'Rockhopper Penguin' to anything other than 'Arctic Exhibit'.

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]          
• 딕셔너리의 key 값이 'Sloth', 'Bengal Tiger'인 항목(값)을 삭제하라.    
• 삭제는 명령어 del 을 사용하라.    
• 딕셔너리의 key 값 'Rockhopper Penguin' 의 value(값) 'Arctic Exhibit'을 'Plains Exhibit' 으로 변경하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Check out the examples in the instructions if you need help!


**설명:** [ Hint ]          
• 주석을 잘 읽어보면 도움이 된다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# key - animal_name : value - location 
zoo_animals = { 'Unicorn' : 'Cotton Candy House',
'Sloth' : 'Rainforest Exhibit',
'Bengal Tiger' : 'Jungle House',
'Atlantic Puffin' : 'Arctic Exhibit',
'Rockhopper Penguin' : 'Arctic Exhibit'}
# A dictionary (or list) declaration may break across multiple lines

# Removing the 'Unicorn' entry. (Unicorns are incredibly expensive.)
del zoo_animals['Unicorn']

# Your code here!
del zoo_animals['Sloth']
del zoo_animals['Bengal Tiger']
zoo_animals['Rockhopper Penguin'] = 'Plains Exhibit'

print zoo_animals
```

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• 명령어 del 을 사용하여 딕셔너리 zoo_animals 의 key값 'Sloth' 를 삭제한다.    
• 명령어 del 을 사용하여 딕셔너리 zoo_animals 의 key값 'Bengal Tiger' 를 삭제한다.    
• 딕셔너리 zoo_animals 의 key값 'Rockhopper Penguin' 의 value(값)는 원래 'Arctic Exhibit' 이었다.     
• key값 'Rockhopper Penguin' 의 value(값) 을 'Plains Exhibit'로 변경했다.
{: .notice--info}



**결과** 
``` 
{'Atlantic Puffin': 'Arctic Exhibit', 'Rockhopper Penguin': 'Plains Exhibit'}
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 13. Remove a Few Things    

Sometimes you need to remove something from a list.

```python
beatles = ["john","paul","george","ringo","stuart"]
beatles.remove("stuart")
print beatles
```    
This code will print:    
```
 ["john","paul","george","ringo"]
```    

* We create a list called `beatles` with 5 strings.
* Then, we remove the first item from beatles that matches the string "stuart". Note that `.remove(item)` does not return anything.
* Finally, we print out that list just to see that "stuart" was actually removed.




**설명:** [ Learn ]          
• Ch13. Remove a Few Things 에서는 리스트의 삭제를 학습한다.    
• 리스트에서도 항목(값) 삭제가 가능하다.    
• 리스트 beatles 에 5개의 항목이 있다.     
• 메서드 .remove 를 사용하여 항목 'stuart'를 삭제한다.     
• 리스트 beatles 에는 4개의 항목이 남아 있다.     
• 리스트도 딕셔너리처럼 해당 값을 지정하여 직접 삭제할 수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Remove `'dagger'` from the list of items stored in the `backpack` variable.

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]          
• 리스트 backpack 의 항목 'dagger' 를 삭제하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Check out the examples in the instructions to review how to remove items from a list!


**설명:** [ Hint ]          
• 상단의 리스트를 삭제하는 법을 다시한번 읽어 보고 참조하자.    
• 주의) .remove[] 가 아니다.  .remove() 를 사용하자.
{: .notice--info}


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
backpack = ['xylophone', 'dagger', 'tent', 'bread loaf']
backpack.remove('dagger')
```

**설명:** [ Solution ]      
• 리스트의 항목중 하나인 'dagger' 를 삭제한다.    
• 메서드 .remove() 를 사용하여, 'dagger'를 직접 지정하여 삭제한다.   
• backpack.remove('dagger') 
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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 14. It's Dangerous to Go Alone! Take This    

Let's go over a few last notes about dictionaries    

```python
my_dict = {
  "fish": ["c", "a", "r", "p"],
  "cash": -4483,
  "luck": "good"
}
print my_dict["fish"][0]
```    

* In the example above, we created a dictionary that holds many types of values.    

* The key "fish" has a list, the key "cash" has an int, and the key "luck" has a string.    

* Finally, we print the letter `"c"`. When we access a value in the dictionary like `my_dict["fish"]`, we have direct access to that value (which happens to be a list). We can access the item at index `0` in the list stored by the key `"fish"`.




**설명:** [ Learn ]       
• Ch14. It's Dangerous to Go Alone! Take This 에서는 딕셔너리를 복습한다.    
• 딕셔너리에 대하여 전체적으로 정리해 보자.     
• key 'fish' 는 value 로 리스트를 가진다.    
• key 'cash' 는 value 로 숫자를 가진다.    
• key 'luck' 는 value 로 문자열을 가진다.        
• 문자 'c' 를 출력하기 위해선, key 가 'fish'이면서, value(값)가 리스트의 인덱스 값 0 인 것을 출력한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    
<p style="page-break-before: always;"></p>
<br>

* Add a key to `inventory` called `'pocket'`

* Set the value of `'pocket'` to be a list consisting of the strings `'seashell', 'strange berry', and 'lint'`

* `.sort()` the items in the list stored under the `'backpack'` key

* Then `.remove('dagger')` from the list of items stored under the `'backpack'` key

* Add `50` to the number stored under the `'gold'` key




**설명:** [ Instruction ]          
• 딕셔너리에 inventory 에 key 'pocket' 를 추가하라.      
• key 'pocket' 의 value 에는 리스트 ['seashell', 'strange berry', 'lint']를 저장하라.    
• key 'backpack' 의 value 를 메소드 .sort() 를 사용하여 정렬하라.    
• key 'backpack' 의 value(값)인 리스트 중에서 'dagger' 를 삭제하라.    
• 메소드 .remove('dagger') 를 사용하여 삭제하라.    
• key 'gold' 에 value(값) 500에 50 을 더하라.    
• 마지막에 출력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can use methods with a list stored in a dictionary as follows:    

```python
dict_name['list_key'].method()
```    

* For example, since 'backpack' is a key in our dictionary inventory you can delete 'dagger' from the corresponding list like this:    

```python
inventory['backpack'].remove('dagger')
```


**설명:** [ Hint ]     
• 딕셔너리의 value가 리스트인 것의 값을 삭제하는 방법은 다음과 같다.    
• e.g. inventory['backpack'].remove('dagger')      
• 주의) add 50 은 기존 값(500)에 추가로 더하는 것이다.(항목을 리스트로 만드는것이 아니다.) 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
inventory = {
  'gold' : 500,
  'pouch' : ['flint', 'twine', 'gemstone'], # Assigned a new list to 'pouch' key
  'backpack' : ['xylophone','dagger', 'bedroll','bread loaf']
}

# Adding a key 'burlap bag' and assigning a list to it
inventory['burlap bag'] = ['apple', 'small ruby', 'three-toed sloth']

# Sorting the list found under the key 'pouch'
inventory['pouch'].sort() 

# Your code here
inventory['pocket'] = ['seashell', 'strange berry', 'lint']
inventory['backpack'].sort()
inventory['backpack'].remove('dagger')
inventory['gold'] = inventory['gold'] + 50

print (inventory)
```

**설명:** [ Solution ]    
• 리스트 inventory['pocket'] 의 value(값)로 리스트 ['seashell', 'strange berry', 'lint'] 를 대입하였다.    
• 리스트 inventory['backpack'] 의 value(값)인 리스트를 정렬 하였다.    
• 정렬은 메소드 .sort() 를 사용하였다.    
• e.g. inventory['backpack'].sort()         
• 삭제는 inventory['backpack'] 의 value(값)인 리스트 'dagger'를 지정해서 삭제했다.   
• e.g. inventory['backpack'].remove('dagger')    
• 추가는 리스트의 key 값을 지정하여 value(값)를 변경할 수 있다.    
• e.g. inventory['gold'] = inventory['gold'] + 50     
• key 'gold' 의 원래 value 값 500 에 추가로 50을 추가한다. 
{: .notice--info}


**결과** 
``` 
{'pocket': ['seashell', 'strange berry', 'lint'], 'backpack': ['bedroll', 'bread loaf', 'xylophone'], 'pouch': ['flint', 'gemstone', 'twine'], 'burlap bag': ['apple', 'small ruby', 'three-toed sloth'], 'gold': 550}

```
