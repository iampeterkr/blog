---
# layout : rchive
title: "Battleship!"
permalink: /battleship/
excerpt: "Let's practice what we have learned so far."
# last_modified_at: 2019-02-19T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    

<hr style="border: solid 1px #dddddd ;">    

LESSON    

In this lesson, we will make a simplified version of the classic board game Battleship! We'll use functions, lists, and conditionals to make our game.

**설명:** [ 학습방향 ]     
이 장에서는 고전 게임인 배틀쉽을 구현해 보자.    
게임을 구현하면서, 함수, 리스트, 조건절 등을 연습해 보자.
{: .notice--info}     
     


<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 1. Welcome to Battleship!    

In this project you will build a simplified, one-player version of the classic board game Battleship! In this version of the game, there will be a single ship hidden in a random location on a 5x5 grid. The player will have 10 guesses to try to sink the ship.

To build this game we will use our knowledge of lists, conditionals and functions in Python. When you're ready to get started, click Next to continue.

 



**설명:** [ Learn ]          
• 지금까지 배운것을 활용하여 1인용 게임 Battleship 을 만든다.    
• 이 게임은 10 번의 질문을 통하여 5 x 5 좌표 위에 숨어 있는 배의 위치를 찾는다.    
• 이 게임은 우리가 이미 배운 리스트와 함수를 활용하여 개발한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

* Click Next to get started with Battleship!


**설명:** [ Instruction ]          
• Run을 실행하고 Next를 눌러 시작한다. 
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
skip
```

**설명:** [ Solution ]          
• skip
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 2. Getting Our Feet Wet    

The first thing we need to do is to set up the game board. 



**설명:** [ Learn ]          
• 첫번째 미션은 게임판을 만든다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a variable `board` and set it equal to an empty list.


**설명:** [ Instruction ]          
• 리스트 board 를 만들고, 빈 리스트로 초기화 하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
lst=[]
```


**설명:** [ Hint ]          
• 리스트 변수 lst=[] 은 변수 lst 를 초기화 하는 것이다. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
board = []
```

**설명:** [ Solution ]          
• 변수 board = [] 를 빈 리스트로 초기화 하였다. 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 3. Make a List    

Good! Now we'll use a built-in Python function to generate our board, which we'll make into a 5 x 5 grid of all "O"s, for "ocean."    
```python
print ["O"] * 5
```    
will print out ['O', 'O', 'O', 'O', 'O'], which is the basis for a row of our board.    

We'll do this five times to make five rows. (Since we have to do this five times, it sounds like a loop might be in order.)





**설명:** [ Learn ]          
• Ch3. Make a List 에서는 리스트로 5 x 5 게임판을 만든다.     
• 바다에 "o"으로 채워진 5 x 5 판이 있다.    
• 이 판을 출력 해보면, 가로가 ["o", "o", "o", "o", "o"]인 게임판이다.     
• 우리는 이런 모양의 세로로 5개가 있는 리스트를 만들것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a 5 x 5 grid initialized to all 'O's and store it in board.     
* Use `range()` to loop 5 times.     
* Inside the loop, `.append()` a list containing 5 "O"s to board, just like in the example above.     
* Note that these are capital letter "O" and not zeros.    

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]          
• 리스트 board 를 만들어라.     
• board는 5 x 5 로 된 판이며, 값 "O" 으로 채워져 있다.    
• 내부 함수 range() 활용하여 5번 loop 반복하라.    
• loop 안에서는 메서드 .append() 를 이용하여 리스트 board 를 작성하라.    
• 리스트 board 에는 ["O","O","O","O","O"] 가 5개가 있는 싱글 리스트를 만들어라.     
• 주의 할것은 "O" 는 숫자가 아닌 영문 대문자 "O" 이다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* What if you use a for loop that does the appending in the `range (0,5)`?

```python
[
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O']
]
```    

**설명:** [ Hint ]          
• for 문과 내부 함수 range(0,5) 를 활용하여 위 모양과 같은 리스트를 만들어라. 
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
board = []
for i in range(5):
  board.append(['O'] * 5)
  
  
#print board
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• 내부 함수 range(5) 를 발생 시킨다.    
• for 문에서 ['O'] 를 5 번 곱하면, 싱글 리스트 ['O','O','O','O','O'] 이 만들어진다.   
• e.g. ['O'] * 5 -> ['O','O','O','O','O']     
• 위와 같은 작업을 5 번( e.g. range(5) ) 반복하여 아래와 같이 만든다.     
[     
    ['O','O','O','O','O'],     
    ['O','O','O','O','O'],     
    ['O','O','O','O','O'],     
    ['O','O','O','O','O'],     
    ['O','O','O','O','O']     
] 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 4. Check it Twice    

Great job! Now that we've built our board, let's show it off.

Throughout our game, we'll want to print the game board so that the player can see which locations they have already guessed. Regularly printing the board will also help us debug our program.

The easiest way to print the board would be to have Python display it for us using the print command. Let's give that a try and see what the results look like—is this a useful way to print our board for Battleship?





**설명:** [ Learn ]          
• Ch4. Check it Twice 에서는 print 문을 통하여 기본적인 Debug 하는 방법을 학습한다.    
• print 문을 통하여 리스트 board 의 상태를 확인할 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Use the print command to display the contents of the `board` list.


**설명:** [ Instruction ]          
• print 문을 사용하여, 리스트 board 의 상태를 출력하라.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>
    
* The syntax for printing a list is     

```python
print list_name.
```

**설명:** [ Hint ]          
• print 문을 사용하여 리스트 list_name 의 내용을 출력한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
board = []
for i in range(5):
  board.append(['O'] * 5)
  
  
print board
```

**설명:** [ Solution ]          
• 빈 리스트 board 를 초기화 한다.    
• 내부 함수 range(5) 를 활용하여 아래 작업을 5번 반복한다.    
• 메서드 .append(['O'] * 5) 를 리스트 board 에 추가한다.     
• print 문을 활용하여 리스트 board 가 어떤 상태인지 확인한다. 
{: .notice--info}



