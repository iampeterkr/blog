---
# layout : rchive
title: "File Input/Output"
permalink: /file-input-output/
excerpt: "We learn about File input/output Syntax."
# last_modified_at: 2019-03-05T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    


<hr style="border: solid 1px #dddddd ;">    
LESSON    

Now that you understand Python syntax and have been introduced to some Python best practices, let's apply what you've learned to a real-world application: writing data to a file.

**설명:** [ 학습방향 ]     
이 장에서는 Python 을 활용한 File 입/출력 구조를 학습한다.    
그 외 지금까지 배워온 Python 문법을 이해하고 연습한다.  
{: .notice--info}     
     
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 1. See It to Believe It    

Until now, the Python code you've been writing comes from one source and only goes to one place: you type it in at the keyboard and its results are displayed in the console. But what if you want to read information from a file on your computer, and/or write that information to another file?

This process is called file I/O (the "I/O" stands for "input/output"), and Python has a number of built-in functions that handle this for you.

Check out the code in the editor to the right. 



**설명:** [ Learn ]   
• Ch1. See It to Believe It 에서는 File I/O 를 학습한다.      
• 지금까지는 코딩을 editor 화면에서 하고, 그 결과를 console 에서 보여주었다.     
• 실상은 컴퓨터가 파일에서 정보를 읽어서 처리후 그 결과를 파일에 저장하여 보여준다.    
• 이러한 파일 처리 절차를 File I/O 라고 부른다.     
• Python에서는 이러한 File I/O를 관리하는 여러가지 내부 함수를 제공한다.    
• Editor 화면에 있는 소스를 보고, 이해해 보자.
{: .notice--info}


<p style="page-break-before: always;"></p>
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


<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 리스트 my_list 에 list comphresion을 이용하여 1부터 10까지의 제곱을 구한다.    
• 파일 output.txt 파일을 쓰기 모드로 연다.  
• 그리고 그 주소를 변수 f 에 저장한다.       
• for 문을 통하여 리스트 my_list 값을 하나씩 추출하여, 변수 f 에 값을 저장한다.    
• for 문이 종료되면, 변수 f 를 종료한다. 
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
• Ch2. The open() Function 에서는 파일 함수 open() 을 학습한다.    
• 파일을 쓴다는 것이 어떻게 진행되는지 하나하나씩 이해해 보자.    
• 첫번째로, 파일을 쓰기 위해서는 해당 파일을 열어야 한다.     
• Python 문법은 open 이라는 함수를 사용해서 연다.    
• 함수 open() 은 2개의 parameter를 가진다.    
• 첫번째 매개변수는 파일의 위치와 이름을 적는다.    
• 두번째 매개변수는 파일을 어떻게 할지(e.g. 읽을지, 쓸지, 읽고/쓸지)를 결정한다.    
• 파일이 정상적으로 open 되면 그 File object 가 반환된다.    
• 그 반환값 File object 값을 변수 f 에 저장한다.    
• 이후, 파일에 접근할때, File object f 를 사용한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a variable, `my_file`, and set it equal to calling the `open()` function on `output.txt`.     
* In this case, pass "r+" as a second argument to the function so the file will allow you to read and write to it! (See the Hint for details.)  

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]    
• 변수 my_file 을 작성하라.    
• 파일 output.txt 을 open() 함수를 사용하여 오픈한다.    
• 반환받은 File object 값을 저장한다.    
• 함수 open("output.txt", "r+")을 할때, r+ 모드로 오픈한다.    
• 모드 ( r+ ) 는 읽고, 쓰기 모드이다.
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
• 쓰기만 가능 ( "w" )    
• 읽기만 가능 ( "r" )     
• 읽기, 쓰기 모두 가능 ( "r+" )    
• 덧붙이기 ( "a" )
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
my_file = open("output.txt", "r+")
```

**설명:** [ Solution ]    
• File object my_file 은 output.txt 파일을 읽기/쓰기 모드로 오픈한다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**결과**     
```
#skip 
```      
<p style="page-break-before: always;"></p>
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
• Ch3. Writing 에서는 쓰기를 학습한다.        
• 파일 output.txt 를 오픈하고, 반환된 값 object를 my_file 에 저장되어 있다.   
• 지금부터, 파일에 저장하기 위해선, File object my_file 을 통하여 저장한다.   
• 메서드 .write() 를 사용하여, 다음과 같이 문자열을 저장한다.    
• e.g.  my_file.write("Data to be written")    
• 파일을 모두 사용한 후, 마지막에는 my_file.close() 를 호출하여, 정리한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

* Iterate over `my_list` to get each value.

* Use `my_file.write()` to write each value to a text file called, `output.txt`.

* Make sure to call `str()` on the iterating data so `.write()` will accept it.

* Make sure to add a newline (+ "\n") after each element to ensure each will appear on its own line.

* Use `my_file.close()` to close the file when you're done.

* Passing the exercise means that you successfully wrote `my_list` to `output.txt`!

 


**설명:** [ Instruction ]    
• File object my_list 에 있는 값을 반복적으로 추출한다.    
• my_file.write() 를 사용하여, output.txt. 파일에 my_list 값의 내용을 저장한다.    
• 함수 str() 을 사용하여 저장하라.    
• 저장할때, ( \n ) 을 추가하여, 새로운 줄에 저장하라.    
• 마지막에 my_file.close() 호출하여, 파일을 닫아라.   
• File object my_list 값을 output.txt 에 정상적으로 저장되면 성공이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, the syntax for iterating over a list looks like this:    

```python
for item in list:
  # Do something
