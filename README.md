# eecs2031-lab-3-solved
**TO GET THIS SOLUTION VISIT:** [EECS2031 Lab 3 Solved](https://www.ankitcodinghub.com/product/eecs2031-lab-3-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91343&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EECS2031 Lab 3 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
LAB 3 Arrays and Strings, Bitwise operations, Type conversion, Program structures, local vs. global variables, Functions (pass-by-value), Debuggers

0. Problem 0 Arrays and Strings (cont.)

This and the next question involve further exercise on manipulating arrays and strings — topics in week 2. Arrays are so important in C that we will deal with them throughout the course. Download problem0.c. This short program uses an array of size 20 to store input strings read in using scanf, and simply outputs the array elements (char and its index) after each read. First observe the initial values of the array. Arrays without explicit initializer get random values. Now enterhelloworld, observe that the array is store ash e l l o w o r l d \0 …… where …… are some other values (\0 or random value).

Next, enter a shorter word such as good, then observe that the array is stored as g o o d \0 w o r l d \0 …..

Next, enter hi, then observe that the array is store as h i \0 o d \0 w o r l d \0 …… Now enter a word that is longer than helloworld(but less than 20 chars), see what happens. The point here is that when an array is used to store a string, not all array elements got reset. So when you enter hello, don’t assume that the array contains character h e l o and \0 only – there may exist random values, there may also exist characters from previous storage. So it is always critical to identify the first \0 encountered when scanning from left to right, ignoring characters thereafter. Actually, String manipulation library functions, such as printf(“%s”), strlen, strcpy, strcmp follow this rule: scan from left to right, terminate after encountering the first \0 character. Your string related functions should follow the same rule. No submission for problem 0.

1. Problem A Arrays and Strings (cont.)

1.1 Specification

Write an ANSI-C program that reads inputs line by line, and determines whether each line of input forms a palindrome. A palindrome is a word, phrase, or sequence that reads the same backward as forward, e.g., “madam”, “dad”.

1.2 Implementation

<ul>
<li>name your program lab3panlindrom.c</li>
<li>assume that each line of input contains no space, and contains at most 30 characters</li>
<li>define a function int isPalindrome (char []) which determines whether the
input array (string) is a palindrome.
</li>
<li>for each input word, first prints it backward, and then determines if it is a palindrome, as
shown in the sample output below.
</li>
<li>keep on reading until a word quit is read in. You can use the isQuit() function you
implemented in lab2, but you are also encouraged to explore the string library function strcmp(). You can issue man strcmp to view the manual. Note that this function returns 0 (false) if the two argument strings are equal. This is the only string library function you should use. Don’t use other string library functions such as strlen, strcpy.
</li>
<li>[bonus] You are encouraged not to use an extra array. Just manipulate the original array. 1</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
1.3 Sample Inputs/Outputs:

</div>
</div>
<div class="layoutArea">
<div class="column">
red 477 % a.out hello

olleh

Is not a palindrome

thisisgood

<pre>doogsisiht
Is not a palindrome
</pre>
lisaxxasil

<pre>lisaxxasil
Is a palindrome
</pre>
dad

<pre>dad
Is a palindrome
</pre>
123454321

<pre>123454321
Is a palindrome
</pre>
33

<pre>33
Is a palindrome
</pre>
A

<pre>A
Is a palindrome
</pre>
quit

red 478 %

Submit your program using

</div>
<div class="column">
<pre>submit 2031Z lab3 lab3palindrome.c
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
2 Problem B0 Bitwise operations

In class we covered bitwise operators &amp; | ~ and &lt;&lt; &gt;&gt;. It is important to understand that,

<ul>
<li>when using bitwise operator &amp; |, there are 4 combinations. Following the truth table of
Boolean Algebra (True AND True is True, False AND True is False etc.), for a bit, &amp;0 turn the

bit off (set it to 0),|1 turns the bit on (set it to 1), &amp;1 and | 0 keep the bit value.
</li>
<li>each bitwise operation generates a new value but does not change the operand itself. For
example, flag &lt;&lt;4, flag &amp; 3, flag | 5 does not change flag. In order to change flag, you have to useflag = flag &lt;&lt;4, flag = flag &amp; 3, flag = flag | 5, or their compound assignment versions flag &lt;&lt;= 4, flag &amp;=3, flag |= 5.

Download provided file lab3B0,c. This program reads integers from stdin, and then performs several bitwise operations. It terminates when -1000 is entered.

Compile and run the program with several inputs, and observe
</li>
</ul>
• what the resulting binary representations look like when the input b is left bit shifted by 4,

and is bit flipped. Note that expression b &lt;&lt; 4 or ~b does not modify b itself, so the program uses the original value for other operations.

</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
<ul>
<li>how 1 &lt;&lt; 4 is used with | to turn on bit 4 (denote the right-most bit as bit 0). Again, expression flag | 1&lt;&lt;4 does not change flag itself.
As a C programming idiom (code pattern), flag = flag|(1&lt;&lt;j) turns on bit j of flag.
</li>
<li>what the bit representation of ~(1&lt;&lt;4) looks like, and how it is used with bitwise operator &amp; to turn off bit 4. As a C programming idiom here, flag = flag &amp; ~(1 &lt;&lt; j) turns
off bit j of flag.

Also observe here that parenthesis is needed around 1&lt;&lt;4 because operator &lt;&lt; has lower precedence than operator ~. (What is the result of ~1&lt;&lt;4 ?)
</li>
<li>how 1 &lt;&lt; 4 is used with &amp; to keep bit 4 and turn off all other bits. As a programming idiom, if (flag &amp; 1&lt;&lt;j) is used to test whether bit j of flag is on (why?).</li>
<li>what the bit representation of 077 looks like, and how it is used with &amp; to keep the lower 6 bits and turn off all other bits. all bit except the lower 7 bits.</li>
<li>what the bit representation of ~077 looks like, and how it is used with &amp; to turn off lower 6 bits and keep all other bits.
Enter different numbers, trying to understand these bitwise idioms.

Then, look at the code after the big while loop. Based on one of the idioms mentioned above, what is the binary representation of flag is when the small while loop terminates?

When you are sure you know the answer, confirm by uncommenting the printBinary line after the small while loop, and compile and run the program.

Lastly, trace the code of the for loop and try to understand what the code intends to do. This loop uses one of the idioms mentioned above. Figure out the output of the loop. When you are confident, uncomment this loop and confirm your answer.

No submission for this question. Doing this exercise gets you better prepared for problem B.

3. Problem B Bitwise operation

3.1 Specification

A digital image is typically stored in computer by means of its pixel values, as well as some formatting information. Each pixel value consists of 3 values of 0 ~ 255, representing red (R), green (G) and blue (B).

As mentioned in class, Java’s BufferedImage class has a method int getRGB(int x,int y), which allows you to retrieve the RGB value of an image at pixel position (x,y). How could the method return 3 values at a time? As mentioned in class, the ‘trick’ is to return an integer (32 bits) that packs the 3 values into it. Since each value is 0~255 thus 8 bit is enough to represent it, an 32 bits integer has sufficient bits. They are packed in such a way that, counting from the right most bit, B values occupies the first 8 bits (bit 0~7), G occupies the next 8 bits, and R occupies the next 8 bits. This is shown below. (The left-most 8 bits is packed with some other information about the image, called Alpha, which we are not interested here.)

31 302928272625242322212019 181716151413121110 9 8 7 6 5 4 3 2 1 0

0

76543210765432107654321076543210 Suppose a pixel has R value 2 (which is binary 00000010), G value 7 (which is binary 00000111)

and B value 8 (which is binary 00001000), and Alpha has value 100, then the integer is packed as

00101010000000100000011100001000 100 for Alpha 2 7 8
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
3.2 Implementation

In this exercise, you are going to use bitwise operations to pack input R,G and B values into an integer, and then use bitwise operations again to unpack the packed integer to retrieve the R, G and B values.

Download and complete lab3RGB.c. This C program keeps on reading input from the stdin. Each input contains 3 integers representing the R, G and B value respectively, and then outputs the 3 values with their binary representations. The binary representations are generated by calling function void printBinary(int val), which is defined for you in another program binaryFunction.c.(How do you use a function that is defined in another file?) Next is the pack part that you should implement. This packs the 3 input values, as well as Alpha value which is assumed to be 100, into integer variable rgb_pack.

Then the value of rgb_pack and its binary representation is displayed (implemented for you).

Next you should unpack the R, G and B value from the packed integer rgb_pack.

After that, the unpacked R,G and B value and their Binary, Octal and Hex representations are displayed (implemented for you).

The program terminates when you enter a negative number for either R, G or B value.

Hint: Packing might be a little easier than unpacking. Considering shifting R,G,B values to the proper positions and then somehow merge them into one integer (how about bitwise OR?). For unpacking, you can either do shifting + masking, or, masking + shifting, or, shifting only. Shifting + masking means you first shift the useful bits to the proper positions, and then turn off (set to 0) the unwanted bits while keeping the values of the useful bits. What you want to end up with, for example for R value, is a binary representation of the following, which has decimal value 2.

00000000000000000000000000000010 Masking + shifting means you first use &amp; to turn off some unrelated bits and keep the values of the good bits, and then do a shifting to move the useful bits to the proper position. When doing shifting, the rule of thumb is to avoid right shifting on signed integers. Explore different approaches for unpacking.

Finally, it is interesting to observe that function printBinary() itself uses bitwise operations to generate artificial ‘0’ or ‘1’. It is recommended that, after finishing this lab, you take a look at the code of printBinary yourself.

</div>
</div>
<div class="layoutArea">
<div class="column">
3.3 Sample Inputs/Outputs:

red 339 % a.out enter R value: 1 enter G value: 3 enter B value: 5

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>A: 100
R: 1
G: 3
B: 5
</pre>
Packed:

</div>
<div class="column">
binary: 00000000 00000000 00000000 01100100 binary: 00000000 00000000 00000000 00000001 binary: 00000000 00000000 00000000 00000011 binary: 00000000 00000000 00000000 00000101

binary: 01100100 00000001 00000011 00000101

</div>
<div class="column">
<pre>(1677787909)
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
Unpacking ……

R: binary: 00000000 00000000 00000000 00000001 (1,01,0X1) G: binary: 00000000 00000000 00000000 00000011 (3,03,0X3) B: binary: 00000000 00000000 00000000 00000101 (5,05,0X5) ————————————

</div>
</div>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
enter R value (0~255): 22 enter G value (0~255): 33 enter B value (0~255): 44

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>A: 100
R: 22
G: 33
B: 44
</pre>
Packed:

</div>
<div class="column">
binary: 00000000 00000000 00000000 01100100 binary: 00000000 00000000 00000000 00010110 binary: 00000000 00000000 00000000 00100001 binary: 00000000 00000000 00000000 00101100

binary: 01100100 00010110 00100001 00101100

</div>
<div class="column">
<pre>(1679171884)
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
Unpacking ……

R: binary: 00000000 00000000 00000000 00010110 (22, 026, 0X16) G: binary: 00000000 00000000 00000000 00100001 (33, 041, 0X21) B: binary: 00000000 00000000 00000000 00101100 (44, 054, 0X2C) ————————————

</div>
</div>
<div class="layoutArea">
<div class="column">
enter R value: 123

enter G value: 224

enter B value: 131

A: 100 binary: 00000000 00000000 00000000 01100100 R: 123 binary: 00000000 00000000 00000000 01111011 G: 224 binary: 00000000 00000000 00000000 11100000 B: 131 binary: 00000000 00000000 00000000 10000011

Packed: binary: 01100100 01111011 11100000 10000011

</div>
<div class="column">
<pre>(1685840003)
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
Unpacking ……

R: binary: 00000000 00000000 00000000 01111011 (123, 0173, 0X7B) G: binary: 00000000 00000000 00000000 11100000 (224, 0340, 0XE0) B: binary: 00000000 00000000 00000000 10000011 (131, 0203, 0X83) ————————————

</div>
</div>
<div class="layoutArea">
<div class="column">
enter R value: 254 enter G value: 123 enter B value: 19

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>A: 100
R: 254
G: 123
B: 19
</pre>
Packed:

</div>
<div class="column">
binary: 00000000 00000000 00000000 01100100 binary: 00000000 00000000 00000000 11111110 binary: 00000000 00000000 00000000 01111011 binary: 00000000 00000000 00000000 00010011

binary: 01100100 11111110 01111011 00010011

</div>
<div class="column">
<pre>(1694399251)
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
Unpacking ……

R: binary: 00000000 00000000 00000000 11111110 (254, 0376, 0XFE) G: binary: 00000000 00000000 00000000 01111011 (123, 0173, 0X7B) B: binary: 00000000 00000000 00000000 00010011 (19, 023, 0X13) ————————————

enter R value: -3 enter G value: 3 enter B value: 56 red 340 %

Assume all the inputs are valid.

Submit your program using submit 2031Z lab3 lab3RGB.c

</div>
</div>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
4. Problem C Type conversion in function calls

4.1 Specification

Write an ANSI-C program that reads inputs from the user one integer, one floating point number, and a character operator. The program does a simple calculation based on the two input numbers and the operator. The program continues until both input integer and floating point number are -1.

4.2 Implementation

<ul>
<li>name the program lab3conversion.c</li>
<li>use scanf to read inputs (from Standard input), each of which contains an integer, a
character (‘+’, ‘-‘ ‘*’ or ‘/’) and a floating point number (defined as float)

separated by blanks.
</li>
<li>Use printf to generate outputs representing the operation results</li>
<li>define a function float fun_IF (int, char, float) which conducts arithmetic
calculation based on the inputs
</li>
<li>define another function float fun_II (int, char, int) which conducts
arithmetic calculation based on the inputs
</li>
<li>define another function float fun_FF (float, char, float) which conducts
arithmetic calculation based on the inputs
</li>
<li>note that these three functions should have the same code in the body. They only differ in
the arguments type and return type.
</li>
<li>pass the integer and the float number to both the three functions directly, without explicit
type conversion (casting)., i.e., fun_IF(i,f) and fun_II(i,f)d fun_FF(i,f)
</li>
<li>display before each input the following prompt:
Enter operand_1 operator operand_2 separated by blanks&gt;
</li>
<li>display the outputs as follows (on the same line. One blank between each words) Your input ‘x xx xxx’ results in xxxx (fun_IF) and xxxxx (fun_II) and xxxxxx (fun_FF)
4.3 Sample Inputs/Outputs: (on the single line)

red 329 % gcc -o lab3Cov lab3conversion.c red 330 % lab3Cov

Enter operand_1 operator operand_2 separated by blanks&gt;12 + 22.3024 Your input ’12 + 22.302401′ result in 34.302399 (fun_IF) and 34.000000 (fun_II) and 34.302399 (fun_FF)

Enter operand_1 operator operand_2 separated by blanks&gt;12 * 2.331 Your input ’12 * 2.331000′ result in 27.972000 (fun_IF) and 24.000000 (fun_II) and 27.972000 (fun_FF)

Enter operand_1 operator operand_2 separated by blanks&gt;2 / 9.18 Your input ‘2 / 9.180000’ result in 0.217865 (fun_IF) and 0.000000 (fun_II) and 0.217865 (fun_FF)

Enter operand_1 operator operand_2 separated by blanks&gt;-1 + -1

red 331 %

Do you understand why the results of the fun-IF and fun-FF are same but both are different from fun-II? Write your justification briefly on the program file (as comments).

Assume all the inputs are valid.

Submit your program using submit 2031Z lab3 lab3conversion.c
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="layoutArea">
<div class="column">
5.0 Problem D0 scope, life time and initialization of global

variables, local variables and static local variables

Download the files lab3D0.c and cal.c, compile them together using gcc lab3D0 cal.c (the order does not matter), and run the a.out file. Observe that global variables x and y, which were defined in cal.c, can be accessed in the main file (x y have global scope), and in order to access x and y, the main file needs to declare them using keyword extern. Moreover, from the output -1 11, we can infer that global variable x, which was not initialized explicitly, got initialized to 0 by the complier. Also observe how the function func_1, which was defined in cal.c, was declared and used in the main file.

Next, uncomment the commented block, and compile the files again. Observe the error message. The problem is that local variable counter’s scope is the block/function in which it is defined, so it is not accessible to the main function. In our case its scope is within function aFun. Commentouttheprintfline,compileandrunit.

Observe that function aFun is called several times. Local variable counter in the function, which has life time ‘automatic’ – comes to life when aFun is called and vanishes when aFun returns – is created and initialized each time the function is called.

Next, make counter a static local variable, compile and run again. Observe that the value of counter is different in each call and its value are maintained during function calls, due to the fact that in C a static local variable has persistent life time over function calls. (Note that, a static local variable’s scope is still within the block where it is defined. So counter is still not accessible outside the function.) Also observe that compound operator += is used.

Finally, remove the initial value 100 for counter, compile and run again, and observe that in the first time call counter gets an initial value 0. As discussed in class, global variables and static local variables get initial value 0 if not initialized explicitly. Local variables, however, are not initialized (or, more precisely, are initialized with some garbage values).

No submission for this question.Submit your program usingsubmit 2031 lab3 lab3D0.c 5. Problem D1

5.1 Specification

Complete the ANSI-C program runningAveLocal.c, which should read integers from the standard input, and computes the running (current) average of the input integers. The program terminates when a -1 is entered. Observe

<ul>
<li>how the code display the running average with 3 decimal points.</li>
<li>how a pre-processing macro MY_PRINT(x,y,z) printf( …… )is defined, which
displays the result as shown in the sample outputs. (Thus, the program use MY_PRINTF, rather than printf() to display averages.) we will cover pre-processing next week.

5.2 Implementation
</li>
</ul>
• define a function double runningAverage(int currentSum, int inputCount)which, given the current sum currentSum and the number of input inputCount, computes and returns the running average in double. The current sum and input count are maintained in main.

</div>
</div>
<div class="layoutArea">
<div class="column">
7

</div>
</div>
</div>
<div class="page" title="Page 8">
<div class="layoutArea">
<div class="column">
5.3 Sample Inputs/Outputs:

red 307 % gcc –Wall runningAveLocal.c

red 308 % a.out

enter number (-1 to quit): 10

running average is 10 / 1 = 10.000 Floor is 10 Ceiling is 10

enter number (-1 to quit): 20

running average is 30 / 2 = 15.000 Floor is 15 Ceiling is 15

enter number (-1 to quit): 33

running average is 63 / 3 = 21.000 Floor is 21 Ceiling is 21

enter number (-1 to quit): 47

running average is 110 / 4 = 27.500 Floor is 27 Ceiling is 28

enter number (-1 to quit): 51

running average is 161 / 5 = 32.200 Floor is 32 Ceiling is 33

enter number (-1 to quit): 63

running average is 224 / 6 = 37.333 Floor is 37 Ceiling is 38

enter number (-1 to quit): -1 red 309 %

Assume all the inputs are valid.

Submit your program using submit 2031Z lab3 runningAveLocal.c nerated runningAve.out

6. Problem D2 6.1 Specification

Modify the above program, simplifying communications between functions.

6.2 Implementation

<ul>
<li>name the program runningAveLocal2.c.</li>
<li>define a function double runningAverage(int currentInput),which, given
the current input currentInput, computes and returns the running average in double. Notice that compared against the previous program, this function takes only one argument current input and does not take current sum and input count as its arguments. In such a implementation, current sum and input count are not maintained in main. Instead, main just pass currentInput to runningAverage(), assuming that runningAverage() somehow maintains the current sum and input count info.
</li>
<li>do not use any global variable. How can runningAverage maintain the current sum and input count info?

Hint: static can be used to local variables to make their lifetime permanent.

6.3 Sample Inputs/Outputs:

Same as in problem D1.

Submit your program using submit 2031 lab3 runningAveLocal2.c
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</div>
<div class="page" title="Page 9">
<div class="layoutArea">
<div class="column">
7. Problem D3

7.1 Specification

Modify the program above, further simplifying communications between functions by using global variables.

7.2 Implementation

<ul>
<li>named your program runningAveGlobal.c, which contains the main()function.</li>
<li>define a function void runningAverage(), which computes the running average in double. Notice that this function takes no arguments and does not return anything.</li>
<li>PutthedefinitionofrunningAverage()inanotherfile, namethefilefunction.c.</li>
<li>define all global variables in function.c
7.3 Sample Inputs/Outputs:

Same as in problem D1. Submit your program using

submit 2031 lab3 runningAveGlobal.c function.c

As a practice, make one of the global variables in function.c to be static, and compile the programs. Observe that the static global variable becomes inaccessible in main().

c

8. Problem E Pass-by-value, and trace a program with debugger 8.1 Specification

In this exercise you will practice tracing/debugging a program using a software tool called debugger, rather than using print statements. The key technique of debugging a program is to examine the values of variables during program execution. With a debugger, you can do this by setting several “breakpoints” in the program. The program will pause execution at the breakpoints and you can then view the current values of the variables.

You will use a GNU debugger call gdb. It is a command line based debugger but also comes with a simple text-based gui (tui).

To debug a C program using gdb, you need to compile the program with –g flag.

8.2 Implementation

Download the program swap.c, and compile using gcc –g swap.c. Then invoke gdb by issuing gdb –tui a.out.

A window with two panels will appear. The upper panel displays the source code and the lower panel allows you to enter commands. Maximize the terminal and use arrow keys to scroll the upper panel so you can see the whole source code.

First we want to examine the values of variables mainA and mainB after initialization. So we set a breakpoint at the beginning of line 11 (before line 11 is executed) by issuing break 11. Observe that a ”B+” symbol appears on the left of line 11. We want to trace the values of variables x and y defined in function swap, both before and after swapping. So we set breakpoints at (the beginning of) line 18 and line 21. Finally we set a breakpoint at line 12 so that we can trace the value of mainA and mainB after the function call.

When the program pauses at a breakpoint, you can view the current values of variables with the print or display or even printf command.
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
9

</div>
</div>
</div>
<div class="page" title="Page 10">
<div class="layoutArea">
<div class="column">
8.3 Sample inout/output

red 64 %gcc –Wall –g swap.c red 65 %gdb –tui a.out

….

Reading symbols from a.out…done. (gdb) break 11

</div>
</div>
<div class="layoutArea">
<div class="column">
Breakpoint 1 at

(gdb) break 18

Breakpoint 2 at

(gdb) break 21

Breakpoint 3 at

(gdb) break 12

Breakpoint 4 at

(gdb) run

Starting program: /eecs/home/huiwang/a.out

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>0x400488: file swap.c, line 11.
0x4004a3: file swap.c, line 18.
0x4004b5: file swap.c, line 21.
0x400497: file swap.c, line 12.
</pre>
</div>
<div class="column">
<pre>/* run the program until the
first breakpoint. Notice the &gt;
sign on the left of the upper
panel */
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
Breakpoint 1, main () at swap.c:11 (gdb) display mainA

mainA = ?

(gdb) display mainB

mainB = ? (gdb) continue Continuing.

</div>
<div class="column">
<pre>What do you get for
mainA and mainB?
</pre>
<pre>           /* continue execution to the next
           breakpoint. Notice the position
           of  &gt; sign */
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
Breakpoint 2, swap (x=1, y=20000) at swap.c:18 (gdb) display x

x=? What do you get

</div>
</div>
<div class="layoutArea">
<div class="column">
(gdb) display y y=?

(gdb) display mainA ……?

(gdb) display mainB ……?

(gdb) continue Continuing.

</div>
<div class="column">
for x and y?

<pre> What do you get
 for mainA and
 mainB, and why?
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
Breakpoint 3, swap (x=20000, y=1) at swap.c:21

</div>
</div>
<div class="layoutArea">
<div class="column">
(gdb) display x x=?

(gdb) display y y=?

(gdb) continue Continuing.

Breakpoint 4, main () at swap.c:12 (gdb) display mainA

mainA = ?

(gdb) display mainB

mainB = ?

(gdb) display x ……?

(gdb) display y ……?

(gdb) quit

</div>
<div class="column">
<pre>What do you get for x
and y? Are they
swapped?
</pre>
<pre> What do you get for mainA
 and mainB? Are they
 swapped?
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>What do you get here, and
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
What do you get for mainA and

</div>
</div>
<div class="layoutArea">
<div class="column">
why?

</div>
</div>
<div class="layoutArea">
<div class="column">
mainB? Are they swapped?

</div>
</div>
<div class="layoutArea">
<div class="column">
10

</div>
</div>
</div>
<div class="page" title="Page 11">
<div class="layoutArea">
<div class="column">
8.4 Submission

Write your answers into a text file, and submit it. Or submit a snapshot of your gdb session.

<pre>             submit 2031Z lab3 text_file_or_pictures
</pre>
In summary you should submit:

lab3palindrome.c, lab3RGB.c, lab3conversion.c, runningAveLocal.c, runningAveLocal2.c, runningAveGlobal.c, function.c, file-for- problemE

Common Notes

All submitted files should contain the following header:

/*************************************** * EECS2031 – Lab3 *

* Author: Last name, first name *

* Email: Your email address *

* eecs_username: Your eecs login username * * york_num: Your student number * ****************************************/

In addition, all programs should follow the following guidelines:

<ul>
<li>Include the stdio.h library in the header of your .c files.</li>
<li>Use /* */ to comment your program. You are not encouraged to use //.</li>
<li>Assume that all inputs are valid (no error checking is required, unless
asked to do so).

You are also encouraged to
</li>
</ul>
<ul>
<li>Give a return type int for main(), and return 0 at the end of main()</li>
<li>Specify parameters for main() function, as main(int argc, char *argv[])</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
11

</div>
</div>
</div>
<div class="page" title="Page 12">
<div class="layoutArea">
<div class="column">
5. Problem E

5.0 purpose

The purpose of this and next question is for you to get familiar with some library functions.

Some of functions from Tuesday’s lecture are listed below:

</div>
</div>
<div class="layoutArea">
<div class="column">
&lt;stdio.h&gt;

<pre>sprintf()
scanf()
</pre>
<pre>gets()
fgets()
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
&lt;sting.h&gt;

<pre>strlen(s)
strcpy(s,s)
strcat(s,s)
strcmp(s)
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
&lt;ctype.h&gt;

<pre>int isdigit(int)
int isalpha(int)
int islower(int)
int isupper(int)
</pre>
<pre>int tolower(int)
int toupper(int)
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
For exact prototypes of these functions, you can 1) use ‘man 3 function’ under Unix 2) look at yesterday’s slides 3) look at Appendix B of the textbook. 4) search the web

