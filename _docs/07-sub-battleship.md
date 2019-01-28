---
# layout : rchive
title: "Battleship!"
permalink: /battleship/
excerpt: "Let's practice what we have learned so far."
last_modified_at: 2019-01-03T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    

<hr style="border: solid 1px #dddddd ;">    

LESSON    

In this lesson, we will make a simplified version of the classic board game Battleship! We'll use functions, lists, and conditionals to make our game.

**설명:** [ 학습방향 ]     
이 장에서는 고전 게임인 배틀쉽을 구현해 보자. 이 게임을 구현하면서, 함수, 리스트, 조건절 등을 연습해 보자.
{: .notice--info}     
     



 <hr style="border: solid 1px #dddddd ;">

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 1. Welcome to Battleship!    

In this project you will **build a simplified**, **one-player version of the classic board game Battleship**! In this version of the game, there will be a single ship hidden in a random location on a 5x5 grid. The player will have 10 guesses to try to sink the ship.

To build this game we will use our knowledge of lists, conditionals and functions in Python. When you're ready to get started, click Next to continue.

 



**설명:**     
지금가지 배운것을 활용하여 1인용 게임 'Battleship1'을 만들 것이다.  이 게임은 10번의 질문을 통하여 5x5 좌표 위에 숨어 있는 배의 위치를 찾아서 침돌 시키는 것이다. 이 게임은 우리가 이미 배운 리스트와 함수를 사용하여 개발 하것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Click Next to get started with Battleship!


**설명:**     
① Run을 실행하고 Next를 눌러 시작하자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
skip


**설명:**     
skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
skip
```

**설명:**     
skip
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 2. Getting Our Feet Wet    

The first thing we need to do is to set up the game board. 



**설명:**     
우리가 첫번째로 해야 할일은 게임 판을 만드는 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a variable **`board`** and set it equal to an empty list.


**설명:**     
①  리스트 **`board`**를 만들고, 빈 리스트로 초기화 해라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
lst=[]
```


**설명:**     
`lst=[]`은 변수 lst를 리스트로 초기화 하는 것이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
board = []
```

**설명:**     
변수 **`board = []`**를 빈 리스트로 초기화 하였다. 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 3. Make a List    

Good! Now we'll use a built-in Python function to generate our board, which we'll make into a **5 x 5** grid of **all "O"s, for "ocean."**
```python
print ["O"] * 5
```
will print out **['O', 'O', 'O', 'O', 'O']**, which is the basis for a row of our board.

We'll do this five times to make five rows. (Since we have to do this five times, it sounds like a loop might be in order.)





**설명:**     
바다에 "o"으로 채워진 5x5 판이 있다.  출력 해보면, 가로가 ["o", "o", "o", "o", "o"]인 판인 것이다. 우리는 이런 모양의 세로로 5개가 있는것을 만들 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a 5 x 5 grid initialized to all **'O's** and store it in board.

* Use **`range()`** to **loop 5 times**.
* Inside the loop, **`.append()`** a list **containing 5 "O"s** to board, just like in the example above.
* Note that these are capital letter **"O"** and **not zeros**.




**설명:**     
① 5 x 5 판에 "O"로 채워진 변수 리스트 **`board`**를 만들어라.     

• **`range()`** 활용하여 5번 loop 반복해라.     
•  loop 안에서는 **`.append()`**를 이용하여 리스트 변수 **`board`**에 ["O","O","O","O","O"]가 5개가 있는 싱글 리스트를 만들어라. 
• 주의 할것은 "O"는 숫자가 아닌 영문 대문자 "O" 이다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
What if you use a for loop that does the appending in the **`range (0,5)`**?

```python
[
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O']
]
```



**설명:**     
**`range(0,5)`**와 for 문을 활용하여 위 모양과 같은 리스트를 만들어라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
board = []
for i in range(5):
  board.append(['O'] * 5)
  
  
#print board
```

**설명:**     
**`['O'] * 5`**는 ['O','O','O','O','O']를 만드는 방법이다. 이를 for문으로 5번 loop를 돌려서 
`[
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O']
]`를 만든다. 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 4. Check it Twice    

