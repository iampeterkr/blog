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

LESSON    

This lesson is a follow up to Unit 2: Strings and Console input and will give you practice with the concepts introduced in that lesson.


**설명:** [ 학습방향 ]     
이 장에서는 2장의 연장선으로 문자열 콘솔 출력에 대한 연습을 한다. 
{: .notice--info}     
     
    
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


![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
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


**설명:**  datetime.now() 는 현재 날짜와 시간을 알려주는 함수이다.  datetime 을 사용하기 위해서는 import 를 사용하여 datetiem 이라는 기본제공 함수를 사용한다. 
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


# ![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 3. Extracting Information

Notice how the output looks like **2013-11-25 23:45:14.317454**. What if you don't want the entire date and time?

```python
from datetime import datetime
now = datetime.now()

current_year = now.year
current_month = now.month
current_day = now.day
```
You already have the first two lines.

In the third line, we take the year (and only the year) from the variable `now` and store it in `current_year`.

In the fourth and fifth lines, we store the `month` and `day` from `now`.




**설명:** 변수 `now`에 `datetime.now()`를 저장하고,  
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
Remember, to print out the `current year`, you can type:
```python
print now.year
```

**설명:** 현재 `now`에 저장된 `year`값을 직접 출력 할 수 있다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from datetime import datetime
now = datetime.now()

print now.year
print now.month
print now.day
```

**설명:** 변수 `now`를 이용하여. `year`, `month`, `day`를 출력 한다. 
{: .notice--info}



**결과**
```
2018
11
27
```

<br>
<br>    
<br>    


![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 4. Hot Date

What if we want to print today's date in the following format? `mm/dd/yyyy`. Let's use string substitution again!

```python
from datetime import datetime
now = datetime.now()

print '%02d-%02d-%04d' % (now.month, now.day, now.year)

# will print the current date as mm-dd-yyyy
```

Remember that the standalone `%` operator after the string will fill the `%02d` and `%04d` placeholders in the string on the left with the **numbers** and **strings** in the parentheses on the right.

`%02d` pads the **month** and **day** numbers with zeros to two places, and `%04d` pads the **year** to four places. This is one way dates are commonly displayed.

**설명:** 변수 `now`에 저장된 날짜&시간을 ex)12-28-2002 와 같이 출력 하고자 할때는 `print` 할때, 각 출력되는 값의 자리수를 ex) 월과 날은 `%02d`를 사용하고, 년도는 `%04d`를 사용한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Print the current date in the form of `mm/dd/yyyy`.

Change the **string** used above so that it uses a `/` character in between the `%02d` and `%04d` placeholders instead of a `-` character.




**설명:** ① 날짜를 `mm/dd/yyyy` 포맷 형태로 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Don't forget to `import datetime`. The example code above shows you how to do so.

Make sure you use `now.day` instead of `now.date`. They are different things!


**설명:** `import datetime`을 선언해 주고, `now.day`, `now.month`, `now.year`를 이용하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from datetime import datetime
now = datetime.now()

print '%02d/%02d/%04d' % (now.month, now.day, now.year)
```

**설명:** 출력시 해당 월, 일, 년도를 `%02d/%02d/%04d`로 표현한다. 
{: .notice--info}



**결과**
```
11/27/2018
```
<br>
<br>    
<br>    



![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 5. Pretty Time

Nice work! Let's do the same for the `hour`, `minute`, and `second`.
```python
from datetime import datetime
now = datetime.now()

print now.hour
print now.minute
print now.second
```
In the above example, we just printed the current `hour`, then the current `minute`, then the current `second`.

We can again use the variable `now` to print the time.




**설명:** 변수 `now`에 저장되어 있는 값중 `hour`, `minute`, `second`를 뽑아서 각각 출력할 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Similar to the last exercise, print the current `time` in the pretty form of `hh:mm:ss`.

1. Change the string that you are printing so that you have a `:` character in between the `%02d` placeholders.

2. Change the three things that you are printing from `month`, `day`, and `year` to `now.hour`, `now.minute`, and `now.second`.




**설명:** ① 먼저 배운 날짜와 마찬가지로, time도 `hour`, `minute`, `secondd`를 구하여 사용할수 있다. 사용 방법은 `now.hour`, `now.minute`, `now.second` 이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
To get the hour, you can type:

```python
now.hour
```
You can also use `now.minute` and `now.second`.


**설명:** `now.minute`, `now.second`, `now.hour`를 참조 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from datetime import datetime
now = datetime.now()

print '%02d:%02d:%02d' % (now.hour, now.minute, now.second)
```

**설명:** `%02d:%02d:%02d`형식을 출력 할 수 있다.  
{: .notice--info}



**결과**
```
10:52:23
```
<br>
<br>    
<br>    



![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYTHON SYNTAX</font> 

### 6. Grand Finale

We've managed to print the `date` and `time` separately in a very pretty fashion. Let's combine the two!

```python
from datetime import datetime
now = datetime.now()

print '%02d/%02d/%04d' % (now.month, now.day, now.year)
print '%02d:%02d:%02d' % (now.hour, now.minute, now.second)
```
The example above will print out the `date`, then on a separate line it will print the `time`.

Let's print them all on the same line in a single print statement!



**설명:** `date`와 `time`을 출력하는 방법이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Print the date and time together in the form: `mm/dd/yyyy hh:mm:ss`.

To start, change the **format** string to the left of the `%` operator.

1. Ensure that it has five `%02d` and one `%04d` placeholder.
2. Put slashes and colons and a space between the placeholders so that they fit the format above.Then, change the variables in the parentheses to the right of the `%` operator.
3. Place the variables so that `now.month`, `now.day`, `now.year` are before now.hour, `now.minute`, `now.second`. Make sure that there is a ( before the six placeholders and a ) after them.



**설명:** ① `day/month/year hour:minute:second` 형식으로 출력하게끔 하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Don't forget to `import datetime`. Look at the example code above if you need help doing so.


**설명:** `import datetime`를 활용하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from datetime import datetime
now = datetime.now()

print '%02d/%02d/%04d %02d:%02d:%02d' % (now.month, now.day, now.year, now.hour, now.minute, now.second)
```

**설명:** `%s`를 활용하여, 각 형태를 만들고, 값을 대입한다. 
{: .notice--info}



**결과**
```
11/27/2018 20:59:59
```

<br>
<br>    
<br>    

