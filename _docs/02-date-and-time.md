---
# layout : rchive
title: "Date and Time"
permalink: /date-and-time/
excerpt: "We learn about Date and Time Syntax."
last_modified_at: 2018-11-25T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    
    
<hr style="border: solid 1px #dddddd ;">

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">DATA AND TIME</font> 
### 1. The datetime Library

A lot of times you want to keep track of when something happened. We can do so in Python using datetime.

Here we'll use datetime to print the date and time in a nice format.


**설명:** Python에서 날짜와 시간을 사용하고자 하면, `datetime` 클래스를 사용하여 표현 할 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Click `Run` to continue.


**설명:** ① `Run`을 클릭하여 실행해 보시오. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
**Skip**


**설명:** `skip`
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
## skip 
```

**설명:** `skip`
{: .notice--info}


**결과**
**skip**
<br>
<br>    
<br>    


<hr style="border: solid 1px #dddddd ;">
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 2. Getting the Current Date and Time
 
We can use a function called `datetime.now()` to retrieve the current **date** and **time**.

```python
from datetime import datetime
print datetime.now()
```
The first line `imports` the `datetime` library so that we can use it.

The second line will `print` out the current **date** and **time**.




**설명:**  `datetime.now()`는 현재 날짜와 시간을 알려주는 함수이다. `datetime`을 사용하기 위해서는 `import`를 사용하여 `datetiem`이라는 기본제공 함수를 사용한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a variable called `now` and store the result of `datetime.now()` in it.

Then, **print** the value of now.


**설명:** ① 변수 `now`를 만들고 그 변수에 `datetime.now()`를 대입하고, 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember that you can assign a value to the variable `now` using the assignment operator `=`

For example, if you wanted to store the value `4` in now, you would type:

```python
now = 4
```

**설명:** 변수를 대입하는것은 `=`를 활용한다.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from datetime import datetime

now = datetime.now()
print now
```

**설명:** ① 먼저 `datetime` 함수를 `import` 한다. ② 변수 `now`를 만들고 거기에 `datetime.now()`를 사용하여 변수 `now`에 현재 일자와 날짜를 저장한다.
③변수 `now`를 출력한다. 
{: .notice--info}


**결과**
```
2018-11-27 10:27:29.102097
```
<br>
<br>    
<br>    


<hr style="border: solid 1px #dddddd ;">
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
### 3.  



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



**결과**

<br>
<br>    
<br>    


<hr style="border: solid 1px #dddddd ;">
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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



**결과**

<br>
<br>    
<br>    



<hr style="border: solid 1px #dddddd ;">
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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



**결과**

<br>
<br>    
<br>    



<hr style="border: solid 1px #dddddd ;">
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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



**결과**

<br>
<br>    
<br>    



<hr style="border: solid 1px #dddddd ;">
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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



**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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



**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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



**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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



**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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



**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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



**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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


**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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

**결과**

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과**



<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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


**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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


**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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


**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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


**결과**

<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 
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


**결과**


<br>
<br>    
<br>    
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *     
<br>
<br>
