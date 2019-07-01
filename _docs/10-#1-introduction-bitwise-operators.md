---
# layout : rchive
title: "Introduction to Bitwise Operators"
permalink: /introduction-bitwise-operators/
excerpt: "We learn about Bitwise Syntax."
# last_modified_at: 2019-02-26T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    
  
<hr style="border: solid 1px #dddddd ;">    

LESSON    

Bitwise operations directly manipulate bits—patterns of 0s and 1s. Though they can be tricky to learn at first, their speed makes them a useful addition to any programmer's toolbox.

**설명:** [ 학습방향 ]     
이 장에서는 비트(bit) 0, 1 에 관한 것을 다룰 것이다.    
처음에는 배우기가 어렵지만, 익숙 해지면 코딩의 속도를 높여주니 공부해 보자.
{: .notice--info}  
     
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 1. Just a Little BIT     

Welcome to an intro level explanation of bitwise operations in Python!

Bitwise operations might seem a little esoteric and tricky at first, but you'll get the hang of them pretty quickly.

Bitwise operations are operations that directly manipulate bits. In all computers, numbers are represented with bits, a series of zeros and ones. In fact, pretty much everything in a computer is represented by bits. This course will introduce you to the basic bitwise operations and then show you what you can do with them.

Bitwise operators often tend to puzzle and mystify new programmers, so don't worry if you are a little bit confused at first. To be honest, you aren't really going to see bitwise operators in everyday programming. However, they do pop up from time to time, and when they do, you should have a general idea of what is going on.



**설명:** [ Learn ]     
• Ch1. Just a Little BIT 에서는 Bit 연산자를 학습한다.        
• Bit 연산자는 이해하기가 어렵고, 모호하지만, 익숙해지면 빠른 계산을 할수 있다.    
• Bit 연산자는 직접적으로 bit 를 조작하여 계산한다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* In the editor are the 6 basic bitwise operations. Click Run and see what the console prints out. All of them will be explained in due time!


**설명:** [ Instruction ]    
• 6 개의 bit 연산자를 실행후, 각각 어떻게 동작 되는지를 설명해 보자.
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
print 5 >> 4  # Right Shift
print 5 << 1  # Left Shift
print 8 & 5   # Bitwise AND
print 9 | 4   # Bitwise OR
print 12 ^ 42 # Bitwise XOR
print ~88     # Bitwise NOT

```

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• Bit 연산자는 6 종류가 있다.     
• 그런데, 어떻게 계산하는지 잘 이해가 되지 않을 것이다.    
• 다음장 부터 차근차근 학습하니, 두려워 말자.        
• 단, bit 연산자는 6 종류가 있다는것만 기억하고 있자.
{: .notice--info}


**결과**     
``` 
0
10
0
13
38
-89
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 2. Lesson I0: The Base 2 Number System    

When we count, we usually do it in base 10. That means that each place in a number can hold one of ten values, 0-9. In binary we count in base two, where each place can hold one of two values: 0 or 1. The counting pattern is the same as in base 10 except when you carry over to a new column, you have to carry over every time a place goes higher than one (as opposed to higher than 9 in base 10).

For example, the numbers one and zero are the same in base 10 and base 2. But in base 2, once you get to the number 2 you have to carry over the one, resulting in the representation "10". Adding one again results in "11" (3) and adding one again results in "100" (4).

Contrary to counting in base 10, where each decimal place represents a power of 10, each place in a binary number represents a power of two (or a bit). The rightmost bit is the 1's bit (two to the zero power), the next bit is the 2's bit (two to the first), then 4, 8, 16, 32, and so on.

The binary number '1010' is 10 in base 2 because the 8's bit and the 2's bit are "on":    

```
8's bit  4's bit  2's bit  1's bit
    1       0       1      0 
    8   +   0    +  2   +  0  = 10 
```        
In Python, you can write numbers in binary format by starting the number with 0b. When doing so, the numbers can be operated on like any other number!

 



**설명:** [ Learn ]     
• Ch2. Lesson I0: The Base 2 Number System 에서는 2 진수를 학습한다.       
• 우리는 10 진수를 사용한다.     
• 10 진수는 0 부터 9 까지의 수를 조합하여 사용한다.     
• 컴퓨터는 2 진수를 사용한다.    
• 2 진수는 0 부터 1 까지의 수를 조합하여 사용한다.    
• 10 진수는 9 에서 1 이 추가되면 자리수가 바뀌면서 10 이 된다.   
• 2 진수는 0b1 에서 0b1 이 추가되면 자리수가 바뀌면서 0b10 가 된다.   
• 2 진수는 각 자리에 값이 있으면 해당 값이 매겨진다.     
• 2 진수 0b1010 는 10 진수 10 이다. 
{: .notice--info}
     


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  Take a look at the examples in the editor. Really try to understand this pattern before moving on. Click Run when you're ready to continue.