```  

* You should write to the file inside your iterator, but you should close the file outside your iterator—otherwise, you'll attempt to close the file after you write each line!    

* And the syntax for calling `str()` looks like this:    

```python
str(42)
# => "42"
```    

* Make sure to add a newline (+ "\n")     

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]     
• for 문을 사용하여 저장한다.       
• for 문이 완료되고, 파일 close() 한다.    
• 숫자는 함수 str() 을 사용하여 문자열로 만든다.    
• NewLine ( \n ) 을 확실히 하라.
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
• 변수 value 값을 함수 str() 을 활용하여 문자열로 만든다.     
• 변수 value 끝에 ( \n ) 을 추가한다.    
• File object my_file 에 value 값을 저장한다.    
• for 문이 완료되면, my_file 을 close() 한다.
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
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 4. Reading     

Excellent! You're a pro.    

Finally, we want to know how to read from our `output.txt` file. As you might expect, we do this with the `read()` function, like so:    
```python
print my_file.read()
```



**설명:** [ Learn ]     
• Ch4. Reading 에서는 파일을 읽는 방법을 학습한다.     
• 파일 output.txt 을 읽기 위해서는 File object my_file에 read() 함수를 사용한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Declare a variable, `my_file`, and set it equal to the file object returned by calling `open()` with both `"output.txt"` and `"r"`.

* Next, print the result of using `.read()` on `my_file`, like the example above.

* Make sure to `.close()` your file when you're done with it! All kinds of doom will happen if you don't.

 


**설명:** [ Instruction ]    
• my_file = open("output.txt", "r") 을 정의하라.    
• File object my_file 을 메서드 .read() 를 사용하여 읽어라. 그리고 출력하라.  
• 파일을 사용후에는 File object my_file 을 메서드 .close() 로 닫아라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, the syntax for opening a file looks like this:    

```python
variable = open("filename", "mode")
```

**설명:** [ Hint ]     
• 파일을 오픈하는 방법을 참조하자.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
my_file = open("output.txt", "r")
print my_file.read()
my_file.close()
```

**설명:** [ Solution ]     
• 파일 output.txt 를 read 모드로 오픈하여, File object my_file 에 저장한다.    
• File object my_file 을 읽어서 출력한다.   
• File object my_file 을 닫는다.
{: .notice--info}



**결과**     
``` 
1
4
9
16
25
36
49
64
81
100
```      
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 5. Reading Between the Lines    

What if we want to read from a file line by line, rather than pulling the entire file in at once. Thankfully, Python includes a `.readline()` method that does exactly that.

If you open a file and call `.readline()` on the file object, you'll get the first line of the file; subsequent calls to `.readline()` will return successive lines.



**설명:** [ Learn ]     
• Ch5. Reading Between the Lines 에서는 파일 함수 readline() 을 학습한다.      
• Python에서 .readline() 을 사용하면, 파일을 한번에 한 줄씩 읽을 수 있다.    
• 파일을 오픈후, 메서드 .readline() 을 사용하면 순차적으로 파일의 내용을 한 줄씩 읽는다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Declare a new variable `my_file` and store the result of calling `open()` on the "text.txt" file in "r"ead-only mode.    