Great job! Now that we've built our board, let's show it off.

Throughout our game, we'll want to print the game board so that the player can see which locations they have already guessed. Regularly printing the board will also help us debug our program.

The easiest way to print the board would be to have Python display it for us using the print command. Let's give that a try and see what the results look like—is this a useful way to print our board for Battleship?





**설명:**     
print문을 통하여 **`board`** 리스트의 상태가 어떤지를 알 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Use the print command to display the contents of the **`board`** list.


**설명:**     
① 리스트 **`board`**의 상태를 출력해 보자.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
The syntax for printing a list is 
```python
print list_name.
```

**설명:**     
리스를 출력하는 방법이다. 
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

**설명:**     
실행시켜 리스트 **`board`**가 어떤 상태인지를 확인한다. 
{: .notice--info}



**결과** 
``` 
[['O', 'O', 'O', 'O', 'O'], ['O', 'O', 'O', 'O', 'O'], ['O', 'O', 'O', 'O', 'O'], ['O', 'O', 'O', 'O', 'O'], ['O', 'O', 'O', 'O', 'O']]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 5. Custom Print    

Now we can see the contents of our list, but clearly it would be easier to play the game if we could print the board out like a grid with each row on its own line.

We can use the fact that our board is a list of lists to help us do this. Let's set up a for loop to go through each of the elements in the outer list (each of which is a row of our board) and print them.



**설명:**     
리스트의 내용을 볼수 있지만, 더 편하게 볼수 있도록 고쳐 보자. 한줄에 좌~악 하고 나오는게 아니라, 5 X 5 모양으로 한줄씩 총 5줄이 보이는 형태로 고쳐 보다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** First, delete your existing **`print`** statement.

* Then, define a function named **`print_board`** with a single argument, **`board_in`**.

* Inside the function, write a for loop to iterates through each row in board and print it to the screen.

* Call your function with board to make sure it works.



**설명:**     
① 먼저, print 문을 삭제 하라.    
* 6라인에서 함수 **`print_board(board_in)`** 작성하여라.  
* 내부 기능으로, for 루프를 돌면선, 입력받은  **`board`** 의 값들을 `row`로 끄집어내라. 그리고 `row`를 출력하라.    
* 함수**`print_board(board)`**를 호출하여 잘 돌아 가는 확인하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember that the syntax to declare a function is **`def fun_name(parameters):`**. The syntax for iterating through a list is **`for x in list_name:`**


**설명:**    
함수는 `def fun_name(parameters):`로 사용해야 하면, for문은 `for x in list_name:`으로 사용해야 한다. 
for 문 다음에 def 문을 정의해라. 
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

**설명:**     
**`board`**에 `['O','O','O','O','O']`를 저장하고,    
**`print_board`** 함수를 만든다.     
**`print_board(board)`**를 호출한다.  
{: .notice--info}



**결과** 
``` 
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
```

<br>
<br>    
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
1. In the example above, we create a list called **`letters`**.
2. Then, we print **a b c d**. The **`.join`** method uses the string to combine the items in the list.
3. Finally, we print **a---b---c---d**. We are calling the **`.join`** function on the **"---"** string.
We want to turn each row into **"O O O O O"**. 



**설명:**     
board를 좀더 다듬어 보자.    
`letters = ['a', 'b', 'c', 'd']`를 `" ".join(letters)`를 실행하면, `a b c d`로 출력된다. 여기에도 `"---".join(letters)`를 하면 `a---b---c`로 처리된다.    
우리는 `.join`기능을 사용하여 우리 board `'O','O','O','O','O'`를 `O O O O O`형태로 만들어 보자.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Inside your function, inside your **for loop**, use **" "** as the separator to **`.join`** the elements of each row.


**설명:**     
① 함수 `print board()`의 for 문 안에서 `.join`을 사용하여 `row` 리스트를 문자간의 구분자를 " "로 바꾸어라. 즉, `[ O O O O O ]`모양이 되게끔 만들어라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Your function should contain a **for loop** that iterates over **each row** in the board. For each row, it should
```python
print " ".join(row)
```

**설명:**     
함수 `print board`의 for 문을 돌면서 보더 속의 `row`를 `" ".join(row)`를 사용하여라.  
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

**설명:**     
`print row`를 `print " ".join(row)`로 변경한다. 
{: .notice--info}



**결과** 
``` 
O O O O O
O O O O O
O O O O O
O O O O O
O O O O O