**설명:** [ Instruction ]    
• Editor 화면에 있는 소스들이 어떤 패턴이 있는지 이해하여 보자.    
• Run 실행 후 계속 진행해 보자.
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
print 0b1,    #1
print 0b10,   #2
print 0b11,   #3
print 0b100,  #4
print 0b101,  #5
print 0b110,  #6
print 0b111   #7
print "******"
print 0b1 + 0b11
print 0b11 * 0b11
```

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 2 진수 자리수는 1, 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024,...늘어난다.    
• 1 번째 자리에 bit 값이 있으면  0b1      십진수 1 이다.     
• 2 번째 자리에 bit 값이 있으면  0b10     십진수 2 이다.     
• 1, 2 번째 자리에 bit 값이 있으면  0b11  십진수 3 이다.     
• 3 번째 자리에 bit 값이 있으면  0b100   십진수 4 이다.     
• 1, 3 번째 자리에 bit 값이 있으면  0b101  십진수 5 이다.     
• 2, 3 번째 자리에 bit 값이 있으면  0b110  십진수 6 이다.     
• 1,2,3번째 자리에 bit 값이 있으면  0b111  십진수 7 이다.     
• 이진수  0b1  +  0b11                 십진수 4 이다.     
• 이진수  0b11 *  0b11                 십진수 9 이다.     
{: .notice--info}


**결과**     
```
1 2 3 4 5 6 7
******
4
9
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 3. I Can Count to 1100!    

All right! Time to practice counting in binary.

To make sure you've got the hang of it, fill out the rest of the numbers all the way up to twelve. Please do not use the `str()` method or any other outside functions.

Here are a few numbers that will be good to know going forward -    
```python
2 ** 0 = 1
2 ** 1 = 2
2 ** 2 = 4
2 ** 3 = 8
2 ** 4 = 16
2 ** 5 = 32
2 ** 6 = 64
2 ** 7 = 128
2 ** 8 = 256
2 ** 9 = 512
2 ** 10 = 1024
```    
You may recognize these numbers. Do you have a 32 or 64 bit system? Does your computer have a 256GB hard drive? Computers think in binary! 



**설명:** [ Learn ]     
• Ch3. I Can Count to 1100! 에서는 2 진수를 학습한다.    
• 2 진수로 10 자리까지 있는 것을 12 자리까지 확대하여 채워 넣어 보자.    
• 값을 채워 넣어 보는걸로 2 진수를 이해해 보자.    
• 컴퓨터는 2 진수로 움직인다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

*  Fill out the rest of the numbers with their corresponding binary values up to twelve in the editor to the right, using the 0bxxx format.


**설명:** [ Instruction ]    
• Editor 화면에서 변수 twelve 에 값을 채워 넣어라.    
• 2 진수 형식은 ( 0bxxx ) 이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Feel free to peek back at the previous exercise if you're having trouble!


**설명:** [ Hint ]     
• 앞에서 배운것을 자유롭게 참조하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
one = 0b1
two = 0b10
three = 0b11
four = 0b100
five = 0b101
six  = 0b110
seven = 0b111
eight = 0b1000
nine = 0b1001
ten  = 0b1010
eleven = 0b1011
twelve = 0b1100
```

**설명:** [ Solution ]     
• 1 부터 12 자리의 2 진수를 나타낸 것이다.
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
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 4. The bin() Function   

Excellent! The biggest hurdle you have to jump over in order to understand bitwise operators is learning how to count in base 2. Hopefully the lesson should be easier for you from here on out.

There are Python functions that can aid you with bitwise operations. In order to print a number in its binary representation, you can use the bin() function. bin() takes an integer as input and returns the binary representation of that integer in a string. (Keep in mind that after using the bin function, you can no longer operate on the value like a number.)

You can also represent numbers in base 8 and base 16 using the oct() and hex() functions. (We won't be dealing with those here, however.)





**설명:** [ Learn ]      
• Ch4. The bin() Function 에서는 함수 bin() 를 학습한다.     
• Python 에는 bit 연산자를 지원하는 함수가 있다.    
• print 출력할때 2 진수로 재표현 해주는 것으로 함수 bin() 를 사용한다.    
• 함수 bin() 는 정수를 입력값으로 가진다. 그리고 2 진수를 반환해 준다.    
• print 출력할때, 2 진수로 보여주지만, 그 값은 실제로는 string(문자)이다.    
• 함수 bin() 과 비슷한 것으로 8진수( oct() ), 16진수( hex() )도 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* We've provided an example of the bin function in the editor. Go ahead and use `print` and `bin()` to print out the binary representations of the numbers 2 through 5, each on its own line. 


**설명:** [ Instruction ]    
• 함수 bin() 를 사용하여 정수 2 부터 5 까지를 출력하라.     
• 각 라인마다 출력하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the code on line 1 as a guide! You can use a separate `print` statement for each number, though a loop or range should work just as well.


**설명:** [ Hint ]     
• Editor 화면의 라인 1 을 참조하라.    
• Loop 또는 range 를 사용할 줄 알지만, print 문을 개별로 사용하라.  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print bin(1)
print bin(2)
print bin(3)
print bin(4)
print bin(5)
```

