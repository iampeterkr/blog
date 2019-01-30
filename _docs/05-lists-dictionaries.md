---
# layout : rchive
title: "Lists & Dictionaries"
permalink: /lists-dictionaries/
excerpt: "We learn about Lists and Dictonaries Syntax."
last_modified_at: 2018-12-24T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---


<hr style="border: solid 1px #dddddd ;">    

LESSON    

Lists and dictionaries are powerful tools you can use to store, organize, and manipulate all kinds of information.

**설명:** [ 학습방향 ]     
리스트와 딕셔너리에 대한 공부를 해보자.    
이들은 모든 종류의 데이타를 저장, 구성 및 조작 하는데 활용할 수 있는 강력한 도구이다.     
{: .notice--info}     
     
    
<hr style="border: solid 1px #dddddd ;">


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 1. Introduction to Lists    

**Lists** are a **datatype** you can use to store a collection of different pieces of information as a sequence under a single variable name. (Datatypes you've already learned about include strings, numbers, and booleans.)

You can assign items to a list with an expression of the form

```python
list_name = [item_1, item_2]
```

with the items in between brackets. A list can also be empty: empty_list = [].

Lists are very similar to strings, but there are a few key differences 



**설명:**    
리스트는 다른 형태의 타입을 모아 놓은 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** The list `zoo_animals` has three items (check them out on line 1). Go ahead and **add** a **fourth**! Just enter the name of your favorite animal (as a "string") on line 1, **after the final comma** but before the closing ].


**설명:**    
① 리스트 `zoo_animals`에는 3개의  값들이 들어가 잇다. 마지막에 4번째 자신이 좋아하는 동물 이름을 추가하라. 주의) 동물이름은 String 형으로 하고, 마지막에 추가하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

Remember:

```python
list_name = ["item_0", "item_1", "item_2", "your_item"]
```
If your favorite animals are already on the list, add an animal that's exciting, but inexpensive. (This is a poor zoo with very few animals.)    

**설명:**    
자신이 좋아하는 동물이 이미 리스트에 있다면, 리스트에 없는 동물을 추가해 보라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
zoo_animals = ["pangolin", "cassowary", "sloth", "dog"];
# One animal is missing!

if len(zoo_animals) > 3:
  print "The first animal at the zoo is the " + zoo_animals[0]
  print "The second animal at the zoo is the " + zoo_animals[1]
  print "The third animal at the zoo is the " + zoo_animals[2]
  print "The fourth animal at the zoo is the " + zoo_animals[3]
```

**설명:**     
리스트에 있는 동물의 수가 4개 이상이면, 리스트 `zoo_aimals` 값들이 출력된다. 
{: .notice--info}


**결과** 
``` 
The first animal at the zoo is the pangolin
The second animal at the zoo is the cassowary
The third animal at the zoo is the sloth
The fourth animal at the zoo is the dog
```

<br>
<br>    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png) 
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 2. Access by Index    

You can access an individual item on the list by its index. An index is like an address that identifies the item's place in the list. The index appears directly after the list name, in between brackets, like this: ```python
list_name[index]
```

List indices begin with **0, not 1**! You access the first item in a list like this: list_name[0]. The second item in a list is at index 1: list_name[1]. Computer scientists love to start counting from zero.

 
**설명:**    
리스트의 각 항목값을 주소로 지정할수 있다. 주소의 시작은 `0`부터 시작한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Write a statement that prints the result of adding the second and fourth items of the list. Make sure to access the list by index!

```python
numbers = [5, 6, 7, 8]

print "Adding the numbers at indices 0 and 2..."
print numbers[0] + numbers[2]
print "Adding the numbers at indices 1 and 3..."
# Your code here!