```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 7. Hide...    

Excellent! Now, let's hide our battleship in a random location on the board.

Since we have a 2-dimensional list, we'll use two variables to store the ship's location, **`ship_row`** and **`ship_col`**.
```python
from random import randint
coin = randint(0, 1)
dice = randint(1, 6)
```
1. In the above example, we first import the **`randint(low, high)`** function **from the random module**.

2. Then, we **generate** either **zero or one** and store it in coin.
3. Finally, we **generate** a number from **one to six** inclusive.
Let's generate a **`random_row`** and **`random_col`** from **zero to four**!





**설명:**     
① 내재 함수 `randint(low, high)`는 `low`와 `high`사이의 값을 random으로 출력해준다.    
② `randint(0,1)`은 0과 1사이의 값을 random으로 출력 해준다.     
③ 마지막으로, `randint(1, 6)`은 1에서 6사이의 값을 random으로 출력 해준다.     
변수 `random_row`와 `random_col`에 0부터 4까지의 값을 넣어 보도록 하자.      
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define two new functions, **`random_row`** and **`random_col`**, that each take **`board_in`** as input.

These functions should return a **random row index** and a **random column index** from your board, respectively. Use **`randint(0, len(board_in) - 1)`**.

Call each function on board.




**설명:**     
① 함수 `random_row`와 `random_col`을 정의하고, 각 함수는 입력 값으로 `board_in`을 가진다. 각 함수는 보드의 random row index와 random colum index를 가진다. `randint(0, len(board_in) -1)`을 활용하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
While we could just call **`randint(0, 4)`**, we use **`len(board) - 1`** in case we want to change the board size later.


**설명:**     
`randint(0,4)`이라고 직접 값을 넣어 호출 할수 있지만, 향후 board 사이즈가 변할때를 대비하여 입력 값을  `len(board) -1`로 사용하면 미리 대비할 수 있다. 
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

# Add your code below!

def random_row(board):
  return randint(0, len(board) - 1)
    
def random_col(board):
  return randint(0, len(board) - 1)

random_row(board)
random_col(board)

```

**설명:**     
`random_row(board)`함수는 board의 값은 ['O', 'O', 'O', 'O', 'O'] 항목이 5개 들어 있는 리스트가 넘어온다. 이 리스트의 길이는 5이다.     
`randint(0, len(5) -1)`과 같기에, `randint(0, 4)`를 호출 하는것과 같다. 즉, 0부터 4사이의 숫자가 random하게 출력되는 것이다. 
`random_col(board)`도 동일하다.  
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 8. ...and Seek!    

Good job! For now, let's store coordinates for the ship in the variables **`ship_row`** and **`ship_col`**. Now you have a hidden battleship in your ocean! Let's write the code to allow the player to guess where it is.
```python
number = raw_input("Enter a number: ")
if int(number) == 0:
  print "You entered 0"
```  
**`raw_input`** asks the user for input and returns it as a string. But we're going to want to use integers for our guesses! To do this, we'll wrap the **`raw_inputs`** with **`int()`** to convert the string to an integer.





**설명:**     
변수 `ship_row`와 `ship_col`에 배에 대한 정보를 저장해 보자. 그리고 board를 오션 이라고 가정하고 당신의 배가 오션(board)에 숨겨보자.      
`raw_input` 함수는 문자를 입력 받을 수 있는 함수이다. 그런데, 우리는 입력값을 숫자로 인식해야 하기에 입력은 문자열로 입력 받지만, `int(number)`를 활용하여 숫자로 바꾸어 숫자값이 0인지를 확인한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a new variable called **`guess_row`** and set it to **`int(raw_input("Guess Row: "))`**.

Create a new variable called **`guess_col`** and set it to **`int(raw_input("Guess Col: "))`**.

