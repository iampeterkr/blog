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
### 2.  



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
### 3.  



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
### 4.



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
### 5. 



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
### 6. 



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