```
**설명:**    
① 리스트 `numbers = [5,6,7,8]`에서 `0`번 주소와 `2`주소 값을 더하여 출력하는 소스이다. # Your code here ! 밑에 `1`번 주소와 `3`번 주소 값을 더하여 출력하는 소스를 구현하라. 
{: .notice--info}



<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

Remember:

1 List indices begin with 0, not 1.
2 The second item will have an index of 1.
3 The fourth item will have an index of 3.    

**설명:**    
리스트의 주소는  `0` 부터 시작한다. 
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

**설명:** numbers[1]은 `7` 이며, numbers[3]은 `8` 이다. 
{: .notice--info}


**결과** 
```
Adding the numbers at indices 0 and 2...
12
Adding the numbers at indices 1 and 3...
14
```

<br>
<br>    
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

**설명:** 리스트의 주소값을 지정하면(`zoo_animals[0]`), 리스트의 해당 항목(`pangolin`)을 읽을수 있고, 해당 리스트의 주소값을 입력하면(`zoo_animals[2] = "hyena"`), `zoo_animals[2]`값 `sloth`을 `hyena`로 변경할 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Write an assignment statement that will replace the item that currently holds the value `"tiger"` with another animal (as a string). It can be any animal you like.

**설명:** ① `zoo_animals[3]="tiger"`을 당신이 좋아하는 다른 동물로 바꾸어라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

Remember:

1. List indices begin with 0, not 1!
2. The fourth item will have an index of 3.    


**설명:** 주소(indices)는 `0`부터 시작한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


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

**설명:** `zoo_animals[3]`에 `lion` 문자열을 넣는다. 
{: .notice--info}



**결과** 
``` 
Skip
```

<br>
<br>    
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
2. Then, we **add** the string `'d'` to the end of the letters list.
3. Next, we print out **4**, the length of the letters list.
4. Finally, we print out `['a', 'b', 'c', 'd']`.


**설명:**    
① 리스트 `letters` 만들고, 그 값으로 `a`,`b`,`c` 값을 넣는다.
② 값 `d`를 append 내장 함수 `append`를 사용하여 추가한다. 
③ 리스트 `letters`의 길이를 내장 함수 `len`을 사용하여 출력한다.  
④ 리스트 `letters`의 전체 값을 출력한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** On lines 5, 6, and 7, append three more items to the `suitcase` list, just like the second line of the example above. (Maybe bring a bathing suit?)

Then, set `list_length` equal to the length of the suitcase list.


**설명:** ① 5,6,7 라인에 리스트 `suitcase`에 3개의 아이템 값을 추가하고(`append`활용 ), 변수 `list_length`에 리스트 `suitcase`의 길이(`len`활용)를 저장하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

That bit of `%` magic on line 11 is the string formatting we learned earlier. The `%d` tells Python to expect an integer to insert instead of a string value (%s).    



**설명:** `%`는 앞에서 배운 변수의 갑을 대체하는 기호이며, `%d` 는 숫자를 출력하기 위한 형태이다. 스트링을 출력하기 위해선 `%s`를 활용한다.   
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

**설명:** `.append`내장 함수를 활용하여, 각 `shirt`, `pants`, `shoes`를 추가하고, 리스트 `suitcase`의 길이를 `len(suitcase)`를 활용하여 구하여 변수 `list_length`에 저장한다. 마지막으로 해당 변수값을 출력한다.  
{: .notice--info}



**결과** 
``` 
There are 4 items in the suitcase.
['sunglasses', 'shirt', 'pants', 'shoes']
```

<br>
<br>    
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

Then, we take a subsection of the list and store it in the slice list. We do this by defining the indices we want to include after the name of the list: `letters[1:3]`. In Python, when we specify a portion of a list in this manner, we **include** the element with the **first index**, 1, but we **exclude** the element with the **second index**, 3.

Next, we print out slice, which will print `['b','c']`. Remember, in Python indices always **start at 0**, so the 1 element is actually b.

Finally, we print out `['a', 'b', 'c', 'd', 'e']`, notice that we did not modify the original letters list.


**설명:**    
리스트 `letters`에서 특정 인덱스에 있는 값들, 예를 들어, `b, c`값만 뽑아 낼려고하면, 리스트에서 인덱스 값의 범위를 주어 뽑아 낼수 있다. `letters[1:3]`이라고 주어지면, 리스트 `letters`의 1번 주소 부터 3번 주소까지만 잘라 내겠다는 이야기다. 단, 잘라내는 규칙은 첫번째 항목은 포함되고, 두번째 항목은 포함되지 않는다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** On line 7, create a list called `middle` containing only the **two middle items** from `suitcase`.

On line 10, create a list called `last` made up only of the **last two items** from `suitcase`.


**설명:**    
① Edit 화면 7번 라인에서, 리스트 `suitcase`에서 중간에 있는 2개의 항목(값)을 뽑아내어 리스트 `middle` 변수에 대입하라.    
② Edit 화면 10번 라인에서, 리스트 `suitcase`에서 마지막 2개의 항목(값)을 뽑아내어, 리스트 `last` 변수에 대입하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

In order to slice the last two items from the list
`myList = [0,1,2,3,4]`, the ending index of your slice will be one beyond the actual last index of the list. Check it out:
```python
myList[3:5]
# Returns [3, 4]    
```


**설명:**    
인덱스 3, 4만 잘아 내겠다는 의미이다. 
{: .notice--info}

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

**설명:** 
① `suitcase[2:4]`는 인덱스 `2, 3`인 `"passport"`, `"laptop"` 이 선택되고,     
② `suitcase[4:6]`는 인덱스 `4, 5`인 `"suit"`, `"shoes"`가 잘라짐.
{: .notice--info}



**결과** 
``` 
Skip
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 6. Slicing Lists and Strings    