**결과** 
``` 
[['O', 'O', 'O', 'O', 'O'], ['O', 'O', 'O', 'O', 'O'], ['O', 'O', 'O', 'O', 'O'], ['O', 'O', 'O', 'O', 'O'], ['O', 'O', 'O', 'O', 'O']]
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 5. Custom Print    

Now we can see the contents of our list, but clearly it would be easier to play the game if we could print the board out like a grid with each row on its own line.

We can use the fact that our board is a list of lists to help us do this. Let's set up a for loop to go through each of the elements in the outer list (each of which is a row of our board) and print them.

<br>

**설명:** [ Learn ]          
• Ch5. Custom Print 에서는 print 문을 응용하는 연습을 한다.    
• print 문으로 리스트의 내용을 볼 수 있다.     
• 하지만, 더 편하게 볼수 있도록 고쳐 보자.    
• 한줄에 좌~악 하고 출력되니, board 판 같지가 않다.    
• 리스트가 5 X 5 모양으로 한줄씩 총 5줄이 보이는 형태로 수정하자. 
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* First, delete your existing `print` statement.

* Then, define a function named `print_board` with a single argument, `board_in`.

* Inside the function, write a for loop to iterates through each row in board and print it to the screen.

* Call your function with board to make sure it works.

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]          
• 먼저, print 문을 삭제 하라.    
• 라인 6 에서 함수 print_board(board_in) 를 정의후 작성하라.    
• 함수 print_board(board_in) 는 다음과 같이 동작한다.    
• for 루프를 반복한다.    
• for 문에서 리스트 board 값을 추출하여 변수 row 에 저장한다.    
• 변수 row 를 출력한다.    
• 함수 print_board(board) 를 호출하여 정상적으로 동작하는지 확인하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)        
* Remember that the syntax to declare a function is `def fun_name(parameters):`. The syntax for iterating through a list is `for x in list_name:`

<br>
**설명:** [ Hint ]         
• 함수는 다음 예제처럼 정의하여 사용한다.    
• e.g. def fun_name(parameters):    
• for문은 다음 예제처럼 사용한다.    
• e.g. for x in list_name:     
• 함수를 for 문 다음에 정의하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
board = []

for i in range(5):
  board.append(["O"] * 5)

def print_board(board_in):
  for row in board:
    print row
    
print_board(board)
```   
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• 빈 리스트 board 를 만든다.    
• 빈 리스트 board 에 ['O'] * 5 를 추가한다.    
• 함수 print_board(board_in) 을 정의한다.    
• 함수 print_board(board_in) 은 다음과 같이 동작한다.    
• for 문에서 리스트 board 의 값을 추출하여, 변수 row 에 저장한다.    
• 변수 row 를 출력한다.(for 문의 board 항목 만큼)    
• 함수 print_board(board) 를 호출한다.
{: .notice--info}



**결과** 
``` 
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 6.Printing Pretty    

We're getting pretty close to a playable board, but wouldn't it be nice to get rid of those quote marks and commas? We're storing our data as a list, but the player doesn't need to know that!    

```python
letters = ['a', 'b', 'c', 'd']
print " ".join(letters)
print "---".join(letters)
```    

1. In the example above, we create a list called `letters`.     
2. Then, we print a b c d. The `.join` method uses the string to combine the items in the list.    
3. Finally, we print a---b---c---d. We are calling the `.join` function on the "---" string.    

We want to turn each row into "O O O O O". 



**설명:** [ Learn ]    
• Ch6.Printing Pretty 에서는 메서드 .join() 를 사용법을 학습한다.    
• 리스트 board 를 다듬어 보자.    
• 리스트 letters = ['a', 'b', 'c', 'd'] 를 다음과 같이 실행하면,    
• e.g. " ".join(letters)     
• 리스트 letters 는 다음과 같이 바뀐다.    
• e.g. "a b c d"      
• 다른 예로, "---".join(letters) 를 실행하면,    
• 리스트 letters 는 다음과 같이 바뀐다.    
• e.g. "a---b---c"    
• 마지막으로, 메서드 .join() 기능을 사용하여 다음과 같이 바뀌도록 한다.    
• 리스트 board =[ 'O','O','O','O','O' ] -> [ O O O O O ]
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Inside your function, inside your for loop, use " " as the separator to `.join` the elements of each row.

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]          
• 함수 print board() 를 다음과 같이 동작되도록 작성하라.    
• for 문 안에서 메서드 .join() 을 사용하여라.    
• 리스트 row 항목값 의 구분자를 'O' -> O 모양이 되게 만들어라.    
• e.g. 'O','O','O','O','O' ->  O O O O O 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Your function should contain a for loop that iterates over each row in the board. For each row, it should    

```python
print " ".join(row)
```

**설명:** [ Hint ]          
• for 문에서 리스트 board 의 추출값을 변수 row 에 저장한다.    
• 이때, 변수 row 를 출력할때, " ".join(row) 를 사용하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
board = []

for i in range(5):
  board.append(["O"] * 5)

def print_board(board_in):
  for row in board:
    print " ".join(row)
    
print_board(board)
```

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Solution ]          
• 소스코드 print row 를 print " ".join(row) 로 변경했다.
{: .notice--info}

**결과** 
``` 
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O

```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 7. Hide...    

Excellent! Now, let's hide our battleship in a random location on the board.

Since we have a 2-dimensional list, we'll use two variables to store the ship's location, `ship_row` and `ship_col`.    

```python
from random import randint
coin = randint(0, 1)
dice = randint(1, 6)
```    

1. In the above example, we first import the `randint(low, high)` function from the random module.

2. Then, we generate either zero or one and store it in coin.
3. Finally, we generate a number from one to six inclusive.
Let's generate a `random_row` and `random_col` from zero to four!





**설명:** [ Learn ]          
• Ch7. Hide... 에서는 내부 함수 randinit() 를 학습한다.     
• 내부 함수 randint(low, high) 는 low 와 high 사이의 값을 random 으로 출력한다.    
• e.g. randint(0, 1) :  0 과 1 사이의 값을 random 으로 출력한다.     
• e.g. randint(1, 6) :  1 에서 6 사이의 값을 random 으로 출력 해준다.     
• 함수 random_row() 와 random_col() 에 0 부터 4 까지의 값이 random 으로 출력되게 한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define two new functions, `random_row` and `random_col`, that each take `board_in` as input.
<p style="page-break-before: always;"></p>
<br>

* These functions should return a random row index and a random column index from your board, respectively. Use `randint(0, len(board_in) - 1)`.

* Call each function on board.