**설명:** [ Solution ]     
• 함수 bin(1) 은 정수 1 을 2 진수 0b1  로 바꿔준다.    
• 함수 bin(2) 은 정수 2 을 2 진수 0b10 로 바꿔준다.    
• 함수 bin(3) 은 정수 3 을 2 진수 0b11 로 바꿔준다.    
• 함수 bin(4) 은 정수 4 을 2 진수 0b110 로 바꿔준다.    
• 함수 bin(5) 은 정수 5 을 2 진수 0b101 로 바꿔준다.    
{: .notice--info}



**결과**     
``` 
0b1
0b10
0b11
0b100
0b101
```      
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 5. int()'s Second Parameter    

Python has an `int()` function that you've seen a bit of already. It can turn non-integer input into an integer, like this:      
```python
int("42")
# ==> 42
```    
What you might not know is that the int function actually has an optional second parameter.    
```python
int("110", 2)
# ==> 6
```    
When given a string containing a number and the base that number is in, the function will return the value of that number converted to base ten.



**설명:** [ Learn ]      
• Ch5. int()'s Second Parameter 에서는 함수 int() 사용법을 학습한다.    
• 함수 int() 는 입력값을 int 로 바꿔주는 함수이다.    
• 함수 int("42") 는 문자열 "42" 를 입력하면, 정수 42 가 반환된다.    
• 함수 int() 는 다른 옵션 기능도 있다.    
• 함수 int("110", 2) 는 2 진수 "110" 을 입력하고, 옵션값을 2 로 입력한다.    
• 함수 int() 는 입력값 2 진수 "110" 을 int(정수) 6 으로 반환한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* In the console are several different ways that you can use the int function's second parameter.On line 7, use int to print the base 10 equivalent of the binary number 11001001.     
     
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]     
• Editor 화면에는 몇개의 함수 int() 를 사용한 예제들이 있다.    
• 라인 7 에서, 2 진수 0b11001001 을 함수 int() 를 사용하여 10 진수로 변경후 출력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the examples on lines 1 – 4 as a guide!


**설명:** [ Hint ]     
• 라인 1 ~ 4 의 예제들을 참조하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print int("1", 2)
print int("10", 2)
print int("111", 2)
print int("0b100", 2)
print int(bin(5), 2)
# Print out the decimal equivalent of the binary 11001001.
print int("11001001", 2)
```

**설명:** [ Solution ]     
• 함수 int( "1", 2 )     
→ 2 진수 "1"  을  10 진수 1 로 변환 후 출력.    
• 함수 int( "10", 2 )    
→ 2 진수 "10" 을  10 진수 2 로 변환후 출력.    
• 함수 int( "111", 2 )    
→ 2 진수 "111" 을 10 진수 7 로 변환후 출력.    
• 함수 int( "0b100", 2 )    
→ 2 진수 "0b100" 을 10 진수 4 로 변환후 출력.    
• 함수 int( bin(5), 2 ) 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

→ 2 진수 "110"   을 10 진수 5 로 변환후 출력.    
• 함수 int( "11001001", 2 )    
→ 2 진수 "11001001" 을  10 진수 201 로 변환후 출력.
{: .notice--info}

**결과**     
``` 
1
2
7
4
5
201
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 6. Slide to the Left! Slide to the Right!    

The next two operations we are going to talk about are the **left** and **right** shift bitwise operators. These operators work by shifting the bits of a number over by a designated number of slots.

