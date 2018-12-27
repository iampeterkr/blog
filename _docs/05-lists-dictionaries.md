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


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 1.Introduction to Lists

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


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)Remember:

```python
list_name = ["item_0", "item_1", "item_2", "your_item"]
```
If your favorite animals are already on the list, add an animal that's exciting, but inexpensive. (This is a poor zoo with very few animals.)    

**설명:**    
본이이 좋아하는 동물이 이미 리스트에 있다면, 리스트에 없는 동물을 추가해 보라. 
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


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)Remember:

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


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)Remember:

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
### 4.



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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 5. 



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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 6. 



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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 7. 



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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 8. 



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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 9. 



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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
### 10. 



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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
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
<font size="3"  face="돋움">PYTHON LISTS AND DICTIONARIES</font> 
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