You can **slice** a string exactly like a list! In fact, you can think of strings as lists of characters: each character is a sequential item in the list, starting from index **0**.
```python
my_list[:2]
# Grabs the first two items
my_list[3:]
# Grabs the fourth through last items
```
If your list slice includes the very first or last item in a list (or a string), the index for that item doesn't have to be included.


**설명:**     
문자열도 각 알파벳별 인덱스가 부여되어 있다. 문자열도 각 항목의 인덱스 값으로 잘라 낼수 있다.     
`my_list[:2]`는 처음부터 인덱스 2번(미포함)까지 뽑아냄. 처음부터 두번째 까지 개념.   
`my_list[3:]`는 인덱스 3번(포함)부터 끝까지 뽑아냄. 즉, 4번째 항목부터 끝까지 개념.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Assign to `dog` a slice of `animals` from **index 3** up until but **not including index 6**.

**②** Assign to `frog` a slice of `animals` from **index 6** until the **end** of the string.


**설명:**    
① 리스트 `dog` 변수에 `animals`의 인덱스 3번(포함) 부터 6번(미포함)까지 잘라내서 저장    
② 리스트 `frog` 변수에 `animals`의 인덱스 6번(포함) 부터 끝까지 잘라내서 저장. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

Remember: you don't need the first index if you're starting from the beginning of the string, and you don't need the second index if you're going all the way to the end!    


**설명:**    
첫번째 인덱스는 포함, 마지막 인덱스는 미포함. 그리고 마지막 인덱스를 적지 않으면 끝까지 임.

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

**설명:**    
① `animals[3:6]`은 인덱스 3(포함) 부터 인덱스 6[미포함]까지 잘라냄.(`dog`)    
② `anmals[6:]`은 인덱스 6(포함)부터 끝까지 잘라냄. (`frog`)
{: .notice--info}



**결과** 
``` 
Skip
```

<br>
<br>    
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
**①** First, we create a list called `animals` with three strings.
**②** Then, we print the **first** index that contains the string **"bat"**, which will print **1**.
We can also insert items into a list.
```python
animals.insert(1, "dog")
print animals
```
**①**We insert **"dog"** at index **1**, which moves everything down by 1.
**②**We print out **["ant", "dog", "bat", "cat"]**




**설명:**    
**①** 리스트 `animals`에 3개의 스트링 "ant", "bat", "cat"이 들어 있다.     
**②** 리스트 `animals`의 인덱스 1번 자리에 "dog"를 추가 하고자 하면 다음과 같이 사용할수 있다.    
방법은 `animals.insert(1,"dog")` 해당 추가하고자 하는 인덱스 번호와 값을 지정해주면 된다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Use the `.index(item)` function to find the index of **"duck"**.    
**②** Assign that result to a variable called `duck_index`.    
**③** Then `.insert(index, item)` the string **"cobra"** at that index.  