You are encouraged to use some of these functions for this question, especially string functions. Don’t forget to include the corresponding header files. You don’t need to link any libraries, unless you use functions from &lt;math.h&gt;

5.1 Specification

Complete the ANSI-C program q5.c that reads user information from the standard inputs, and outputs both the original and the modified version of the records.

5.2 Implementation

The program should:

<ul>
<li>use loop to read inputs (from standard in), one input per line, about the user information
in the form of name age wage, where age is an integer literal, and wage is a floating point

literal with up to 2 decimal number. See sample input below.
</li>
<li>use scanf(“%s %s %s”, name, age, wage) to read in three input ‘strings’;</li>
<li>continue reading input, until a name xx is entered.</li>
<li>after reading each line of inputs, create a string resu of the modified version of the
input. In the modified version of input, the first letter of name is capitalized, age becomes

age + 10, and wage has 100% increase.
</li>
<li>Then copy the array/string resu to resu2</li>
<li>Then output both the two resulting strings resu and resu2.</li>
<li>Before terminating, display the current date and time and your program name.</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
&lt;stdlib.h&gt;

<pre>double atof(s)
int    atoi(s)
long   atol(s)
</pre>
int abs(int)

</div>
</div>
<div class="layoutArea">
<div class="column">
&lt;math.h&gt;

