---
# layout : rchive
title: "Date and Time"
permalink: /date-and-time/
excerpt: "We learn about Date and Time Syntax."
# last_modified_at: 2019-01-30T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    
<hr style="border: solid 1px #dddddd ;">    

LESSON    

This lesson is a follow up to Unit 2: Strings and Console input and will give you practice with the concepts introduced in that lesson.


**설명:** [ 학습방향 ]     
이 장에서는 2장의 연장선으로, 다양한 문자열을 콘솔에 출력하는 방법을 연습한다.
{: .notice--info}     
     
    
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">DATA AND TIME</font> 
### 1. The datetime Library    

A lot of times you want to keep track of when something happened. We can do so in Python using `datetime`.

Here we'll use `datetime` to print the date and time in a nice format.


**설명:** [ Learn ]    
• Ch1. The datetime Library 에서는 datetime 클래스를 학습한다.     
• 날짜와 시간을 사용하고자 하면, 클래스 datetime 을 사용한다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Click `Run` to continue.


**설명:** [ Instruction ]    
• Run 을 클릭하여 실행하라. 
{: .notice--info}


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
from datetime import datetime
```

**설명:** [ Solution ]    
• 클래스 datetime 으로 부터 datetime 을 import 한다.
{: .notice--info}    


**결과**  
```
#skip
```    
<p style="page-break-before: always;"></p>    
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




**설명:** [ Learn ]    
• Ch2. Getting the Current Date and Time 에서는 현재시간을 학습한다.     
• datetime.now() 는 현재 날짜와 시간을 알려주는 함수이다.    
• datetime 을 사용하기 위해서는 클래스 datetime 기본제공 함수를 사용한다.    
• datetime.now() 를 출력한다.
{: .notice--info}



<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a variable called `now` and store the result of `datetime.now()` in it.

* Then, **print** the value of now.


**설명:** [ Instruction ]    
• 변수 now 를 만들어라.    
• 변수 now 에 datetime.now() 를 대입하라.    
• 변수 now 를 출력하라. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember that you can assign a value to the variable `now` using the assignment operator `=`

* For example, if you wanted to store the value `4` in now, you would type:

```python
now = 4
```

**설명:** [ Hint ]    
• 변수를 대입할때  ( = )를 사용한다.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from datetime import datetime

now = datetime.now()
print now
```

**설명:** [ Solution ]    
• 클래스 datetime 를 import 한다.     
• 변수 now 를 만들고, datetime.now() 를 저장한다.      
• datetime.now() 는 현재 일자와 날짜를 반환한다.    
• 변수 now 를 출력한다. 
{: .notice--info}


**결과**
```
2018-11-27 10:27:29.102097
```    
<p style="page-break-before: always;"></p>
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


**설명:** [ Learn ]    
• Ch3. Extracting Information 에서는 년, 월, 일을 학습한다.     
• 변수 now 에 datetime.now() 저장하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On a new line, print `now.year`.    
* Make sure you do it after setting the `now` variable!    
* Then, print out `now.month`.    
* Finally, print out `now.day`.


**설명:** [ Instruction ]    
• 라인 3 에 다음 3 개를 작성 후 실행하라.     
• now.year 을 출력하라.    
• now.month 을 출력하라.    
• now.day 을 출력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, to print out the `current year`, you can type:    

```python
print now.year
```

**설명:** [ Hint ]    
• 변수 now 에 저장된 year 값을 직접 출력할 수 있다. 
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

**설명:** [ Solution ]    
• 변수 now 의  ( .year ) , ( .month ) , ( .day )를 출력한다. 
{: .notice--info}



**결과**
```
2018
11
27
```    
<p style="page-break-before: always;"></p>
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


**설명:** [ Learn ]    
• Ch4. Hot Date 에서는 날짜&시간의 출력 형태를 학습한다.    
• 변수 now 에 저장된 날짜 & 시간을 예제와 같이 사용하고자 한다.    
• e.g. 12-28-2002    
• print 문 출력시, 월 : %02d , 일 : %02d , 년 : %04d 로 작성한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Print the current date in the form of `mm/dd/yyyy`.

* Change the **string** used above so that it uses a `/` character in between the `%02d` and `%04d` placeholders instead of a `-` character.


**설명:** [ Instruction ]    
• 날짜를 *mm/dd/yyyy* 형태로 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Don't forget to `import datetime`. The example code above shows you how to do so.

* Make sure you use `now.day` instead of `now.date`. They are different things!


**설명:** [ Hint ]    
• import datetime 을 선언하라.    
• now.day , now.month , now.year 를 사용하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from datetime import datetime
now = datetime.now()

print '%02d/%02d/%04d' % (now.month, now.day, now.year)
```

**설명:** [ Solution ]    
• 출력을  월, 일, 년도 를 %02d/%02d/%04d 로 표현한다. 
{: .notice--info}



**결과**
```
11/27/2018
```    
<p style="page-break-before: always;"></p>
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


**설명:** [ Learn ]    
• Ch5. Pretty Time 에서는 시간을 학습한다.     
• 변수 now 에 저장 되어 있는 값 중 hour, minute, second 를 각각 출력한다.
{: .notice--info}



<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Similar to the last exercise, print the current `time` in the pretty form of `hh:mm:ss`.

* Change the string that you are printing so that you have a `:` character in between the `%02d` placeholders.

* Change the three things that you are printing from `month`, `day`, and `year` to `now.hour`, `now.minute`, and `now.second`.


**설명:** [ Instruction ]     
• 시간은 hour, minute, second 를 사용한다.    
• 사용 방법은 now.hour , now.minute , now.second 이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* To get the hour, you can type:

```python
now.hour
```
You can also use `now.minute` and `now.second`.


**설명:** [ Hint ]   
• now.minute , now.second , now.hour 를 사용하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from datetime import datetime
now = datetime.now()

print '%02d:%02d:%02d' % (now.hour, now.minute, now.second)
```

**설명:** [ Solution ]     
• 시, 분, 초 를 %02d:%02d:%02d 형식으로 출력한다.   
{: .notice--info}



**결과**
```
10:52:23
```    
<p style="page-break-before: always;"></p>
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



**설명:** [ Learn ]    
• Ch6. Grand Finale 에서는 datetime 사용법을 학습한다.    
• 날짜를 반환하는 date 와 시간을 반환하는 time 사용법을 학습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Print the date and time together in the form: `mm/dd/yyyy hh:mm:ss`.    
* To start, change the **format** string to the left of the `%` operator.    
* Ensure that it has five `%02d` and one `%04d` placeholder.    
* Put slashes and colons and a space between the placeholders so that they fit the format above.Then, change the variables in the parentheses to the right of the `%` operator.    
* Place the variables so that `now.month`, `now.day`, `now.year` are before now.hour, `now.minute`, `now.second`. Make sure that there is a ( before the six placeholders and a ) after them.



**설명:** [ Instruction ]    
• day/month/year hour:minute:second 형식으로 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Don't forget to `import datetime`. Look at the example code above if you need help doing so.


**설명:** [ Hint ]     
• import datetime 를 사용하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from datetime import datetime
now = datetime.now()

print '%02d/%02d/%04d %02d:%02d:%02d' % (now.month, now.day, now.year, now.hour, now.minute, now.second)
```

**설명:** [ Solution ]    
• Print 문의 %s 을 기능을 사용하여, 각 변수의 값을 대입한다.
{: .notice--info}


**결과**
```
11/27/2018 20:59:59
```    