Click **`Run`** and then answer the prompts by typing in a number and pressing Enter (or Return on some computers).




**설명:**     
① 변수 `guess_row`에 `int(raw_input("Guess Row: "))`을 대입하자. 예, `guess_row=int(raw_input("Guess Row: "))`     
변수 `guess_col`에 `int(raw_input("Guess Col: "))`을 대입하자. 예, `guess_col=int(raw_input("Guess Col: "))`    
`Run` 버튼을 눌러 실행해서 prompt 에 해당 값을 입력해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
The syntax for the input command with changing it to int is
```python
var = int(raw_input("Prompt text"))
```

**설명:**     
`var = int(raw_input("Prompt text))`를 참조하자. 
{: .notice--info}

<br>
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

ship_row = random_row(board)
ship_col = random_col(board)

# Add your code below!
guess_row = int(raw_input("Guess Row: "))
guess_col = int(raw_input("Guess Col: "))
```

**설명:**     
`guess_row = int(raw_input("Guess Row: "))`는 prompt에 "Guess Row: "에 문자열을 입력 받아 변수 `guess_row`에 저장하는 것이다.    
`guess_col = int(raw_input("Guess Col: "))`는 prompt에 "Guess Col: "에 문자열을 입력 받아 변수 `guess_col`에 저장하는 것이다. 
{: .notice--info}



**결과** 
``` 
Guess Row: 3
Guess Col: 3
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 9. It's Not Cheating—It's Debugging!    

Awesome! Now we have a hidden battleship and a guess from our player. In the next few steps, we'll check the user's guess to see if they are correct.

While we're writing and debugging this part of the program, it will be helpful to know where that battleship is hidden. Let's add a print statement that displays the location of the hidden ship.

Of course, we'll remove this output when we're finished debugging since if we left it in, our game wouldn't be very challenging. :)



**설명:**     
battleship을 오션(board)에 특정 좌표에 숨겨 놓고, 질문으로 그 배가 어디 있는지 찾아내는 game이다. 프로그램 debugging을 위하여 좌표를 우리는 출력하여 배위 위치를 확인해 보자. 물론 나중에는 배의 위치를 출력하는 부분을 삭제할 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Before the lines prompting the user for input:

* Print the value of ship_row.

* Print the value of ship_col.


**설명:**     
① 변수 `ship_row`, `ship_col` 값을 산출하고, prompt 실해되기 전에 변수 `ship_row`, `ship_col`을 출력하여라.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

```python
ship_row = random_row(board)
print (ship_row)
```

**설명:**     
배의 위치 row 좌료르 구하고, 그 변수 `ship_row`를 출력하라. 
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

**설명:**     
배의 좌표를 알수 있는 변수 `ship_row`, `ship_col`을 출력하여 배위 위치가 어디 있는지 확인한다. 
{: .notice--info}



**결과** 
``` 
1
0
Guess Row: 2
Guess Col: 2
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 10. You win!   

Okay—now for the fun! We have the actual location of the ship and the player's guess so we can check to see if the player guessed right.

For a guess to be right, **`guess_col`** should be equal to **`ship_col`** and **`guess_row`** should be equal to **`ship_row`**.

if guess_col == 0 and guess_row == 0:
  print "Top-left corner."
The example above is just a reminder about if statements.





**설명:**    
배의 위치가 random으로 만들어지고, 참여자가 위치를 맞추면 게임이 끝나는 것이다. 이것을 프로그램으로 풀이하면 `guess_col`이 `ship_col`과 값이 같고, `guess_row`가 `ship_row`와 값이 같으면, 참여자가 승리하는 것이다. if 절을 사용하여 비교하는 부분을 공부해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** On line 29, add an if to check if guess_row equals ship_row and guess_col equals ship_col.

If that is the case, please print out "Congratulations! You sank my battleship!"

When you run this code, be sure to enter integer guesses in the panel where it asks for "Guess Row" and then "Guess Col".




**설명:**     
① 29 라인에서, if문을 추가하여 `guess_row`와 `ship_row`같은지와 `guess_col`와 `ship_col`가 같은지를 추가한다.    
만약에 같으면 "Congratulations! You sank my battleship!" 을 출력한다.    
이 프로그램 실행하면, "Guess Row"와 "Guess Col"을 묻는다. 예상되는 위치의 row, col 숫자 값을 넣는 소스이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
if g_col == s_col and g_row == s_row:
  print "Your right."
```