<pre>pow()
sqrt()
ceil()
floor()
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
12

</div>
</div>
</div>
<div class="page" title="Page 13">
<div class="layoutArea">
<div class="column">
5.3 Sample Inputs/Outputs:

red 117 % gcc q5.c

red 118 % a.out

input name age and wage: hui 22 33.3 Hui-32-66.600 Hui-32-66.600

input name age and wage: john 60 1.0 John-70-2.000 John-70-2.000

input name age and wage: lisa 30 1.34 Lisa-40-2.680 Lisa-40-2.680

input name age and wage: judy 40 3.2 Judy-50-6.400 Judy-50-6.400

input name age and wage: xx 2 2 Jan 30 2013 00:07:17 q5.c

red 119 %

1.5 submission:

When you are confident that you program works correctly, submit your program using

<pre>                     submit 2031 lab4 lab4a.c
</pre>
6. Problem F (Advanced)

6.1 Specification

Write an ANSI-C program that reads user information from the standard inputs, and outputs both the original and the modified version of the records.

6.2 Implementation

The program should:

<ul>
<li>be named lab4a.c</li>
<li>use a 2-D array to record the inputs</li>
<li>use loop to read inputs (from standard in), one input per line, about the user information
in the form of name age wage, where age is an integer literal, and wage is a floating point