**설명:** [ Instruction ]          
• 함수 random_row() 와 random_col() 을 정의하라.    
• 각 함수는 parameters 변수로 board_in 을 가진다.    
• 각 함수는 보드판 위의 가로/세로 index 값을 random으로 가진다.     
• 함수 randint(0, len(board_in) -1) 을 활용하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* While we could just call `randint(0, 4)`, we use `len(board) - 1` in case we want to change the board size later.


**설명:** [ Hint ]          
• 손쉽게 내부 함수 randint(0,4) 로 직접 값을 호출할 수 있다.    
• 하지만, 향후 board 사이즈가 커질때를 대비하여 확장성 있게 만든다.    
• 함수 randint(0, len(board)-1) 의 입력값을 ( len(board) - 1 ) 로 정의한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint 

board = []

for x in range(0, 5):
  board.append(["O"] * 5)

def print_board(board):
  for row in board:
    print " ".join(row)
```
<p style="page-break-before: always;"></p>
<br>

```python
# Add your code below!

def random_row(board):
  return randint(0, len(board) - 1)
    
def random_col(board):
  return randint(0, len(board) - 1)

random_row(board)
random_col(board)

```

**설명:** [ Solution ]          
• 함수 random_row(board) 를 정의한다.    
• 함수 random_rwo(board) 는 다음과 같이 동작한다.    
• 함수 randint(0, len(board)-1) 을 호출하여, 가로 index 값을 random 하게 산출한다.    
• 함수 random_col(board) 를 정의한다.    
• 함수 random_col(board) 는 다음과 같이 동작한다.    
• 함수 randint(0, len(board)-1) 을 호출하여, 세로 index 값을 random 하게 산출한다.     
• 리스트 board 의 값은 'O', 'O', 'O', 'O', 'O' 항목이 5 개 들어있다.    
• 이 리스트의 길이는 5 이다.     
• 함수 randint(0, len(5) -1) 는 randint(0, 4) 를 호출 하는것과 같다.    
• e.g. randint(0, 4) : 0 부터 4 사이의 숫자가 random 하게 출력된다.    
• 함수 random_row(board), random_col(board) 를 호출한다.
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 8. ...and Seek!    

Good job! For now, let's store coordinates for the ship in the variables `ship_row` and `ship_col`. Now you have a hidden battleship in your ocean! Let's write the code to allow the player to guess where it is.    

```python
number = raw_input("Enter a number: ")
if int(number) == 0:
  print "You entered 0"
```   

`raw_input` asks the user for input and returns it as a string. But we're going to want to use integers for our guesses! To do this, we'll wrap the `raw_inputs` with `int()` to convert the string to an integer.





**설명:** [ Learn ]          
• Ch8. ...and Seek! 에서는 내부 함수 int() 를 학습한다.    
• 변수 ship_row 와 ship_col 에 배에 대한 위치 정보(가로/세로)를 저장해 보자.    
• 리스트 board 를 바다라고 가정하자.     
• 당신의 배가 바다(board) 어딘가에 있다고 생각하자.    
• 함수 raw_input() 은 prompt 에서 문자를 입력 받을수 있는 함수이다.    
• 입력 받은 문자 값을 숫자로 바꿔야 한다. 이유는 board 의 좌표 index 값은 숫자이다.    
• 함수 int(number) 활용하여 문자열 number 를 숫자로 바꾼다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a new variable called `guess_row` and set it to `int(raw_input("Guess Row: "))`.

* Create a new variable called `guess_col` and set it to `int(raw_input("Guess Col: "))`.

* Click `Run` and then answer the prompts by typing in a number and pressing Enter (or Return on some computers).


<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]          
• 변수 guess_row 에 int(raw_input("Guess Row: ")) 을 대입하라.    
• e.g. guess_row=int(raw_input("Guess Row: "))     
• 변수 guess_col 에 int(raw_input("Guess Col: ")) 을 대입하라.    
• e.g. guess_col=int(raw_input("Guess Col: "))    
• Run  버튼을 눌러 실행후, prompt 에서 값을 입력하라.
{: .notice--info}



<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* The syntax for the input command with changing it to int is    

```python
var = int(raw_input("Prompt text"))
```

**설명:** [ Hint ]          
• 참조 : var = int(raw_input("Prompt text)) 
{: .notice--info}

<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint

board = []

for x in range(0,5):
  board.append(["O"] * 5)

def print_board(board):
  for row in board:
    print " ".join(row)

def random_row(board):
  return randint(0, len(board) - 1)

def random_col(board):
  return randint(0, len(board[0]) - 1)
```    
<p style="page-break-before: always;"></p>
<br>

```python
ship_row = random_row(board)
ship_col = random_col(board)

# Add your code below!
guess_row = int(raw_input("Guess Row: "))
guess_col = int(raw_input("Guess Col: "))
```

**설명:** [ Solution ]          
• 소스 : guess_row = int(raw_input("Guess Row: ")) 는 다음과 같이 동작한다.    
• e.g. "Guess Row: " 가 출력되어 문자열 입력받을 준비를 하고 있다.    
• e.g. 문자열을 입력하고 Enter를 치면, 그 문자열 값이 변수 guess_row 에 저장된다.    
• 소스 : guess_col = int(raw_input("Guess Col: ")) 는 다음과 같이 동작한다.    
• e.g. "Guess Col: " 가 출력되어 문자열 입력받을 준비를 하고 있다.    
• e.g. 문자열을 입력하고 Enter를 치면, 그 문자열 값이 변수 guess_col 에 저장된다.
{: .notice--info}