**설명:**     
if 문을 사용하는 법을 잘 활용 하자. 
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
guess_row = int(raw_input("Guess Row: "))
guess_col = int(raw_input("Guess Col: "))

print ship_row
print ship_col

# Write your code below!
if guess_row == ship_row and guess_col == ship_col:
  print "Congratulations! You sank my battleship!"

```

**설명:**    
if 문을 사용하여 배의 좌표와, 플레이어가 예상하여 입력한 값이 일치하면 게임을 승리하는 것이다. 배의 좌표를 먼저 알면 안되기에, `ship_row`, `ship_col`는 입력하고 출력하게끔 위치를 바꿨다.   
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

<br>
<br>    
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



**설명:**     
항상, 한번에 맞출수는 없기에, 못 맞추었을 경우도 생각해야 한다. `print board[2][3]`은 좌표가 3번째, 4번째를 가리키는 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** **Add** an else under the if we wrote in the previous step.

Print out "You missed my battleship!"

**Set** the list element at guess_row, guess_col to **"X"**.

As the last line in your **else** statement, **call print_board(board)** again so you can see the **"X"**. Make sure to enter a col and row that is on the board!




**설명:**     
① if 문 밑의 else문에  "You missed my battleship!" 을 작성하라. 그리고 보드 리스트의  guess_row, guess_col 좌표에 문자 "X"를 저장하라. 그리고 else 문에 `print_board(board)`를 한번더 호출 하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
To specify a single element in a 2-dimensional list, you need to give two indices. The syntax is: list_name[i][j], where i is an index in the outer list and j is an index in the inner list.


**설명:**     
2차원 리스트를 만들어서 사용하라. 2차원 리스트는 `list_name[i][j]`로 만들고, i는 바깥 인덱스, j는 내부 인덱스를 이야기 한다. ( ex. [ [1,2], [3,4], [5,6] ]는 i = 2, j=1 )
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

**설명:**     
못 맞췄을 경우를 대비하여, else 문을 작성한다.    
못 맞춘 좌표를 `board[guess_row][guess_col]="X"`표시해 놓고, 전체 board를 한번 보여준다. 이는 이미 틀린 좌표는 더 이상 입력 하지 않도록 유도 하기 위해서이다. 
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

<br>
<br>    
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




**설명:**     
좀더 치밀한게 프로그램을 다듬어 보자. 프로그램에서 실수할 요소가 다음과 같이 있다.     
① board 보다 더 큰 값을 입력 할 경우    
② 이미 추측한 값을 입력할 경우     
③ 배의 틀린 위치 값을 예측한 경우     
상단의 소스는 입력값 `x`의 범위를 주어, 이 값을 벗어 나면 알려주는 예제 소스이다. 문자 `\`는 소스가 다음 라인에 있지만, 이전과 계속 이어진다는 것을 얼려주는 표시이다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Add a new if statement that is **nested under the else**.

Like the example above, it should check if **`guess_row`** is **not in range(5)** or **`guess_col`** is **not in range(5)**.

If that is the case, print out "Oops, that's not even in the ocean."

After your new if statement, add an else that contains your existing handler for an incorrect guess. Don't forget to **indent the code**!


**설명:**     
① 추가 if 문을 기존의 else 문 안에 추가하라. 
추가 if 문은 변수 `guess_row`와 `guess_col`의 범위가 5를 넘지 않도록 `range(5)`를 사용하라.    
만약 범위가 넘으면 "Oops, that's not even in the ocean." 을 출력하라.    
그리고 기존의 else 문을 추가 if 문과 연결되는 else 문으로 사용하라. 
추가 if문은 else 안에 구현하기에 들여 쓰기를 조심해라.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
The valid values for guess_row are 0 to rows - 1 and the valid values for guess_col are 0 to cols - 1. You will need to build up a complex Boolean expression of the form:
```python
if guess_row not in range(your_desired_range) or guess_col not in range(your_desired_range):
  # do something