The block below shows how these operators work on the bit level. Note that in the diagram, the shift is always a positive integer:    
<br>
```python

# Left Bit Shift (<<)  
0b000001 << 2 == 0b000100 (1 << 2 = 4)
0b000101 << 3 == 0b101000 (5 << 3 = 40)       

# Right Bit Shift (>>)
0b0010100 >> 3 == 0b000010 (20 >> 3 = 2)
0b0000010 >> 2 == 0b000000 (2 >> 2 = 0)

```    
<br>
Shift operations are similar to rounding down after **dividing** and **multiplying** by 2 (respectively) for every time you shift, but it's often easier just to think of it as shifting all the 1s and 0s left or right by the specified number of slots.

Note that you can only do bitwise operations on an **integer** Trying to do them on strings or floats will result in nonsensical output!





**설명:** [ Learn ]     
• Ch6. Slide to the Left! Slide to the Right! 에서는 시프트 연산을 학습한다.    
• Bit 를 왼쪽으로 한칸 옮기면 2를 곱하는 효과가 있다.    
• Bit 를 오른족으로 한칸 옮기면 2로 나누는 효과가 있다.    
• Bit 연산자는 int(정수)만 가능하다.    
• 문자열, 실수 등은 아무런 반응이 없다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Shift the variable `shift_right` to the right twice (`>> 2`) and shift the variable `shift_left` to the left twice (`<< 2`). Try to guess what the printed output will be!


**설명:** [ Instruction ]    
• 변수 shift_right 에는 ( >> 2 ) 를 하라.( 오른쪽으로 2칸 시프트 )    
• 변수 shift_left  에는 ( << 2 ) 를 하라.( 왼쪽으로 2칸 시프트 )    
• 출력이 어떻게 될지 생각해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the example in the instructions above as a guide.


**설명:** [ Hint ]     
• 상단의 설명을 참조하자. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
shift_right = 0b1100
shift_left = 0b1

# Your code here!
shift_right = shift_right >> 2
shift_left = shift_left << 2

print bin(shift_right)
print bin(shift_left)
```

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 변수 shift_right 는 오른쪽으로 bit 를 2 칸 이동한후 저장한다.    
• 그 결과는 0b11 이다.(10 진수 3)    
• 십진수 12를 나누기 2 를 2 번 한 효과가 나타난다.    
• 변수 shift_left 는 왼쪽으로 bit 를 2 칸 이동한후 저장한다.    
• 그 결과는 0b100 이다.(10진수 4)    
• 십진수 1를 곱하기 2 를 2 번 한 효과가 나타난다.         
• 변수 shift_right, shift_left 를 출력한다.
{: .notice--info}



**결과**     
``` 
0b11
0b100
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 7. A BIT of This AND That    

The bitwise **AND (&)** operator compares two numbers on a bit level and returns a number where the bits of that number are turned on if the corresponding bits of both numbers are 1. For example:    

```python

     a:   00101010   42
     b:   00001111   15       
===================
 a & b:   00001010   10
```    

As you can see, the 2's bit and the 8's bit are the only bits that are on in both a and b, so a & b only contains those bits. Note that using the & operator can only result in a number that is less than or equal to the smaller of the two values.

So remember, for every given bit in a and b:    

```python
0 & 0 = 0
0 & 1 = 0
1 & 0 = 0
1 & 1 = 1
```    
Therefore,     
```python
0b111 (7) & 0b1010 (10) = 0b10
```    
which equals two.    


**설명:** [ Learn ]       
• Ch7. A BIT of This AND That 에서는 AND 비트 연산자를 학습한다.    
• 연산자 AND (&) 는 두개의 비교 할 a, b 가 모두 1 일때 1 을 반환한다.    
• a, b 중 하나라도 0 이면 0 을 반환한다.   
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* print out the result of calling `bin()` on 0b1110 & 0b101.

* See if you can guess what the output will be!


**설명:** [ Instruction ]    
• 함수 bin() 를 사용하여 2 진수 ( 0b110 & 0b101 ) 를 계산후 출력하라.         
• 출력 결과가 어떻게 되는지 확인하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
print ( bin ( a & b ) )
```

**설명:** [ Hint ]     
• 함수 bin() 안에 2 진수를 넣어라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print (bin(0b110 & 0b101))
```

**설명:** [ Solution ]     
• 함수 bin() 안에 단순히 2 진수만 넣는게 아니라, AND(&) 연산자도 넣어서 계산한다.    
• 먼저, 0b110 & 0b101 이 계산된 2 진수 0b100이 반환된다.    
• 함수 bin(0b100) 에 넣는다.    
• 그 결과를 출력한다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>