**결과** 
``` 
Guess Row: 3
Guess Col: 3
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 9. It's Not Cheating—It's Debugging!    

Awesome! Now we have a hidden battleship and a guess from our player. In the next few steps, we'll check the user's guess to see if they are correct.

While we're writing and debugging this part of the program, it will be helpful to know where that battleship is hidden. Let's add a print statement that displays the location of the hidden ship.

Of course, we'll remove this output when we're finished debugging since if we left it in, our game wouldn't be very challenging. :)



**설명:** [ Learn ]          
• Ch9. It's Not Cheating—It's Debugging! 에서는 기본적 디버깅을 학습한다.    
• battleship 게임은 오션(board)의 특정 좌표에 배를 숨겨 놓는다.    
• 이후, 질문으로 그 배가 어디 있는지 맞추는 game이다.    
• 프로그램 debugging을 위하여 배의 좌표를 print 로 출력하여 배의 위치를 확인한다.    
• 나중에, 배의 위치를 출력하는 부분을 삭제할 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Before the lines prompting the user for input:

* Print the value of ship_row.

* Print the value of ship_col.


**설명:** [ Instruction ]          
• 배의 위치를 맞추기 위한 입력값을 받기 전에, 배의 위치를 먼저 출력하라.    
• 배의 위치는 변수 ship_row , ship_col 에 저장되어 있다.   
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

```python
ship_row = random_row(board)
print (ship_row)
```

**설명:** [ Hint ]          
• 배의 위치 row 좌표를 random 하게 구하여 저장한다.    
• 변수 ship_row 를 출력한다. 
{: .notice--info}


<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint

board = []

for x in range(0, 5):
  board.append(["O"] * 5)

def print_board(board):
  for row in board:
    print " ".join(row)

def random_row(board):
  return randint(0, len(board) - 1)

def random_col(board):
  return randint(0, len(board[0]) - 1)

ship_row = random_row(board)
ship_col = random_col(board)
# Add your code below!
print ship_row
print ship_col

guess_row = int(raw_input("Guess Row: "))
guess_col = int(raw_input("Guess Col: "))
```

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• Prompt 에서 입력값을 받기 전에    
• 임의로 저장되어 있는 배의 좌표 변수 값을 출력한다.    
• 배의 좌표는 변수 ship_row , ship_col 에 저장되어 있다. 
{: .notice--info}



**결과** 
``` 
1
0
Guess Row: 2
Guess Col: 2
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 10. You win!   

Okay—now for the fun! We have the actual location of the ship and the player's guess so we can check to see if the player guessed right.

For a guess to be right, `guess_col` should be equal to `ship_col` and `guess_row` should be equal to `ship_row`.    

```python
if guess_col == 0 and guess_row == 0:
  print "Top-left corner."
```   

The example above is just a reminder about if statements.





**설명:** [ Learn ]         
• Ch10. You win! 에서는 if 절을 사용하는 방법을 학습한다.      
• 배의 위치가 random 으로 정해지고, 참여자가 위치를 맞추면 게임이 끝난다.    
• 참여자가 승리하는 조건은 다음과 같다.    
• e.g. if guess_col == ship_col and guess_row == ship_row    
• if 절을 사용하여 비교하는 부분을 공부해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On line 29, add an if to check if `guess_row` equals `ship_row` and `guess_col` equals `ship_col`.

* If that is the case, please print out "Congratulations! You sank my battleship!"

* When you run this code, be sure to enter integer guesses in the panel where it asks for "Guess Row" and then "Guess Col".

<p style="page-break-before: always;"></p>
<br>



**설명:** [ Instruction ]          
• Editor 화면의 29 라인에서, if 문을 추가한다.    
• if 문은 (guess_row == ship_row) and (guess_col == ship_col) 비교한다.    
• if 조건문을 만족하면, *Congratulations! You sank my battleship!* 을 출력한다.     
• 이 프로그램을 실행하면, prompt 에 Guess Row 와 Guess Col 을 질문한다.    
• 예상 되는 배의 위치의 row, col 숫자 값을 입력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
if g_col == s_col and g_row == s_row:
  print "Your right."
```

**설명:** [ Hint ]          
• if 문을 사용하여 입력값과 배의 좌표 값을 비교한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint

board = []

for x in range(0, 5):
  board.append(["O"] * 5)

def print_board(board):
  for row in board:
    print " ".join(row)

print_board(board)
```    
<p style="page-break-before: always;"></p>
<br>

```python
def random_row(board):
  return randint(0, len(board) - 1)

def random_col(board):
  return randint(0, len(board[0]) - 1)

ship_row = random_row(board)
ship_col = random_col(board)
guess_row = int(raw_input("Guess Row: "))
guess_col = int(raw_input("Guess Col: "))

print ship_row
print ship_col

# Write your code below!
if guess_row == ship_row and guess_col == ship_col:
  print "Congratulations! You sank my battleship!"

```

**설명:** [ Solution ]         
• if 문을 사용하여 배의 좌표와, 플레이어가 예상하여 입력한 값이 일치하는지 비교한다.    
• 일치하면 플레이어가 게임을 승리하는 것이다.    
• 플레이어가 배의 좌표를 먼저 알면 안되기에,     
• 변수 ship_row, ship_col는 입력이 끝나고, 마지막에 출력하게 위치를 바꿨다.
{: .notice--info}



**결과** 
``` 
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O
Guess Row: 1
Guess Col: 1
3
3
-------------------------
```    
<p style="page-break-before: always;"></p>
<br>

```
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O
2
0
Guess Row: 2
Guess Col: 0
Congratulations! You sank my battleship!

```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 11. Danger, Will Robinson!!    

Great! Of course, the player isn't going to guess right all the time, so we also need to handle the case where the guess is wrong.
```python
print board[2][3]
```
The example above prints out "O", the element in the 3rd row and 4th column.

<br>

**설명:** [ Learn ]          
• Ch11. Danger, Will Robinson!! 에서는 else 문을 학습한다.   
• 항상, 한번에 맞출수는 없기에, 못 맞추었을 경우도 생각해야 한다.    
• ( print board[2][3] )은 좌표가 3번째, 4번째를 위치를 가리킨다.
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Add an else under the if we wrote in the previous step.

* Print out "You missed my battleship!"

* Set the list element at guess_row, guess_col to "X".

* As the last line in your else statement, call print_board(board) again so you can see the "X".     
* Make sure to enter a col and row that is on the board!


<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]          
• if 문 밑의 else 문에 *You missed my battleship!* 을 작성하라.    
• 리스트 board 의 guess_row, guess_col 좌표에 해당하는 곳에 문자 X 를 저장하라.     
• e.g. board[1][2] = "X"    
• print_board(board) 를 다시 호출하라.    
• 해당 좌표에 문자 "O" 대신에 문자 X 가 저장되어 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* To specify a single element in a 2-dimensional list, you need to give two indices. The syntax is: list_name[i][j], where i is an index in the outer list and j is an index in the inner list.


**설명:** [ Hint ]          
• 2차원 리스트를 만들어서 사용하라.     
• 2차원 리스트는 list_name[i][j] 로 만든다.    
• i 는 바깥 index, j는 내부 index 가리킨다.    
• e.g.  list_name = [ [1,2], [3,4], [5,6] ] => list_name[1,1] = 4 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint

board = []

for x in range(0, 5):
  board.append(["O"] * 5)

def print_board(board):
  for row in board:
    print " ".join(row)

print_board(board)
```
<p style="page-break-before: always;"></p>