**설명:**    
**①** 리스트 `animals`에서 "duck"의 인데스 값을 내장함수 `.index("duck")`를 사용하여 해당 인덱스 값을 알아 내라.     
**②** "duck"의 인덱스 값을 변수 `duck_index`에 저장하라.   
**③** 내장함수 `.index(index.item)`을 활용하여 리스트 `animals`의 "duck" 자리에  "cobra" 문자열을 추가하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

You're **not replacing** "duck" with "cobra"—you're just finding "duck", then inserting "cobra".    



**설명:**    
"duck" 대신 "cobra"를 대체하는 것이 아니라, "duck" 자리에 "cobra"가 삽입 되는 것이다. 정상적으로 되면 "duck"는 "cobra"에 다음에 올것이다. 
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

**설명:**     
`duck_index`에 "duck" 인덱스 `2`가 저장되고, 리스트 `animals.insert(2, "cobra")`와 같이 실행되면, `animals`에 `"duck"`가 index `3`이 되고, `"cobra"`가 index `2` 자리에 삽입된다. 
{: .notice--info}



**결과** 
``` 
['aardvark', 'badger', 'cobra', 'duck', 'emu', 'fennec fox']
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 8. For One and All    

If you want to do something with **every item** in the list, you can use a for **loop**. If you've learned about for **loops** in JavaScript, pay close attention! They're different in Python.
```python
for variable in list_name:
  # Do stuff!
```
A `variable` name follows the `for` keyword; it will be assigned the value of each list item in turn.

Then in `list_name` designates `list_name` as the list the loop will work on. The **line ends** with a colon `(:)` and the indented code that follows it will be executed once per item in the list.


**설명:**    
리스트에 있는 항목(값)들을 모두 뽑아 내려면, 일일이 해당 인덱스 값을 지정해 주어도 되지만, `for` loop문을 사용하여 뽑아 낼수도 있다.    
방법은 `for` 다음에 리스트에 뽑아낸 항목을 저장할 변수를 지정하고, `in` 다음에 리스트를 적고, 마지막에 `:`을 적으면 된다.  `for`문으로 반복적인 작업을 할 내용들은 `for` 밑에 들여 쓰기를 하여 정의해준다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Write a statement in the indented part of the **for-loop** that prints a number equal to 2 * number for every list item.


**설명:**    
**①** `for`문을 사용하여 리스트 my_list 에서 추출한 값을 각각 x 2를 하여 출력 하여라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

Each list item is assigned to the user-defined variable number in turn. All you need to do is print two times number in the body of the loop (the indented part).

The for loop will automatically execute your code as many times as there are items in my_list!    



**설명:**    
변수 `number`에 리스트 `my_list` 항목(값) 들이 하나씩 자동으로 뽑아져 저장된다. 변수 `number`에 x 2 를 하여 출력하자.    
단, `for`문을 쓰기 위해서는 들여 쓰기를 주의해야한다. 
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

**설명:**    
리스트 `my_list`의 값 `1,9,3,8,5,7`이 자동으로, 변수 `number`에 저장된다. `for` 문을 반복적으로 돌면서, number x 2 가 출력한다. 
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

<br>
<br>    
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
**①** First, we create a list called `animals` with **three strings**. The strings are not in alphabetical order.     
**②** Then, we **sort** `animals` into alphabetical order. Note that `.sort()` modifies the list rather than returning a new list.    
**③** Then, for each item in `animals`, we print that item out as **"ant", "bat", "cat"** on their own line each.



**설명:**    
**①** 리스트 `animals`에 3개의 문자열이 알파멧 순서와 상관없이 뒤죽박죽 정리되어 있다.    
**②** 내장 함수 `.sort()`를 사용하여, 리스트 `animals`를 알파멧 오름차순으로 정렬하였다.     
**③** 이후, 정렬된 리스트 `animals`를 출력 해보면, 리스트의 각 항목(값)이, 알파벳 오름차순으로 정렬 되어 있음을 알수 있다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Write a for-loop that iterates over `start_list` and `.append()`s each number **squared (x ** 2)** to `square_list`.

**②** Then sort `square_list`!


**설명:**    
**①** 리스트 `start_list`에 `.append()`를 활용하여, 각 항목(값)의 제곱근 값을 만들어서, 리스트 `square_list`에 저장하라.    
**②** 리스트 `square_list`를 sort 함수를 사용하여 정렬 하여라. 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You will need to use:

1. A for loop
2. The .append() method
3. The .sort() method
Feel free to peek back at previous exercises in this section if you need to!




**설명:**     
**①** `for` 문을 사용하고      
**②** `.append()`를 사용하고    
**③** `.sort()`를 사용하라.    
**④** 해당 내장형 함수 사용법이 기억이 나지 않으면, 앞 장에서 배운 것을 다시 확인하라. 
{: .notice--info}

<br>
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

**설명:**     
**①** `for`문에서, 리스트 `start_list`에서 각 항목값을 변수 `number`에 저장하고,     
**②** 변수 `number`를 `.append()`를 제곱근을 구하여, 리스트 `square_list`에 저장하고,    
**③** 리스트 `square_list`를 `.sort()`를 활용하여 정렬한다.    
**④** 리스트 `square_list`를 출력한다. 
{: .notice--info}



**결과** 
``` 
[1, 4, 9, 16, 25]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 10. This Next Part is Key    