**결과**     
```
0b100 
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 8. A BIT of This OR That    

The bitwise **OR (|)** operator compares two numbers on a bit level and returns a number where the bits of that number are turned on if either of the corresponding bits of either number are 1. For example:     
```python
    a:  00101010  42
    b:  00001111  15       
================
a | b:  00101111  47
```    
Note that the bitwise | operator can only create results that are greater than or equal to the larger of the two integer inputs.    

So remember, for every given bit in a and b:    
```python
0 | 0 = 0
0 | 1 = 1 
1 | 0 = 1
1 | 1 = 1
```    
Meaning    
```python
110 (6) | 1010 (10) = 1110 (14)
```    


**설명:** [ Learn ]     
• Ch8. A BIT of This OR That 에서는 OR 비트 연산을 학습한다.    
• OR ( | ) 연산자는 두수 a, b 를 비교하여, 비트값이 하나라도 1 이면 값 1 을 반환한다.    
• 값 a, b 모두 0 이면 0 을 반환한다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* For practice, print out the result of using `OR(|)`on 0b1110 and 0b101 as a binary string.    
* Try to do it on your own without using the `OR(|)` operator if you can help it.


**설명:** [ Instruction ]    
• OR ( | ) 연산자를 사용하여 0b1110 과 0b101 을 계산하라.   
• OR ( | ) 연산자를 사용하지 않고 한번 해보세요.( And 연산자로 실행해 보아라. ) 
{: .notice--info}



<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* This is pretty similar to what you did in the previous exercise! You're just using `OR(|)` instead of `AND(&)`.


**설명:** [ Hint ]     
• AND( & ) 연사자 대신에 OR( | ) 연산자를 사용한다. 
{: .notice--info}


<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print bin(0b1110 | 0b101)
```

**설명:** [ Solution ]     
• 0b1110 과 0b101 을 OR ( | ) 연산자로 계산한다.    
• ( 0b1110 | 0b101 ) 을 계산하면 0b1011 이 된다.    
• 그 결과값을 2 진수 함수 bin() 을 호출후 출력한다.
{: .notice--info}



**결과**     
``` 
0b1111
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 9. This XOR That?    

The **XOR (^)** or **exclusive** or operator compares two numbers on a bit level and returns a number where the bits of that number are turned on if either of the corresponding bits of the two numbers are 1, but not both.    
```python
    a:  00101010   42
    b:  00001111   15       
================
a ^ b:  00100101   37
```    
Keep in mind that if a bit is off in both numbers, it stays off in the result. Note that XOR-ing a number with itself will always result in 0.    

So remember, for every given bit in a and b:    
```python
0 ^ 0 = 0
0 ^ 1 = 1
1 ^ 0 = 1
1 ^ 1 = 0
```    
Therefore:    
```python
 111 (7) ^ 1010 (10) = 1101 (13)
```    



**설명:** [ Learn ]     
• Ch9. This XOR That? 에서는 XOR 비트 연산을 학습한다.       
• XOR( ^ )는 두 수 a, b 의 값이 같으면 0 을 반환한다.    
• 두 수 a, b 중 하나라도 틀리면, 1 을 반환한다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* For practice, print the result of using `XOR(^)` on 0b1110 and 0b101 as a binary string. Try to do it on your own without using the `XOR(^)` operator. 


**설명:** [ Instruction ]    
• XOR( ^ ) 연산자를 사용하여 0b1110 과 0b101 을 계산하라.        
• XOR( ^ ) 연산자 없이 한번 시도해 보시오.( OR 연산자로 한번 해보라. )
{: .notice--info}



<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* This is pretty similar to what you did in the previous exercise! You're just using `XOR(^)` instead of `OR(|)`.


**설명:** [ Hint ]     
• 기존 소스에서 OR( | ) 대신에 XOR( ^ ) 를 넣으면 된다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print bin(0b1110 ^ 0b101)
```

**설명:** [ Solution ]     
• 0b1110 과 0b101 을 XOR( ^ ) 연산을 하면, 같은 자리의 숫자가 같으면 0을 반환한다.   
• ( 0b1110 ^ 0b101 ) 을 계산하면 0b1011 이 된다.     
• 그 결과값을 2 진수 함수 bin() 을 사용하여 출력한다.
{: .notice--info}