```python
def random_row(board):
  return randint(0, len(board) - 1)

def random_col(board):
  return randint(0, len(board[0]) - 1)

ship_row = random_row(board)
ship_col = random_col(board)
print ship_row
print ship_col
guess_row = int(raw_input("Guess Row: "))
guess_col = int(raw_input("Guess Col: "))

# Write your code below!
if guess_row == ship_row and guess_col == ship_col:
  print "Congratulations! You sank my battleship!"  
else:
  print "You missed my battleship!"
  board[guess_row][guess_col] = "X"
  print_board(board)

```

**설명:** [ Solution ]          
• 플레이어가 배의 위치를 못 맞췄을 경우를 대비하여, else 문을 작성한다.    
• else 문에서는 못 맞춘 좌표 board[guess_row][guess_col]="X" 표시한다.    
• 전체 board 를 한번 보여준다.     
• "X" 를 넣는 이유는, 이미 틀린 좌표는 더 이상 입력 하지 않도록 유도하기 위해서이다. 
{: .notice--info}


**결과** 
``` 
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O
4
2
Guess Row: 1
Guess Col: 1
You missed my battleship!
O O O O O
O X O O O
O O O O O
O O O O O
O O O O O
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 12. Bad Aim    

Great job! Now we can handle both correct and incorrect guesses from the user. But now let’s think a little bit more about the "miss" condition.

1. They can enter a guess that's off the board.
2. They can guess a spot they’ve already guessed.
3. They can just miss the ship.    

We'll add these tests inside our else condition. Let's build the first case now!

```python
if x not in range(8) or \
   y not in range(3):
  print "Outside the range"
```
The example above checks if either x or y are outside those ranges. The `\` character just continues the if statement onto the next line.




**설명:** [ Learn ]          
• Ch12. Bad Aim  에서는 if/else 의 예외 처리를 강화하는 방법을 학습한다.    
• 좀더 치밀한게 프로그램을 다듬어 보자.     
• 프로그램에서 실수할 요소가 다음과 같이 있다.     
• ① board 보다 더 큰 값을 입력 할 경우     
• ② 이미 추측한 값을 입력할 경우     
• ③ 배의 틀린 위치 값을 예측한 경우     
• 상단의 소스는 입력값 변수 x 가 8 보다 크면, 입력 범위를 알려주는 소스이다.    
• 문자 `\` 는 소스가 다음 라인에 있지만, 이전과 계속 이어진다는 것을 알려주는 표시이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

* Add a new if statement that is nested under the else.

* Like the example above, it should check if `guess_row` is not in range(5) or `guess_col` is not in range(5).

* If that is the case, print out "Oops, that's not even in the ocean."    
* After your new if statement, add an else that contains your existing handler for an incorrect guess.     
* Don't forget to indent the code!

<br>
**설명:** [ Instruction ]          
• else 문의 내부에 추가로 if 문을 넣는다.    
• 추가한 if 문은 다음과 같은 기능을 한다.    
• 변수 guess_row 와 guess_col 의 범위가 5 를 넘지 않도록 한다.    
• 내부 함수 range(5) 를 사용하라.    
• 만약 입력값이 범위 5 를 넘으면 다음 메시지를 출력한다.    
• 메시지 : *Oops, that's not even in the ocean.*    
• 추가 if 문과 쌍이 되는 추가 else 문을 추가하라.    
• 추가 if 문과, 추가 else 문은 들여 쓰기를 조심하라. 
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* The valid values for guess_row are 0 to rows - 1 and the valid values for guess_col are 0 to cols - 1. You will need to build up a complex Boolean expression of the form:    

```python
if guess_row not in range(your_desired_range) or guess_col not in range(your_desired_range):
  # do something
```


**설명:** [ Hint ]          
• 변수 guess_row , guess_col 의 값은 0 부터 rows -1 , cols -1 이다.      
• e.g. rows : 5 -> 0, 1, 2, 3, 4    
• if 문에서 범위에 포함되고 안되고는 ( not in )을 사용한다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint

board = []

for x in range(0, 5):
  board.append(["O"] * 5)

def print_board(board):
  for row in board:
    print " ".join(row)

print_board(board)

def random_row(board):
  return randint(0, len(board) - 1)

def random_col(board):
  return randint(0, len(board[0]) - 1)

ship_row = random_row(board)
ship_col = random_col(board)
print ship_row
print ship_col
guess_row = int(raw_input("Guess Row: "))
guess_col = int(raw_input("Guess Col: "))

# Write your code below!
if guess_row == ship_row and guess_col == ship_col:
  print "Congratulations! You sank my battleship!"   
else:
  if guess_row not in range(5) or \
    guess_col not in range(5):
    print "Oops, that's not even in the ocean."
  else:
    print "You missed my battleship!"
    board[guess_row][guess_col] = "X"
  print_board(board)

```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]          
• else 문에서는 추가 if/else 문을 표현한다.    
• 추가 if 문을 사용하여, 가로, 세로 입력한 값이 5 개 범위 내인지를 점검한다.    
• 5 개의 범위를 벗어 났으면 print 문으로 알려준다.    
• 5 개 범위 안에는 있지만, 배의 위치를 맞추지 못했으면, 다음 2 가지 동작을 한다.    
• 첫번째, *You missed my battleship!* 출력한다.    
• 두번째, 플레이어가 입력한 좌표에 문자열 값 X 를 대입한다.     
• 프로그램의 말미에는 현재 board 의 최종 좌표를 보여준다.
{: .notice--info}