A **dictionary** is similar to a **list**, but you access values by looking up a **key** instead of an **index**. A key can be **any string or number**. Dictionaries are **enclosed** in curly braces, like so:
```python
d = {'key1' : 1, 'key2' : 2, 'key3' : 3}
```
This is a dictionary called `d` with **three key-value pairs**. The key 'key1' points to the value 1, 'key2' to 2, and so on.

Dictionaries are great for things like phone books (pairing a name with a phone number), login pages (pairing an e-mail address with a username), and more!

 



**설명:**     
딕셔너리에 대하여 알아보자.    
딕셔너리는 리스트와 비슷하다.  리스트는 눈에 보이지 않는 인덱스를 가지고 해당 항목(값)을 나타내지만, 딕셔너리는 **key**를 이용하여 해당 항목(값)을 나타낸다.     
예와같이 `d = {'key1' : 1, 'key2' : 2, 'key3' : 3}` `key:값`의 형태로 표현되며, `key1`을 키(key)라 부르면 이와 매칭되는 `1`을 값(value)이라 부른다.    
딕셔너리 특징은 key 값은 문자열, 숫자 모두 가능한다. 꼭 key/value 한쌍이어야 한다. 그리고 key는 중복 된 이름을 가질수 없다.       
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Print the values stored under the `'Sloth'` and `'Burmese Python'` keys. Accessing dictionary values by key is just like accessing list values by index:
```python
residents['Puffin']# Gets the value 104
```
Check the Hint if you need help!




**설명:**     
**①** 딕셔너리 `residents`에서 key 값이 `Sloth`, `Burmese Python`인 것의 값(value)를 출력하라.    
참고로, 리스트는 `[]`에 index값을 지정하여 해당 값을 찾는다. 하지만, 딕셔너리는 `[]`에 key 값을 지정하여 해당 값을 찾는다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)As an example, code has been provided that prints the value stored under the 'Puffin' key. The code on line 4 It will print 104 (do you see why?). Your code should be very similar, but should target the other two keys ('Sloth' and 'Burmese Python').    



**설명:**    
`print residents['Puffin'] `를 참고하라. 
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

**설명:**    
`residents['Sloth']`와 같이 `[]`에 Key 값을 주면 해당 key와 매치되는 항목(값) `105`를 반환한다. 
{: .notice--info}