**결과**     
``` 
0b1011
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 10. See? This is NOT That Hard!    

The bitwise **NOT** operator **(~)** just flips all of the bits in a single number. What this actually means to the computer is actually very complicated, so we're not going to get into it. Just know that mathematically, this is equivalent to adding one to the number and then making it negative.

And with that, you've seen all of the basic bitwise operators! We'll see what we can do with these in the next section.



**설명:** [ Learn ]     
• Ch10. See? This is NOT That Hard! 에서는 NOT 비트 연산을 학습한다.       
• NOT ( ~ )은 반대 값을 출력한다.    
• 0 은 1 을 출력하고, 1 은 0 을 출력한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Click Run and observe what the console prints out.


**설명:** [ Instruction ]    
• 소스를 실행후 어떻게 출력되는지 살펴본다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]     
• skip   
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print ~1
print ~2
print ~3
print ~42
print ~123
```

**설명:** [ Solution ]     
• 1 의 2 진수는 0b01 이고, ~ 는 첫째 bit에 1 을 더한 값 0b10 이다.    
• 0b11 의 정수값은 2 이고, ~ 이기에 - 값을 붙인다. 즉 -2 이다.     
• 2 의 2 진수는 0b10 이고, ~ 는 첫째 bit에 1을 더한 값 0b11 이다.      
• 0b11 의 정수값은 3 이고, ~ 이기에 - 값을 붙인다. 즉 -3 이다.    
• 이와 같이 ~3 은 -4 가 출력된다.    
• ~42는 -43 이 출력된다.    
• ~123 은 -124 가 출력된다.
{: .notice--info}



**결과**     
``` 
-2
-3
-4
-43
-124
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 11. The Man Behind the Bit Mask    

A **bit mask** is just a variable that aids you with bitwise operations. A bit mask can help you turn specific bits on, turn others off, or just collect data from an integer about which bits are on or off.    
<br>
```python
num  = 0b1100
mask = 0b0100

desired = num & mask
if desired > 0:
  print "Bit was on"

```    
In the example above, we want to see if the third bit from the right is on.    

1. First, we first create a variable num containing the number 12, or 0b1100.
2. Next, we create a mask with the third bit on.
3. Then, we use a bitwise-and operation to see if the third bit from the right of num is on.
4. If desired is greater than zero, then the third bit of num must have been one.



**설명:** [ Learn ]     
• Ch11. The Man Behind the Bit Mask 에서는 비트 Mask 를 학습한다.    
• Bit mask는 bit 단위 연산을 돕기 위한 단순한 변수이다.     
• Bit mask는 특정 bit 의 값을 활성화 하는데 도움을 준다.    
• 우리는 우선 bit 가 1 이면 On(켜짐)이라 하고, 0 이면 Off(꺼짐)라 표현한다.    
• 특정 자리의 bit 만을 On(켜짐)하기 위해 사용되는 것을 bit mask 라 한다.    
• 변수 num 의 3번째 bit 만을 On(1)하기 위해 사용되는 것을 bit mask 라 한다.    
• 예제에서, 변수( num & mask )한 값이 0 보다 크려면, mask 값이 0b0100 이어야 한다.    
• 변수 desired 가 0 보다 크므로 "Bit was on" 출력된다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function, `check_bit4`, with one argument, `input`, an integer.

* It should check to see if the **4th bit** from the right is on.

* If the bit is on, return "on" (not print!)

* If the bit is off, return "off".

* Check the Hint for some examples!




**설명:** [ Instruction ]    
• 함수 check_bit4(input) 을 작성하라.        
• 함수는 입력한 2 진수의 4 번째 bit 값이 1 이면 "on" 을 반환한다.    
• 입력한 4 번째의 bit 값이 0 이면 "off" 를 반환한다.     
• 함수만 구현하고, 출력하는 함수 호출은 하지 않는다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Here are some examples:      

```python
check_bit4(0b1) # ==> "off"
check_bit4(0b11011) # ==> "on"
check_bit4(0b1010) # ==> "on"
```    
* You'll need to use a mask where all bits are off except for the fourth bit from the right.


**설명:** [ Hint ]    
• 입력한 4 번째 bit 값이 1 인지를 확인하는 함수를 작성하라. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def check_bit4(input):
  mask = 0b1000
  desired = input & mask
  if desired > 0:
    return "on"
  else:
    return "off"

#print check_bit4(0b1010)      
```

**설명:** [ Solution ]     
• 변수 ( mask = 0b1000 ) 의 4 번째 bit 만 1 인것을 만든다.    
• 입력받은 input 과 mask 값을 AND 연산을 한다.    
• mask 가 4 번째 bit 가 1 인 경우에만 정수값 8(0b1000)이상이 생성된다.    
• 그 결과값을 desired 에 저장한다.   
• desired 가 0 보다 큰 경우(4 번째 bit가 1 인 경우) on 을 반환한다.     
• desired 가 0 보다 작은 경우 off 를 반환한다.    
• 다음 예제와 같이 실행하여 입력값이 정상적으로 실행되는지 확인한다.    
• e.g. print check_bit4(0b1010)
{: .notice--info}



