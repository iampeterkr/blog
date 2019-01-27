---
# layout : rchive
title: "File Input/Output"
permalink: /file-input-output/
excerpt: "We learn about File input/output Syntax."
last_modified_at: 2019-01-27T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
<hr style="border: solid 1px #dddddd ;">    
LESSON    

Now that you understand Python syntax and have been introduced to some Python best practices, let's apply what you've learned to a real-world application: writing data to a file.

**설명:** [ 학습방향 ]     
이 장에서는 Python 을 활용한 File 입출력 구조를 학습한다. 그 외 지금까지 배워온 Python 문법을 이해하고 연습 해보자.  
{: .notice--info}     
     
 <hr style="border: solid 1px #dddddd ;">

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 1. See It to Believe It    

Until now, the Python code you've been writing comes from one source and only goes to one place: you type it in at the keyboard and its results are displayed in the console. But what if you want to read information from a file on your computer, and/or write that information to another file?

This process is called file I/O (the "I/O" stands for "input/output"), and Python has a number of built-in functions that handle this for you.

Check out the code in the editor to the right. 



**설명:** [ Learn ]     
• 지금까지는 코딩을 edit 창에서 하고, 그 결과를 console에서 보여주었다.     
• 그런데, 실제에는 컴퓨터의 파일에서 정보를 읽어서 처리하고 그 결과를 파일에 저장하여 보여준다.    
• 이러한 처리 절차를 File I/O 라고 부른다.     
• Python에서는 이러한 File I/O를 관리하는 여러가지 내부 함수를 제공한다.    
• Edit 창에 있는 소스를 보고, 이해해 보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Click Run! You just wrote all the contents of `my_list` to a text file called `output.txt`. 


**설명:** [ Instruction ]    
• 리스트 my_list 의 내용들을 파일 output.txt 에 저장하는 것이다.    
• 실행 해보고, 어떻게 동작되는지 이해해 보자.    
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
my_list = [i ** 2 for i in range(1, 11)]
# Generates a list of squares of the numbers 1 - 10

f = open("output.txt", "w")

for item in my_list:
  f.write(str(item) + "\n")

f.close()
```

**설명:** [ Solution ]     
• 리스트 변수 my_list 에 list comphresion을 이용하여 1부터 10까지의 제곱근을 구한다.    
• 파일 output.txt 파일을 쓰기 모드로 연다. 그리고 그 주소를 변수 f 에 저장한다.       
• for 문을 통하여 리스트 my_list 값을 하나씩 추출하여, 파일 f 값에 저장한다.    
• for 문이 종료되면, 파일 f 를 종료한다.
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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 2. The open() Function     

Let's walk through the process of writing to a file one step at a time.

The first code that you saw executed in the previous exercise was this:
```python
f = open("output.txt", "w")
```

This told Python to open `output.txt` in "w" mode ("w" stands for "write"). We stored the result of this operation in a file object, `f`.

Doing this opens the file in write-mode and prepares Python to send data into the file.




**설명:** [ Learn ]    
• 파일을 쓴다는 것이 어떻게 진행되는지 하나하나씩 이해해 보자.    
• 첫번째로, 파일을 쓰기 위해서는 해당 파일을 열어야 한다.     
• Python 문법은 open 이라는 함수를 사용해서 연다.    
• open()는 2개의 parameter를 가진다.    
• 첫번째는 파일의 위치와 이름을 적는다.    
• 두번째는 파일을 어떻게 할지(e.g. 읽을지, 쓸지, 읽고/쓸지)를 결정한다.    
• 파일이 정상적으로 open 되면 그 object가 반환된다.    
• 그 반환값 object 값을 변수 f 에 저장한다.    
• 이후, 파일에 접근하는뎅, object f를 활용한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a variable, `my_file`, and set it equal to calling the `open()` function on `output.txt`.     
* In this case, pass "r+" as a second argument to the function so the file will allow you to read and write to it! (See the Hint for details.)  


**설명:** [ Instruction ]    
• 변수 my_file 을 만들어라.    
• 파일 output.txt 을 open() 함수를 사용하여 열고 반환받은 objec 값을 저장한다.    
• open("output.txt", "r+")을 할때, "r+" 모드로 오픈한다.    
• 모드 "r+" 는 읽고, 쓰기 모드이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can open files in any of the following modes:    

* write-only mode ("w")
* read-only mode ("r")
* read and write mode ("r+")
* append mode ("a"), which adds any new data you write to the file to the end of the file.


**설명:** [ Hint ]     
• File 모드 에 대해서 알아보자.    
• 쓰기만 가능 ("w")    
• 읽기만 가능 ("r)")     
• 일기, 쓰기 모두 가능 ("r+")    
• 덧붙이기 ("a")
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
my_file = open("output.txt", "r+")
```