```


**설명:**     
값을 인식할때, 변수 `guess_row`, `guess_col`에 들어 있는 값은 0부터 `rows -1`,`cols -1`이다.      
if 문에서 range가 포함되고 안되고는 `not in` 표현한다. 
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

**설명:**     
맞추지 못한 경우의 동작을 else문에서 표현한다.    
먼저, if을 추가하여, 가로, 세로 입력한 값이 5개 범위 내인지를 점검합니다. 만약 벗어 났으면 Print로 알려 줍니다. 그리고 범위안에 있으면 찾지 못했다고 알려주고, 그 위치에 "X"를 표시합니다. 그리고 최종 좌표를 보여줍니다. 
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

<br>
<br>    
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





**설명:**     
이미 추측하여 입력값 좌표를 다시 입력시 어떻게 이미 입력한 값인지를 알 수 있을까?    
`print board[guess_row][guess_col]`는 반환 값이 "X" 이거나 "O" 일 것이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Add an elif to see if the guessed location already has an 'X' in it.

* If it has, print "You guessed that one already."


**설명:**     
① 기존에 추가한 if 문 밑에 elif 문을 추가하라. elif 문 내용은 다음과 같다.    
• 만약 입력 받은 위치가 이전에 입력 받은 좌표 즉, 해당 위치 값이 "X" 이면 "You guessed that one alrady."라는 메시지를 출력하여라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember to use two equal signs (**`==`**) when you're checking for equality.


**설명:**     
`==` 는 비교할때 양쪽의 값이 같다는 뜻이다. if 문에서 `==`을 활용하라. 
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

**설명:**     
리스트 `board[guess_row][guess_col] == 'X'`인지를 확인해서 이미 입력 된 값인지를 점검한다. 
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

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 14. Test Run    

Congratulations! Now you should have a game of Battleship! that is fully functional for one guess.

Make sure you play it a couple of times and try different kinds of incorrect guesses. This is a great time to stop and do some serious debugging.

In the next step, we'll move on and look at how to give the user 4 guesses to find the battleship.



**설명:**    
여러번 실행해 보고, 입력하여, 문법적으로, 내용적으로 이상이 없는지 확인해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Thoroughly test your game. Make sure you try a variety of different guesses and look for any errors in the syntax or logic of your program.


**설명:**     
① 여러번 실행해서 문법적이나, 로직상 문제가 없는지 확인해 보자. 소스가 어떻게 동작되는지를 확인해 보는것도 좋다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
skip


**설명:**     
skip
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

**설명:**     
skip 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 15. Play It, Sam    

You can successfully make one guess in Battleship! But we’d like our game to allow the player to make up to **4 guesses** before they lose.
```python
for turn in range(4):
  # Make a guess
  # Test that guess