**결과**     
``` 
on
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 12. Turn It On    

You can also use masks to turn a bit in a number on using `|`. For example, let's say I want to make sure the rightmost bit of number a is turned on. I could do this:    
```python
a = 0b110 # 6
mask = 0b1 # 1
desired =  a | mask # 0b111, or 7
```    
Using the bitwise `OR(|)` operator will turn a corresponding bit on if it is off and leave it on if it is already on.

 

**설명:** [ Learn ]     
• Ch12. Turn It On 에서는 비트 Mask 연습을 학습한다.       
• OR ( | ) 연산자를 사용하여 bit mask 를 만들 수 있다.    
• OR ( | ) 연산자는 두 수의 계산값중 하나라도 1 이면 결과값이 1 이된다.    
• OR ( | ) bit mask 는 off 되어 있는 bit, 0 을 on, 즉 1 로 만들어 준다.    
• 이미 on, 즉, bit 값이 1 이어서 on 되어 있는것은 on 으로 유지한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* In the editor is a variable, `a`.    
* Use a bitmask and the value `a` in order to achieve a result where the * 3th bit from the right of `a` is turned on.     
* Be sure to print your answer as a `bin()` string! 


**설명:** [ Instruction ]    
• 변수 a 에 있는 3 번째 bit를 on(1) 시켜라.    
• 함수 bin() 을 사용하여 출력하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You should use `OR(|)` and the variable `a` with a mask where the third bit from the right, and only the third bit from the right, is on.    
* If you do not use `bin()` then you will see integer results    

**설명:** [ Hint ]     
• 변수 a 의 3 번째 bit 가 0 이든 1 이든 mask 를 사용하여 OR 연산자를 사용하여 무조건 1(on)이 되게 한다.    
• 결과값을 함수 bin() 을 사용하지 않으면 정수값이 출력된다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
a = 0b10111011

mask = 0b100
desired = a | mask
print bin(desired)

```

**설명:** [ Solution ]     
• 3 번째 bit 가 1 인 변수 mask = 0b100 을 만든다.        
• 변수 a 와 mask 를 OR ( | ) 연산을 한다.    
• 그 결과를 변수 desired 에 저장한다.    
• 변수 desired 를 bin(desired) 로 변환후 출력한다.
{: .notice--info}



**결과**     
``` 
0b10111111
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 13. Just Flip Out    

Using the **XOR (^)** operator is very useful for flipping bits. Using **^** on a bit with the number one will return a result where that bit is flipped.

For example, let's say I want to flip all of the bits in `a`.    
I might do this:    
```python
a = 0b110 # 6
mask = 0b111 # 7
desired =  a ^ mask # 0b1
```



**설명:** [ Learn ]     
• Ch13. Just Flip Out 에서는 XOR 을 활용한 비트 Mask 를 학습한다.    
• XOR ( ^ ) 연산자는 두 수가 같으면 0, 틀리면 1 을 반환한다.   
• 변수 a 에 mask = 0b111 을 XOR 연산해 주면, 두수가 같으면 0, 틀리면 1 을 반환한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* In the editor is the 8 bit variable `a`.     
* Use a bitmask and the value `a` in order to achieve a result where all of the bits in a are **flipped**.     
* Be sure to print your answer as a `bin()` string!


**설명:** [ Instruction ]    
• 변수 a 는 8 개의 bit 가 저장되어 있다.    
• 변수 a 의 값 모두를 반대로 만들어라.    
• 출력할때, 함수 bin() 를 사용하여라.   
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You'll need a mask the same length as a in which all of the bits are turned on (all set to 1).


**설명:** [ Hint ]     
• mask 값을 만들때 먼저 다음과 같은 절차로 진행해야 함.    
• 바꿔야할 변수에 저장되어 있는 2 진수의 갯수를 알아내야 한다.    
• 그 변수의 2 진수 값 길이만큼, 1 을 만들어야 한다.
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
a = 0b11101110

mask = 0b11111111
desired = a ^ mask

print bin(desired)
```

**설명:** [ Solution ]     
• 변수 a 의 2 진수 값 길이만큼 변수 mask 에 2 진수 1 을 채운다.    
• 변수 a 와 변수 mask 를 XOR ( ^ ) 계산한다.    
• bit 값이 같으면 0 , 틀리면 1 반환되므로, 현재 값의 반대값이 생성된다.        
• 계산 결과값을 변수 desired 에 저장한다.    
• 변수 desired 를 함수 bin(desired) 로 출력한다.     
• 함수 bin(desired)를 사용하지 않으면 정수로 출력된다.
{: .notice--info}