**결과** 
``` 
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O
2
2
Guess Row: 1
Guess Col: 1
You missed my battleship!
O O O O O
O X O O O
O O O O O
O O O O O
O O O O O
----------------
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O
3
3
Guess Row: 6
Guess Col: 6
Oops, that's not even in the ocean.
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 13. Not Again!  

Great! Now let's handle the second type of incorrect guess: the player guesses a location that was already guessed. How will we know that a location was previously guessed?    

```python
print board[guess_row][guess_col]
```    

The example above will print an 'X' if already guessed or an 'O' otherwise.





**설명:** [ Learn ]          
• Ch13. Not Again! 에서는 elif 를 학습한다.     
• 이미 틀렸던, 좌표를 다시 입력하면, 이미 입력 했다는것을 어떻게 알 수 있을까?    
• print board[guess_row][guess_col] 의 반환값은 문자열 X 이거나 O 이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Add an elif to see if the guessed location already has an 'X' in it.

* If it has, print "You guessed that one already."


**설명:** [ Instruction ]          
• 추가 if 문 밑에 elif 문을 추가하라.    
• elif 문의 기능은 다음과 같이 동작한다.    
• 입력받은 좌표가 기존에 입력했던 좌표 X 인지를 비교하라.    
• 좌표에 X 가 있으면 다음 메시지를 출력하라.    
• 메시지 : *You guessed that one alrady.*
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember to use two equal signs (`==`) when you're checking for equality.


**설명:** [ Hint ]          
• 연사자 ( == ) 는 비교 할때 양쪽의 값이 같다는 뜻이다.    
• if 문에서 연산자 ( == ) 를 활용한다. 
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint

board = []

for x in range(0, 5):
  board.append(["O"] * 5)

def print_board(board):
  for row in board:
    print " ".join(row)

print_board(board)

def random_row(board):
  return randint(0, len(board) - 1)

def random_col(board):
  return randint(0, len(board[0]) - 1)

ship_row = random_row(board)
ship_col = random_col(board)
print ship_row
print ship_col
guess_row = int(raw_input("Guess Row: "))
guess_col = int(raw_input("Guess Col: "))
```
```python
# Write your code below!
if guess_row == ship_row and guess_col == ship_col:
  print "Congratulations! You sank my battleship!"   
else:
  if guess_row not in range(5) or \
    guess_col not in range(5):
    print "Oops, that's not even in the ocean."
  elif (board[guess_row][guess_col] == 'X'):
    print "You guessed that one already."
  else:
    print "You missed my battleship!"
    board[guess_row][guess_col] = "X"
  print_board(board)

```

**설명:** [ Solution ]          
• elif 문에서 리스트 board[guess_row][guess_col] == "X" 인지 확인한다.    
• 이미 X 값이 존재하면 *You guessed that one already.* 를 출력한다.
{: .notice--info}


**결과** 
``` 
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O
3
0
Guess Row: 4
Guess Col: 4
You missed my battleship!
O O O O O
O O O O O
O O O O O
O O O O O
O O O O X
# 다음에 4,4를 입력 하면 이미 입력한 값이라고 출력 될 것이다.  
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 14. Test Run    

Congratulations! Now you should have a game of Battleship! that is fully functional for one guess.

Make sure you play it a couple of times and try different kinds of incorrect guesses. This is a great time to stop and do some serious debugging.

In the next step, we'll move on and look at how to give the user 4 guesses to find the battleship.



**설명:** [ Learn ]         
• Ch14. Test Run 에서는 프로그램 UAT(단위 테스트)를 학습한다.    
• 여러번 실행해 보고, 입력해 보자.     
• 그리고 문법적으로 또는 내용적으로 이상이 없는지 점검한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Thoroughly test your game.    
* Make sure you try a variety of different guesses and look for any errors in the syntax or logic of your program.


**설명:** [ Instruction ]          
• 여러번 실행해서 문법적 오류나 소스의 로직에 이상이 없는지 확인한다.     
• 소스가 어떻게 동작 되는지를 확인한다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
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
from random import randint

board = []

for x in range(0, 5):
  board.append(["O"] * 5)

def print_board(board):
  for row in board:
    print " ".join(row)

print_board(board)

def random_row(board):
  return randint(0, len(board) - 1)

def random_col(board):
  return randint(0, len(board[0]) - 1)

ship_row = random_row(board)
ship_col = random_col(board)
print ship_row
print ship_col

```
<p style="page-break-before: always;"></p>
<br>

```python
guess_row = int(raw_input("Guess Row: "))
guess_col = int(raw_input("Guess Col: "))

# Write your code below!
if guess_row == ship_row and guess_col == ship_col:
  print "Congratulations! You sank my battleship!"   
else:
  if guess_row not in range(5) or \
    guess_col not in range(5):
    print "Oops, that's not even in the ocean."
  elif (board[guess_row][guess_col] == 'X'):
    print "You guessed that one already."
  else:
    print "You missed my battleship!"
    board[guess_row][guess_col] = "X"
  print_board(board)

```

**설명:** [ Solution ]          
• skip 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 15. Play It, Sam    

You can successfully make one guess in Battleship! But we’d like our game to allow the player to make up to 4 guesses before they lose.    
```python
for turn in range(4):
  # Make a guess
  # Test that guess
```     
We can use a for loop to iterate through a range. Each iteration will be a turn.





**설명:** [ Learn ]          
• Ch15. Play It, Sam 에서는 입력을 4 번까지만 허용하는 기능을 추가한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Add a for loop that repeats the guessing and checking part of your game for 4 turns, like the example above.

* At the beginning of each iteration, `print "Turn"`, `turn + 1` to let the player know what turn they are on.

* Indent everything that should be repeated.


**설명:** [ Instruction ]          
• 질문 기회를 4 번까지 가능한 for 문을 추가하라.    
• for 문의 끝에는 몇 번 시도 했는지를 표시해 주는 print 문을 만들어라.    
• e.g. print ( "Turn :", turn+1)     
• for 문 안쪽에 들여 쓰여진 모든 소스는 반복된다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Don't forget to indent the code!


**설명:** [ Hint ]          
• for 문의 블럭안 내용은 모두 반복된다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint

board = []

for x in range(0, 5):
  board.append(["O"] * 5)

def print_board(board):
  for row in board:
    print " ".join(row)

print_board(board)

def random_row(board):
  return randint(0, len(board) - 1)

def random_col(board):
  return randint(0, len(board[0]) - 1)

ship_row = random_row(board)
ship_col = random_col(board)
print ship_row
print ship_col

```
<p style="page-break-before: always;"></p>
<br>

```python