literal with 1 decimal number. See sample input below.
</li>
<li>continue reading input, until a name xx is entered.</li>
<li>after reading all the inputs, output both original input and the modified input, with each
original input followed by a modified version of the input. In the modified version of input,

the name is capital case, age becomes age + 10, and wage has 50% increase.
</li>
<li>display the current date and time at the beginning of the output</li>
<li>assume there are no more than 10 inputs.
6.3 Sample Inputs/Outputs:

<pre>indigo 307 % lab4a
</pre>
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
13

</div>
</div>
</div>
<div class="page" title="Page 14">
<div class="layoutArea">
<div class="column">
<pre>input name age and wage: john 60 1.0
input name age and wage: eric 30 1.3
input name age and wage: lisa 22 2.2
input name age and wage: judy 40 3.2
input name age and wage: xx 2 2
</pre>
<pre>records generated Jun  1 2011 00:06:57
john 60 1.0
JOHN 70 1.5
eric 30 1.3
</pre>
<pre>ERIC 40 2.0
lisa 22 2.2
LISA 32 3.3
judy 40 3.2
JUDY 50 4.8
indigo 308 %
</pre>
6.4 Testing:

You can test your program by using the provided sample input and output file. Sample input and out file are located at /cs/dept/course/2010-11/S/2031/records.in /cs/dept/course/2010-11/S/2031/records.out

6.5 submission:

When you are confident that you program works correctly, submit your program using

<pre>                     submit 2031 lab4 lab4a.c
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
7. Common Notes

</div>
</div>
<div class="layoutArea">
<div class="column">
All submitted files should contain the following header:

/*************************************** * CSE2031 – Lab4 *

* Filename: Name of file *

* Author: Last name, first name *

* Email: Your email address *

* cs_num: Your cs number * ****************************************/ In addition, all programs should follow the following guidelines:

<ul>
<li>Include the stdio.h library in the header of your .c files.</li>
<li>Declare variables at the beginning of main function.</li>
<li>Use /* */ to comment your program. You can not encouraged to use //</li>
<li>Assume that all inputs are valid (no error checking is required).</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
14

</div>
</div>
</div>