**결과**     
``` 
0b10001
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO BITWISE OPERATORS</font> 
### 14. Slip and Slide    

Finally, you can also use the **left shift** (<<) and **right shift** (>>) operators to slide masks into place.    
<br>
```python

a = 0b101 
# Tenth bit mask
mask = (0b1 << 9)  # One less than ten 
#0b1000000000
desired = a ^ mask
#0b0000000101
#0b1000000000
#----------------
#0b1000000101

```    
<br>
Let's say that I want to turn on the **10th bit** from the right of the integer `a`.    

Instead of writing out the entire number, we **slide a bit** over using the `<<` operator.    

We use 9 because we only need to slide the mask nine places over from the first bit to reach the tenth bit.    


**설명:** [ Learn ]     
• Ch14. Slip and Slide 에서는 시프트 연산자를 학습한다.    
• 변수 a 값의 10 번째 bit를 on(1) 로 만들려고 한다.    
• 변수 mask 의 값 ( 0b1 ) 을 ( << 9 ) 9 bit를 왼쪽으로 민다.     
• 즉, ( 0b1 ) 다음에 0 이 9 개가 온다. ( e.g. mask=0b1000000000 )    
• 10 번째 bit 에 1 이 오기 위해선, bit 를 옆으로 9 번 민다(slid).    
• 변수 a 의 10 번째 bit 를 on 하려면, XOR 연산을 한다. ( e.g. a ^ mask )        
• 두 변수의 비트가 같으면 0, 하나라도 틀리면 1 이 된다.    
• 변수 desired 값은 ( 0b1000000101 )이 된다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function called `flip_bit` that takes the inputs`(number, n)`.

* Flip the **nth** bit (with the ones bit being the first bit) and store it in `result`.

* Return the `result` of calling `bin(result)`. 


**설명:** [ Instruction ]    
• 함수 flip_bit(number, n) 를 작성하라.    
• 입력값 변수 number 에는 bit 값을 입력하라.        
• 입력값 변수 n 에는 몇번째를 반전 시킬것인지를 입력하라.        
• 반전시킨 결과를 변수 result 에 저장하라.    
• 그 결과를 함수 bin(result) 로 값을 출력하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the `<<` operator to move your mask into place and the `XOR(^)` operator to flip your desired bit.

* The base bit is 0b1 
* if you want 10th slide bit, you have to move `<<(10 -1)`
* No print and call the `flip_bit()` function

**설명:** [ Hint ]     
• ( << )  연산자를 사용하여, 원하는 곳까지 이동(slide) 시켜라.    
• 그리고 원하는 bit 를 반전 시키기 위하여 ( ^ ) 를 사용하여 연산하라.    
• 기본 bit 는 0b1 이다.    
• 0b1 을 10 번째 bit 로 옮기고 싶으면  `<< (10번째 -1)` 로 코딩해야 한다.    
• 함수 flip_bit() 를 호출후, 출력은 하지마라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
def flip_bit(number, n):
  bit_to_flip = 0b1 << (n -1)
  result = number ^ bit_to_flip
  return bin(result)


#print (flip_bit(2,3))
```

**설명:** [ Solution ]     
• 입력값 parameter 변수 number 에 옮길 정수값을 입력한다.    
• 입력값 parameter 변수 n 에 1 로 셋팅하길 원하는 bit 의 위치를 입력한다.    
• 비트 0b1 을 (n-1) 만큼 << 왼쪽 으로 보낸다.(3번째는 시프트 2를 해야 한다.)    
• 변수 bit_to_flip 에 시프트 된 결과값을 저장한다.    
• 변수 result 에 변수 number ^ bit_to_flip 를 XOR 연산을 한다.    
• e.g.       number : 0b10    
• e.g. bit_to_flip : 0b100    
• 두 변수의 XOR 계산값은 0b110 이다.    
• 변수 result 에 결과값 0b110 을 저장한다.    
• 변수 result 의 값은 정수이다.    
• 함수 bin(result) 를 사용하여 2 진수로 출력한다.         
• 임의로 해당 값을 출력해 본다. 정수 2 의 2 진수값 3 번째 비트에 1 이 셋팅되어 있다.
{: .notice--info}


**결과**     
``` 
0b110
```   



<br>
<br>    
<br>    