**결과** 
``` 
104
105
106
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 11. New Entries    

Like Lists, Dictionaries are **mutable**. This means they can be changed after they are created. One advantage of this is that we can add new **key/value** pairs to the dictionary after it is created like so:
```python
dict_name[new_key] = new_value
```
An empty pair of curly braces `{}` is an **empty dictionary**, just like an empty pair of `[]` is an **empty list**.

The length `len()` of a dictionary is the number of key-value pairs it has. Each pair counts only once, even if the value is a list. (That's right: you can put lists inside dictionaries!)





**설명:**     
딕셔너리도 리스트와 마찬가지로 변형이 가능하다. 여기서 변형은 추가/삭제 이다. 추가 하기 위해선 `dict_name[new_key]=new_value`와 같이 쌍으로 해야 한다.    
딕셔너리 초기화는 `{}`로 할수 있다. `[]`는 리스트 초기화 이니, 혼돈하지 말자.    
`len()` 함수를 사용하면 해당 딕셔너리이 쌍의 갯수가 몇개인지 알수 있다. key/value는 1:1 매칭이다. value 의 값은 리스트 형이기에, key1:[list1, list2] 와 같이 사용할수도 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Add at least three more **key-value** pairs to the `menu` variable, with the dish name (as a "string") for the key and the price (a float or integer) as the value. Here's an example:
```python
menu['Spam'] = 2.50
```

**설명:**     
**①** 딕셔너리 `menu`에 3개 이상의 `key/value`를 추가하라.     
kye값은 음식명으로 하고, value 값은 가격으로 하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You will need to add at **least three key-value** pairs. One has already been added on line 2. Your code will follow the same format, but should create and assign different keys!


**설명:**    
3개의 key/value가 필요하다. 이미 1개는 있으니, 2,3번 key/vaue를 만들면 된다. key는 중복이 안된다. 
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

**설명:**     
딕셔너리 `menu`에 key `Hamburger, Pizza Slice, Salad` 에 각각  value `8.50, 3.50, 10.00`을 매칭 시켜 저장한다.   
{: .notice--info}



**결과** 
``` 
14.5
There are 4 items on the menu.
{'Chicken Alfredo': 14.5, 'Pizza Slice': 3.5, 'Hamburger': 8.5, 'Salad': 10.0}
```

<br>
<br>    
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
will **remove** the key key_name and its associated value from the dictionary.

A new value can be associated with a key by assigning a value to the key, like so:
```python
dict_name[key] = new_value
```



**설명:**     
딕셔너리 삭제는 `del` 명령어로 삭제할 수 있다.    
`del dict_namep[key_name]`같이 key값을 가지고 해당 key에 매칭되는 value를 딕셔너리에서 삭제할 수 있다.    
딕셔너리에 추가는 앞에서 배운바와 같이 `dict_name[key]=new_value`로 추가할수 있다.    
단, key는 중복 할 수 없다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Delete the **'Sloth'** and **'Bengal Tiger'** items from `zoo_animals` using `del`.

**②** Set the value associated with **'Rockhopper Penguin'** to anything other than **'Arctic Exhibit'**.


**설명:**     
**①** `del` 명령을 사용하여 딕셔너리의 key값이 `Sloth`, `Bengal Tiger`인 항목들을 삭제하시오.     
**②** 딕셔너리에서 key 값이 `Rockhopper Penguin`인 value `Arctic Exhibit`를 다른 값으로 바꾸시오. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Check out the examples in the instructions if you need help!


**설명:**     
주석을 잘 읽어보면 도움이 된다. 
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

**설명:**     
`del`명령을 사용하여 key값인 `Sloth`, `Bengal Tiger`를 삭제하고, key값이 `Rockhopper Penguin`인 value 값을  `zoo_animals['Rockhopper Penguin']= 'Plains Exhibit'` 와 같이 변경한다. 

{: .notice--info}



**결과** 
``` 
{'Atlantic Puffin': 'Arctic Exhibit', 'Rockhopper Penguin': 'Plains Exhibit'}
```

<br>
<br>    
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
**①** We create a list called `beatles` with 5 strings.
**②** Then, we remove the first item from beatles that matches the string "stuart". Note that .remove(item) does not return anything.
**③** Finally, we print out that list just to see that "stuart" was actually removed.




**설명:**     
딕셔너리에서 삭제가 가능하듯이, 리스트에서도 항목(값) 삭제가 가능하다.    
코드에서 보듯이 리스트 `beatles`에 5개의 항목이 있다. 이중 `stuart`를 내장함수 `.remove`를 이용하여 삭제하면, 리스트 `beatles`에는 4개의 항목(값)이 남아 있다.     
리스트의 값을 삭제할때 해당 값을 딕셔너리 처럼 지정하여 삭제할 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Remove `'dagger'` from the list of items stored in the `backpack` variable.


**설명:**     
**①** 리스트 `backpack`의 저장된 값중 하나인 `dagger`를 삭제하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Check out the examples in the instructions to review how to remove items from a list!


**설명:**     
상단의 리스트를 삭제하는 법을 다시한번 읽어 보고 참조하자. `.remove[]`가 아니라. `.remove()`임을 주의하자. 
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
backpack = ['xylophone', 'dagger', 'tent', 'bread loaf']
backpack.remove('dagger')
```