# Everything from here on should be in your for loop
# don't forget to properly indent!
for turn in range(4):
  print "Turn", turn + 1
  guess_row = int(raw_input("Guess Row: "))
  guess_col = int(raw_input("Guess Col: "))

  if guess_row == ship_row and guess_col == ship_col:
    print "Congratulations! You sank my battleship!"   
  else:
    if guess_row not in range(5) or \
      guess_col not in range(5):
      print "Oops, that's not even in the ocean."
    elif board[guess_row][guess_col] == "X":
      print( "You guessed that one already." )
    else:
      print "You missed my battleship!"
      board[guess_row][guess_col] = "X"
    print_board(board)
```

**설명:** [ Solutin ]      
• for 문에서 4번 반복 하는것은 다음과 같이 작성한다.    
• e.g. for turn in range(4):    
• for 문으로 둘러 쌓여진(들여 쓰진) 소스는 4번 반복된다.
{: .notice--info}


**결과** 
``` 
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O
1
0
Turn 1
Guess Row: 1
Guess Col: 1
You missed my battleship!
O O O O O
O X O O O
O O O O O
O O O O O
O O O O O
```
<p style="page-break-before: always;"></p>
<br>

```
Turn 2
Guess Row: 2
Guess Col: 2
You missed my battleship!
O O O O O
O X O O O
O O X O O
O O O O O
O O O O O
```    

``` 
Turn 3
Guess Row: 3
Guess Col: 4
You missed my battleship!
O O O O O
O X O O O
O O X O O
O O O O X
O O O O O
Turn 4
Guess Row: 5
Guess Col: 5
Oops, that's not even in the ocean.
O O O O O
O X O O O
O O X O O
O O O O X
O O O O O

```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 16. Game Over    

If someone runs out of guesses without winning right now, the game just exits. It would be nice to let them know why.

Since we only want this message to display if the user guesses wrong on their last turn, we need to think carefully about where to put it.

We’ll want to put it under the else that accounts for misses
We’ll want to print the message no matter what the cause of the miss
Since our turn variable starts at 0 and goes to 3, we will want to end the game when turn equals 3.




**설명:** [ Learn ]         
• Ch16. Game Over 에서는 if 문을 사용하여 게임을 종료하는 방법을 학습한다.    
• 플레이어가 4번 만에 배의 위치를 맞추지 못하면 게임은 끝난다.    
• 게임이 끝났으면, 끝났다고 알려주면 좋을 것이다.         
• 소스의 어느 위치에 이 기능을 넣어야 할지를 고민하라.     
• 3 번의 기회가 주어지고, 그 안에 맞추지 못하면, 끝났다고 알려주기를 원한다.    
• 어느 위치가 좋을지 고민하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Add an if statement that checks to see if the user is out of guesses.

* Put it under the else that accounts for misses.
* Put it after the if/elif/else statements that check for the reason the player missed. We want "Game Over" to print regardless of the reason.
* If turn equals 3, print "Game Over".


<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]          
• 3번 틀리면 게임을 끝나는 부분을 어디에 넣을지 생각하라.    
• 첫째, 3번 틀렸는지를 비교하는 if/elif/else 문 밑에 추가하라.    
• 둘째, 실패 했을때 실행되는 else 문 안에 위치한다.    
• 셋째, 플레이어가 못 맞췄는 else 문 안에 위치한다.   
• 마지막으로, 변수 turn == 3 이면, *Game Over* 를 출력한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Your new if should go under the else that handles all of the incorrect guesses, but outside of any of the nested conditions. This is because it doesn't matter why the guess is wrong; after 4 wrong guesses, the game is over.




**설명:** [ Hint ]          
• 새로 추가되는 if 문은 3번 틀렸는지를 점검한다.     
• 기존 if/elif/else 에는 속하지 않는다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint

board = []

for x in range(0, 5):
  board.append(["O"] * 5)

def print_board(board):
  for row in board:
    print " ".join(row)

print_board(board)

```
<p style="page-break-before: always;"></p>
<br>

```python

def random_row(board):
  return randint(0, len(board) - 1)

def random_col(board):
  return randint(0, len(board[0]) - 1)

ship_row = random_row(board)
ship_col = random_col(board)

print ship_row
print ship_col

# Everything from here on should be in your for loop
# don't forget to properly indent!
for turn in range(4):
  print "Turn", turn + 1
  guess_row = int(raw_input("Guess Row: "))
  guess_col = int(raw_input("Guess Col: "))

  if guess_row == ship_row and guess_col == ship_col:
    print "Congratulations! You sank my battleship!"   
  else:
    if guess_row not in range(5) or \
      guess_col not in range(5):
      print "Oops, that's not even in the ocean."
    elif board[guess_row][guess_col] == "X":
      print( "You guessed that one already." )
    else:
      print "You missed my battleship!"
      board[guess_row][guess_col] = "X"
    if (turn == 3):
      print "Game Over"
    print_board(board)


```


**설명:** [ Solution ]          
• 추가 ( if (turn == 3): )는 따로 위치한다.    
• 기존 입력값과 좌표를 비교하는 if/elif/else 문과 연계하지 않았다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**결과** 
``` 
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O
4
2
Turn 1
Guess Row: 1
Guess Col: 1
You missed my battleship!
O O O O O
O X O O O
O O O O O
O O O O O
O O O O O
Turn 2
Guess Row: 1
Guess Col: 1
You guessed that one already.
O O O O O
O X O O O
O O O O O
O O O O O
O O O O O
Turn 3
Guess Row: 1
Guess Col: 1
You guessed that one already.
O O O O O
O X O O O
O O O O O
O O O O O
O O O O O
Turn 4
Guess Row: 1
Guess Col: 1
You guessed that one already.
Game Over
O O O O O
O X O O O
O O O O O
O O O O O
O O O O O
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font>     

### 17. A Real Win    

Almost there! We can play Battleship!, but you’ll notice that when you win, if you haven’t already guessed 4 times, the program asks you to enter another guess. What we’d rather have happen is for the program to end—it’s no fun guessing if you know you’ve already sunk the Battleship!

We can use the break command to get out of a for loop.





```
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O
2
0
Turn 1
Guess Row: 2
Guess Col: 0
Congratulations! You sank my battleship!
Turn 2
Guess Row: 
```

**설명:** [ Learn ]          
• Ch17. A Real Win 에서는 break 문을 학습한다.    
• 4번의 기회를 다 사용 하기 전에 플레이어가 이기면 멈춰야 한다.    
• 배의 좌표를 맞추어 이겼는데도, 계속 질문을 한다면 그 프로그램은 잘못 된 것이다.    
• 반복문을 강제로 빠져나가는 break 문을 사용한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    
<p style="page-break-before: always;"></p>
<br>

* Add a break under the win condition to end the loop after a win.


**설명:** [ Instruction ]          
• 배의 위치를 맞추는 블럭에서 break 문을 발생시켜서, loop를 빠져 나가라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Your break should go inside your outer if statement, right after your "Congratulations!" message.


**설명:** [ Hint ]         
• 작성 위치는 *Congratulations!!* 메시지 출력되는 다음 라인이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint

board = []

for x in range(0, 5):
  board.append(["O"] * 5)

def print_board(board):
  for row in board:
    print " ".join(row)

print_board(board)

def random_row(board):
  return randint(0, len(board) - 1)
```
<p style="page-break-before: always;"></p>
<br>