* On three separate lines, print out the result of calling `my_file.readline()`.     

* See how it gets the next line each time?    

* Don't forget to `.close()` your file when you're done with it!    

 


**설명:** [ Instruction ]    
• 변수 my_file 에 파일 "text.txt" 을 읽기 모드로 오픈하라.    
• File object my_file.readline() 을 호출하여, 파일의 내용을 읽어 출력하라.    
• 한줄은 읽었는데, 다음줄은 어떻게 할지를 고민해 보라.   
• 파일을 다 사용후에는 꼭 메서드 .close() 로 닫아야 한다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, to open a file:      

```python
variable = open("filename", "mode")
```    

* To read from the file, you can just call `variable.readline()`.    
* Make sure to close your file once you're done reading from it!




**설명:** [ Hint ]     
• Python 문법중 다음 예제의 File I/O 문법을 상기한다.    
• e.g. variable = open("filename", "mode")     
• 파일을 한 줄씩 읽을때는 variable.readline() 를 사용한다.    
• 파일을 다 쓴 후에는 닫는 것을 잊지말라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
my_file = open("text.txt", "r")
print my_file.readline()
print my_file.readline()
print my_file.readline()
my_file.close()
```


**설명:** [ Solution ]     
• 파일 text.txt 을 read 모드로 오픈 후, File object my_file 에 저장한다.     
• File object my_file 에 readline() 으로 한 라인씩 출력한다.    
• File object my_file 을 close() 한다. 
{: .notice--info}



**결과**     
``` 
I'm the first line of the file!
I'm the second line.
Third line here, boss.
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 6. PSA: Buffering Data     

We keep telling you that you always need to close your files after you're done writing to them. Here's why!

During the I/O process, data is buffered: this means that it is held in a temporary location before being written to the file.

Python doesn't flush the buffer—that is, write data to the file—until it's sure you're done writing. One way to do this is to close the file. If you write to a file without closing, the data won't make it to the target file.



**설명:** [ Learn ]    
• Ch6. PSA: Buffering Data 에서는 버퍼링에 관하여 학습한다.     
• 파일 write 작업이 끝나면 항상 닫아야 한다.     
• 이유는, 파일 write I/O 작업하는 동안 데이타가 버퍼링에 남아 있기 때문이다.    
• 파일을 정상적으로 닫아야 실질적인 파일 저장이 된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out our extremely bad code in the editor.     
* Click Run—you'll note that our `read_file.read()` didn't read any data back!    

* Add a `write_file.close()` call after writing to the file but before reading it.    

* Add a `read_file.close()` call after the print `read_file.read()` line
Run the code again.    

* This time, you'll see the data come through!    

<p style="page-break-before: always;"></p>
<br>
  


**설명:** [ Instruction ]    
• Editor 화면에 있는 코드는 좋은 코드가 아니다.    
• print read_file.read() 소스에서 어떤 데이타도 읽지 못할 것이다.    
• 이유는 파일을 쓰고, .Close() 를 하지 않았다.    
• 파일을 write 한 후, 다음 라인에 아래와 같이 파일을 close 하는 것을 추가하라.     
• e.g. write_file.close()    
• 파일을 read 한 후, 다음 라인에 아래와 같이 파일을 close 하는 것을 추가하라.    
• e.g. read_file.close()
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
# Use a file handler to open a file for writing
write_file = open("text.txt", "w")

# Open the file for reading
read_file = open("text.txt", "r")

# Write to the file
write_file.write("Not closing files is VERY BAD.")

write_file.close()

# Try to read from the file
print read_file.read()

read_file.close()
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 파일을 write 한 후 더 이상 사용할 일이 없으면 해당 파일을 .close() 해야 한다.     
• 파일을 read 한 후 더 이상 사용할 일이 없으면 해당 파일을 .close() 해야 한다. 
{: .notice--info}



**결과**     
``` 
Not closing files is VERY BAD.
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 7. The 'with' and 'as' Keywords    

Programming is all about getting the computer to do the work. Is there a way to get Python to automatically close our files for us?

Of course there is. This is Python.

You may not know this, but file objects contain a special pair of built-in methods: `__enter__()` and `__exit__()`. The details aren't important, but what is important is that when a file object's `__exit__()` method is invoked, it automatically closes the file. How do we invoke this method? With with and as.

The syntax looks like this:    
```python
with open("file", "mode") as variable:
  # Read or write to the file