```  
We can use a for loop to iterate through a range. Each iteration will be a turn.





**설명:**     
4번까지 반복하여 도전할 수 있는 소스를 만들어 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Add a for loop that **repeats the guessing** and checking part of your game for **4** turns, like the example above.

At the beginning of each iteration, **`print "Turn"`**, **`turn + 1`** to let the player know what turn they are on.

Indent everything that should be repeated.


**설명:**     
① 4번까지 질문 할 수 있는 반복문을 추가하라. 반복문의 끝에는 몇번 시도했는지를 표시해 주는 출력문  `print ( "Turn :", turn+1)`을 추가 하여 알려준다. 반복되는 for 문 안쪽에 들여쓰여진 모든 소스는 반복된다.      
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Don't forget to **indent the code**!


**설명:**     
for 문안 모두 반복되어야 할 소스를 들여쓰기를 해야 한다. 
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

**설명:**     
`for turn in range(4):`는 4번 반복 한다.  
for 문 안에 들여 쓰진 모든 소스들이 4번 반복된다. 
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
Turn 2
Guess Row: 2
Guess Col: 2
You missed my battleship!
O O O O O
O X O O O
O O X O O
O O O O O
O O O O O
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

<br>
<br>    
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




**설명:**    
플레이어가 추측을 못하여 게임이 끝나면, 게임은 그냥 끝나는 겁니다. 게임이 끝났으면 끝났다고 알려주면 좋을 것이다.         
소스의 어느 위치에 이 기능을 넣어야 할지를 잘 생각해야 한다.    
우리는 3번의 기회가 끝나고 틀렸으면 그 위치에 메시지를 넣어 주기를 원한다. 어디가 좋을지 생각해 보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Add an if statement that checks to see if the user is out of guesses.

* Put it under the else that accounts for misses.
* Put it after the if/elif/else statements that check for the reason the player missed. We want "Game Over" to print regardless of the reason.
* If turn equals 3, print "Game Over".




**설명:**     
① if 문을 추측이 끝나는 위치에 넣어 주자.     
•  else 문 밑에 실패 했을때 위치에 넣어 주자. 
•  플레이어가 못 맞췄을 경우의 if/elif/else 밖에 새로 넣어주자. 
•  변수 `turn`이 3이면 "Game Over"를 출력하자.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Your new if should go under the else that handles all of the incorrect guesses, but outside of any of the nested conditions. This is because it doesn't matter why the guess is wrong; after 4 wrong guesses, the game is over.




**설명:**     
새로운 if는 3번 틀렸을는지를 점검하는데 사용하라. 기존 틀렷는지를 점검하는 if/elif/else에는 속하지 않는다.   
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

**설명:**     
`if (turn == 3):`는 입력값 check 인 if/elif/else 문 안에 넣지 않고 마지막 바깥에 넣어 둔다. 
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

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 17. A Real Win    

Almost there! We can play Battleship!, but you’ll notice that when you win, if you haven’t already guessed 4 times, the program asks you to enter another guess. What we’d rather have happen is for the program to end—it’s no fun guessing if you know you’ve already sunk the Battleship!

We can use the **break command** to get out of a for loop.





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

**설명:**     
4번의 기회를 다 사용 하기 전에 플레이어가 이기면 멈춰야 한다. 그런데, 위 내용을 보면,  이겼는데도, 질문을 한다면 그 프로그램은 잘못 된 것이다. break문을 사용하여 loop를 빠져나가 보자. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Add a **break** under the win condition to end the loop after a win.


**설명:**     
① 승리한 영역에서 `break`를 걸어서 loop를 빠져나가 보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Your break should go inside your outer if statement, right after your "Congratulations!" message.


**설명:**    
승리한 위치는 "Congratulations!!" 메시지 출력 되는 다음 라인이다. 
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

**설명:**     
break 문을 만나면 loop를 빠져나간다.  
{: .notice--info}


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

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 18. To Your Battle Stations!    

Congratulations! You have a fully functional Battleship game! Play it a couple of times and get your friends to try it out, too. (Don’t forget to go back and remove the debugging output that gives away the location of the battleship!)

You may want to take some time to clean up and document your code as well.





**설명:**     
프로그램은 모두 완성되었다. Debugging을 위한 배의 위치를 알려주는 print문 마지막에 삭제해야 한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** When you are done playing Battleship! and are ready to move on, click Run.


**설명:**     
① Debugging을 위하여 배의 위치를 알려주는 정보를 삭제 해 보자. 그리고 실행해 보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
whether remove or comment


**설명:**    
삭제하거나, comment 처리 할수 있다.  
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

**설명:**     
이 소스에서는 배의 위치를 알려주는 소스를 삭제 하지 않고 comment 처리를 하였다. 
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

<br>
<br>    
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





**설명:**     
배틀쉽 게임을 더 확장할수 있다.     
① 배틀쉽을 여러대를 보드에 넣어서 찾을 수 있다.    
② 배틀쉽 board 사이즈를 더 크게 확장 할 수 있다.    
③ 플레이어가 1인용이 아니라, 여러명이 할수 있게 만들 수 있다.    
④ 게임의 특징을 rematch 기능을 넣어 보다 다채롭게 만들수 있다.    
한번 도전해 봐라. 당신은 이제 전문 게임 프로그래머가 되었다.    
{: .notice--info}