```python

def random_col(board):
  return randint(0, len(board[0]) - 1)

ship_row = random_row(board)
ship_col = random_col(board)
print ship_row
print ship_col

# Everything from here on should be in your for loop
# don't forget to properly indent!
for turn in range(4):
  print "Turn", turn + 1
  guess_row = int(raw_input("Guess Row: "))
  guess_col = int(raw_input("Guess Col: "))

  if guess_row == ship_row and guess_col == ship_col:
    print "Congratulations! You sank my battleship!"
    break
  else:
    if guess_row not in range(5) or \
      guess_col not in range(5):
      print "Oops, that's not even in the ocean."
    elif board[guess_row][guess_col] == "X":
      print( "You guessed that one already." )
    else:
      print "You missed my battleship!"
      board[guess_row][guess_col] = "X"
    if (turn == 3):
      print "Game Over"
    print_board(board)
```

**설명:** [ Solution ]          
• 컴파일러는 break 문을 만나면 for 문을 강제로 빠져나간다.  
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**결과** 
``` 
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O
2
4
Turn 1
Guess Row: 2
Guess Col: 4
Congratulations! You sank my battleship!
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 18. To Your Battle Stations!    

Congratulations! You have a fully functional Battleship game! Play it a couple of times and get your friends to try it out, too. (Don’t forget to go back and remove the debugging output that gives away the location of the battleship!)

You may want to take some time to clean up and document your code as well.





**설명:** [ Learn ]          
• Ch18. To Your Battle Stations! 에서는 디버깅을 해제 하는법을 학습한다.     
• 프로그램은 모두 완성되었다.    
• Debugging 을 위해서 배의 위치를 알려주는 print 문은 이제 삭제해야 한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* When you are done playing Battleship! and are ready to move on, click Run.


**설명:** [ Instruction ]          
• Debugging을 위하여 배의 위치를 알려주는 정보를 삭제하라.    
• 프로그램을 실행하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* whether remove or comment

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]         
• Debugging 부분을 삭제하거나, comment 처리한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
from random import randint

board = []

for x in range(0, 5):
  board.append(["O"] * 5)

def print_board(board):
  for row in board:
    print " ".join(row)

print_board(board)

def random_row(board):
  return randint(0, len(board) - 1)

def random_col(board):
  return randint(0, len(board[0]) - 1)

ship_row = random_row(board)
ship_col = random_col(board)
#print ship_row
#print ship_col

```
<p style="page-break-before: always;"></p>
<br>

```python

# Everything from here on should be in your for loop
# don't forget to properly indent!
for turn in range(4):
  print "Turn", turn + 1
  guess_row = int(raw_input("Guess Row: "))
  guess_col = int(raw_input("Guess Col: "))

  if guess_row == ship_row and guess_col == ship_col:
    print "Congratulations! You sank my battleship!"
    break
  else:
    if guess_row not in range(5) or \
      guess_col not in range(5):
      print "Oops, that's not even in the ocean."
    elif board[guess_row][guess_col] == "X":
      print( "You guessed that one already." )
    else:
      print "You missed my battleship!"
      board[guess_row][guess_col] = "X"
    if (turn == 3):
      print "Game Over"
    print_board(board)
```

**설명:** [ Solution ]          
• 이 소스에서는 배의 위치를 알려주는 소스를 삭제 하지 않고 comment 처리를 하였다. 
{: .notice--info}


**결과** 
``` 
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O
Turn 1
Guess Row: 1
Guess Col: 1
You missed my battleship!
```

<p style="page-break-before: always;"></p>
<br>

```
O O O O O
O X O O O
O O O O O
O O O O O
O O O O O
Turn 2
Guess Row: 1
Guess Col: 1
You guessed that one already.
O O O O O
O X O O O
O O O O O
O O O O O
O O O O O
```    
```
Turn 3
Guess Row: 1
Guess Col: 1
You guessed that one already.
O O O O O
O X O O O
O O O O O
O O O O O
O O O O O
Turn 4
Guess Row: 1
Guess Col: 1
You guessed that one already.
Game Over
O O O O O
O X O O O
O O O O O
O O O O O
O O O O O
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 19. Extra Credit    

You can also add on to your Battleship! program to make it more complex and fun to play. Here are some ideas for enhancements—maybe you can think of some more!

1. Make multiple battleships: you'll need to be careful because you need to make sure that you don’t place battleships on top of each other on the game board. You'll also want to make sure that you balance the size of the board with the number of ships so the game is still challenging and fun to play.

2. Make battleships of different sizes: this is trickier than it sounds. All the parts of the battleship need to be vertically or horizontally touching and you’ll need to make sure you don’t accidentally place part of a ship off the side of the board.

3. Make your game a two-player game.

4. Use functions to allow your game to have more features like rematches, statistics and more!

Some of these options will be easier after we cover loops in the next lesson. Think about coming back to Battleship! after a few more lessons and see what other changes you can make!





**설명:** [ Learn ]    
• Ch19. Extra Credit 에서는 프로그램을 확장하는 방법을 학습한다.    
• 배틀쉽 게임을 더 확장할수 있다.     
① 배틀쉽을 여러대를 보드에 넣어서 찾을 수 있다.    
② 배틀쉽 board 사이즈를 더 크게 확장 할 수 있다.    
③ 플레이어가 1인용이 아니라, 여러명이 할수 있게 만들 수 있다.    
④ 게임의 특징을 rematch 기능을 넣어 보다 다채롭게 만들수 있다.    
• 한번 도전해 봐라. 당신은 이제 전문 게임 프로그래머가 되었다.    
{: .notice--info}