**설명:** 
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
**①** In the example above, we created a dictionary that holds many types of values.
**②** The key **"fish"** has a list, the key **"cash"** has an int, and the key **"luck"** has a string.
**③** Finally, we print the letter `"c"`. When we access a value in the dictionary like `my_dict["fish"]`, we have direct access to that value (which happens to be a list). We can access the item at index `0` in the list stored by the key `"fish"`.




**설명:**     
**①** 지끔 것 배운 딕셔너리에 대하여 전체적으로 정리해 보자.     
**②** key가 `fish`는 value를 리스트로 가지낟. key가 `cash`는 value로 숫자를 가지고, key가 `luck`인것은 문자열을 value로 가진다.        
**③** 마지막으로, 문자 `c`를 출력하기 위해선, 해당 딕셔너리의 key가 `fish`이고, 리스트 인덱스 값이 `[0]`인 것을 출력 한다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** **Add** a **key** to `inventory` called `'pocket'`

**②** Set the value of `'pocket'` to be a list consisting of the strings `'seashell', 'strange berry', and 'lint'`

**③** `.sort()` the items in the list stored under the `'backpack'` key

**④** Then `.remove('dagger')` from the list of items stored under the `'backpack'` key

**⑤** Add `50` to the number stored under the `'gold'` key




**설명:**     
**①** 딕셔너리에 `inventory`에 key `pocket`를 추가하라.      
**②** key `pocket` value에는 리스트 `seashell, strange berry, lint`를 가진다.       
**③** key `backpack`의 value를 `.sort()`하여 정렬하고,         
**④** `.remove('dagger')`를 활용하여 key `backpack` key의 값이 리스트 중에서 `dagger`를 삭제하라.             
**⑤** key `gold`에 value 값에 `50` 을 더하여라.    
**⑥** 마지막에 출력하여라.             

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can use methods with a list stored in a dictionary as follows:
```python
dict_name['list_key'].method()
```
For example, since 'backpack' is a key in our dictionary inventory you can delete 'dagger' from the corresponding list like this:
```python
inventory['backpack'].remove('dagger')
```


**설명:**
딕셔너리의 value 리스트의 값을 삭제하는 방법은 `inventory['backpack'].remove('dagger')`를 활용하라.     
주의, add `50`은 해당 값에다 더하는 것이다.(항목을 리스트로 만드는것이 아니다.) 

{: .notice--info}


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

**설명:**     
리스트는 `[]inventory['pocket'] = ['seashell', 'strange berry', 'lint']`를 활용하여, value를 입력한다.    
정렬은 `inventory['backpack'].sort()`를 활용하여 정렬한다.    
삭제는 `inventory['backpack'].remove('dagger')` 해당 key의 value항목을 지정하여 삭제한다.    
추가는 `inventory['gold'] = inventory['gold'] + 50` 는 해당 key의 value 에 `+`를 활용하여 기존 500+50을 하는 것이다. 
{: .notice--info}


**결과** 
``` 
{'pocket': ['seashell', 'strange berry', 'lint'], 'backpack': ['bedroll', 'bread loaf', 'xylophone'], 'pouch': ['flint', 'gemstone', 'twine'], 'burlap bag': ['apple', 'small ruby', 'three-toed sloth'], 'gold': 550}

```



<br>
<br>    
<br>    