**설명:** [ Solution ]    
• object my_file은 "output.txt" 파일을 "읽기/쓰기" 모드로 오픈한다. 
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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 3. Writing     

Good work! Now it's time to write some data to a new `.txt` file.

We added the list comprehension from the first exercise to the code in the editor. Our goal in this exercise will be to write each element of that list to a file called `output.txt`. The `output.txt` file that you write to will be created in your current folder - for simplicity, the folder has been hidden. `output.txt` will list each number on its own line.

We can write to a Python file like so:
```python
my_file.write("Data to be written")
```
The `.write()` method takes a string argument, so we'll need to do a few things here:

You must close the file. You do this simply by calling `my_file.close()` (we did this for you in the last exercise). If you don't close your file, Python won't write to it properly. From here on out, you gotta close your files! 



**설명:** [ Learn ]     
• output.txt 를 오픈하고, 반환된 값 object를 my_file 에 저장되어 있다.   
• 지금부터, 파일에 저장하기 위해선, object my_file을 통하여 저장한다.   
• .write()를 사용하여 my_file.write("Data to be written")    
• 파일을 다 사용하고, 마지막에는 my_file.close()를 호출하여, 정리한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Iterate over `my_list` to get each value.

* Use `my_file.write()` to write each value to a text file called, `output.txt`.

* Make sure to call `str()` on the iterating data so `.write()` will accept it.

* Make sure to add a newline (+ "\n") after each element to ensure each will appear on its own line.

* Use `my_file.close()` to close the file when you're done.

* Passing the exercise means that you successfully wrote `my_list` to `output.txt`!

 


**설명:** [ Instruction ]    
• my_list 에 있는 값을 반복적으로 추출한다.    
• my_file.write()를 사용하여, output.txt. 파일에 my_list 값의 내용을 저장한다.    
• 함수 `str()`을 사용하여 저장하라.    
• 저장할때, "\n"을 추가하여, 새로운 줄에 저장하도록 하라.    
• 마지막에 my_file.close()호출하여, 파일을 닫도록 한다.   
• my_list 값을 output.txt 에 정상적으로 저장되면 성공이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, the syntax for iterating over a list looks like this:

```python
for item in list:
  # Do something
```  

You should write to the file inside your iterator, but you should close the file outside your iterator—otherwise, you'll attempt to close the file after you write each line!

And the syntax for calling `str()` looks like this:
```python
str(42)
# => "42"
```

Make sure to add a newline (+ "\n") 

**설명:** [ Hint ]     
• for 문을 사용하여 저장한다.       
• for 문이 완료되고, 파일 close() 한다.    
• 숫자는 str()를 사용하여 문자열로 만든다.
• "\n"을 확실히 해라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
my_list = [i ** 2 for i in range(1, 11)]

my_file = open("output.txt", "w")

# Add your code below!
for value in my_list:
  my_file.write(str(value) + "\n")
  
my_file.close()
```

**설명:** [ Solution ]     
• for 문을 돌면서 아래 작업을 진행한다.
• 변수 value 에 my_list 값을 하나씩 추출한다.    
• value 값을 str()활용하여 문자열로 만든다.    
• value 끝에 "\n"을 추가한다.    
• object my_file에 value 값을 저장한다.
• for 문이 완료되면, my_file을 close() 한다. 
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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 4.



**설명:** [ Learn ]      
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 5. 



**설명:** [ Learn ]      
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 6. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 7. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 8. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 9. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 10. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 11. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 12. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 13.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 14. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 15.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 16. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 17.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 18.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 19.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