```


**설명:** [ Learn ]     
• Ch7. The 'with' and 'as' Keywords 에서는 자동 close 함수를 학습한다.    
• Python 에서는 자동으로 파일을 종료 시켜 주는 기능이 있다.    
• 함수 `__enter__()`, `__exit__()` 을 사용하면 된다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the example in the editor.     
* Note that we don't explicitly `close()` our file, and remember that if we don't close a file, our data will get stuck in the buffer. Click Run!     
* Success! is written to a file called `text.txt`.     

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]    
• Editor 화면에 있는 내용을 실행후 살펴보라.    
• 메서드 .close() 를 하지 않았음에도 정상적으로 text.txt 파일에 저장이 되었다.
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
with open("text.txt", "w") as textfile:
  textfile.write("Success!")
```

**설명:** [ Solution ]     
• 메서드 .close() 가 없음에도 정상적으로 파일이 저장된다. 
{: .notice--info}



**결과**     
``` 
Success!
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 8. Try It Yourself    

It worked! Our Python program successfully wrote to text.txt.



**설명:** [ Learn ]      
• Ch8. Try It Yourself 에서는 자동 저장에 관하여 추가 학습한다.     
• 파일 text.txt 가 정상적으로 저장 되었다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Now you try: write any data you like to a file called `text.txt` using with...as. Give your file object the usual name: `my_file`.


**설명:** [ Instruction ]    
• 파일 text.txt 을 with...as 를 사용하여 아무 데이타를 저장하라.     
• File object 는 my_file 로 하여라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember your syntax:    

```python
with open("file","mode") as variable:
  # Read or write to the file
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]     
• with...as 문법을 기억하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
with open("text.txt", "w") as my_file:
  my_file.write("cheapter 8 ")
  
```

**설명:** [ Solution ]     
• 문법 with ... as 을 사용하여 파일을 오픈하여 저장하였다.    
• 메서드 .close() 를 사용하지 않았지만, 자동으로 저장되었다.
{: .notice--info}



**결과**     
``` 
cheapter 8 
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">FILE INPUT/OUTPUT</font> 
### 9. Case Closed?    

Finally, we'll want a way to test whether a file we've opened is closed. Sometimes we'll have a lot of file objects open, and if we're not careful, they won't all be closed. How can we test this?    

```python
f = open("bg.txt")
f.closed
# False
f.close()
f.closed
# True
```    
Python file objects have a closed attribute which is True when the file is closed and False otherwise.

By checking `file_object.closed`, we'll know whether our file is closed and can call `close()` on it if it's still open.





**설명:** [ Learn ]    
• Ch9. Case Closed? 에서는 파일 close 점검하는 법을 학습한다.    
• 파일이 닫혔는지 열렸는지를 확인해 주는 함수는 file_object.closed 이다.   
• file_object.closed 를 호출하여 False가 반환되면 아직 열려 있는 상태이다.    
• 반대로, True 이면 닫힌 상태이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Below your `with...as` code, do two things:

* Check `if` the `my_file` is not closed.    

* If that's the case, call `.close()` on it.    

<p style="page-break-before: always;"></p>
<br>

* (You don't need an else here, since your if statement should do nothing if closed is True.)

* After your `if` statement, print out the value of `my_file.closed` to make sure your file is really closed.
 


**설명:** [ Instruction ]    
• 문법 with ... as 밑에 두개의 코딩 작업을 하라.    
• 만약에 my_file 이 닫히지 않았으면, 임의로 닫아라.    
• 마지막 라인에 my_file.closed 값을 출력하여라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, if statements look like this:    


```python
if expression:
  # Do something
```    

**설명:** [ Hint ]     
• if 문을 사용하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
with open("text.txt", "w") as my_file:
  my_file.write("My Data!")
  
if not my_file.closed:
  my_file.close()

print my_file.closed
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• my_file.closed 호출하였다.    
• 만약 파일이 닫혀 있으면 False가 반환된다.    
• 현재 소스에서는 자동으로 닫히기에 my_file.closed 가 True가 반환된다.   
• `if not True` -> `if Fasle` 의미이다.  
• 즉, False, 열려 있으면 닫아라는 의미이다.     
• File object my_file는 이미 닫혀 있다.    
• 즉, my_file.closed 를 출력하면 True가 반환된다.
{: .notice--info}



**결과**     
``` 
True
```   

<br>
<br>    
<br>    